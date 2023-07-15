# Comparing `tmp/glmtuner-0.1.0.tar.gz` & `tmp/glmtuner-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glmtuner-0.1.0.tar", last modified: Fri Jul 14 19:09:51 2023, max compression
+gzip compressed data, was "glmtuner-0.1.1.tar", last modified: Sat Jul 15 16:54:28 2023, max compression
```

## Comparing `glmtuner-0.1.0.tar` & `glmtuner-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,82 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.891990 glmtuner-0.1.0/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    17554 2023-07-14 19:09:51.887990 glmtuner-0.1.0/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    16982 2023-07-14 19:09:30.000000 glmtuner-0.1.0/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-14 19:09:38.000000 glmtuner-0.1.0/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-14 19:09:51.891990 glmtuner-0.1.0/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-14 19:09:37.000000 glmtuner-0.1.0/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.599989 glmtuner-0.1.0/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.611989 glmtuner-0.1.0/src/glmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.619989 glmtuner-0.1.0/src/glmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5381 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.667989 glmtuner-0.1.0/src/glmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      165 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6604 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/dsets/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-14 19:09:32.000000 glmtuner-0.1.0/src/glmtuner/dsets/preprocess.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.699989 glmtuner-0.1.0/src/glmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2628 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      148 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5086 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1715 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/extras/save_and_load.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.715989 glmtuner-0.1.0/src/glmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-14 19:09:34.000000 glmtuner-0.1.0/src/glmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4282 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3308 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-14 19:09:33.000000 glmtuner-0.1.0/src/glmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-14 19:09:34.000000 glmtuner-0.1.0/src/glmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3497 2023-07-14 19:09:34.000000 glmtuner-0.1.0/src/glmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.715989 glmtuner-0.1.0/src/glmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.727989 glmtuner-0.1.0/src/glmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4129 2023-07-14 19:09:34.000000 glmtuner-0.1.0/src/glmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8597 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5669 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4069 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.735989 glmtuner-0.1.0/src/glmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10912 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2953 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.743989 glmtuner-0.1.0/src/glmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-14 19:09:35.000000 glmtuner-0.1.0/src/glmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1246 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2803 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.767989 glmtuner-0.1.0/src/glmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2200 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2669 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4243 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.875990 glmtuner-0.1.0/src/glmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2548 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1686 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.887990 glmtuner-0.1.0/src/glmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      242 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      612 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1212 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2569 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1991 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3745 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-14 19:09:36.000000 glmtuner-0.1.0/src/glmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1029 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6121 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2023-07-14 19:09:37.000000 glmtuner-0.1.0/src/glmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-14 19:09:51.615989 glmtuner-0.1.0/src/glmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    17554 2023-07-14 19:09:51.000000 glmtuner-0.1.0/src/glmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1967 2023-07-14 19:09:51.000000 glmtuner-0.1.0/src/glmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-14 19:09:51.000000 glmtuner-0.1.0/src/glmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      227 2023-07-14 19:09:51.000000 glmtuner-0.1.0/src/glmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-14 19:09:51.000000 glmtuner-0.1.0/src/glmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.926215 glmtuner-0.1.1/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-15 16:54:23.000000 glmtuner-0.1.1/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18438 2023-07-15 16:54:28.926215 glmtuner-0.1.1/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    17854 2023-07-15 16:54:23.000000 glmtuner-0.1.1/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-15 16:54:23.000000 glmtuner-0.1.1/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-15 16:54:28.930215 glmtuner-0.1.1/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2006 2023-07-15 16:54:23.000000 glmtuner-0.1.1/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.802214 glmtuner-0.1.1/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.854214 glmtuner-0.1.1/src/glmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      250 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.866213 glmtuner-0.1.1/src/glmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       41 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4515 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2053 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.870214 glmtuner-0.1.1/src/glmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2948 2023-07-15 16:54:18.000000 glmtuner-0.1.1/src/glmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.878214 glmtuner-0.1.1/src/glmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      165 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6589 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4249 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7475 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/dsets/preprocess.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.986214 glmtuner-0.1.1/src/glmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3000 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      312 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      751 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5062 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1716 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2172 2023-07-15 16:54:19.000000 glmtuner-0.1.1/src/glmtuner/extras/save_and_load.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.998214 glmtuner-0.1.1/src/glmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      302 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4283 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3309 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      382 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1685 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3310 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.002214 glmtuner-0.1.1/src/glmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      208 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.050214 glmtuner-0.1.1/src/glmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4113 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8739 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5669 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4125 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.058214 glmtuner-0.1.1/src/glmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11291 2023-07-15 16:54:20.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1673 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3022 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.110214 glmtuner-0.1.1/src/glmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      725 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1523 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2888 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.294214 glmtuner-0.1.1/src/glmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2200 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2657 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4208 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.646215 glmtuner-0.1.1/src/glmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       48 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2605 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2394 2023-07-15 16:54:21.000000 glmtuner-0.1.1/src/glmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:28.890215 glmtuner-0.1.1/src/glmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      242 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      612 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1778 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2740 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1311 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/model.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3862 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1030 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6525 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2501 2023-07-15 16:54:22.000000 glmtuner-0.1.1/src/glmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-15 16:54:27.862213 glmtuner-0.1.1/src/glmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18438 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2038 2023-07-15 16:54:27.000000 glmtuner-0.1.1/src/glmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      227 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-15 16:54:26.000000 glmtuner-0.1.1/src/glmtuner.egg-info/top_level.txt
```

### Comparing `glmtuner-0.1.0/PKG-INFO` & `glmtuner-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -16,35 +16,39 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ChatGLM Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/glmtuner)](https://pypi.org/project/glmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/pulls)
 
 Fine-tuning 🤖[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) model with 🤗[PEFT](https://github.com/huggingface/peft).
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 ## Changelog
 
+[23/07/15] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune ChatGLM-6B model in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) for his efforts in the development.
+
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/25] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in arbitrary ChatGPT-based applications.
 
-[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework! Try `--use_v2` argument to fine-tune and predict that model.
+[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework!
 
 [23/06/05] Now we support 4-bit LoRA training (aka [QLoRA](https://github.com/artidoro/qlora)). Try `--quantization_bit 4` argument to work with 4-bit quantized model. (experimental feature)
 
 [23/06/01] We implemented a framework supporting the efficient tuning of LLaMA and BLOOM models. Please follow [LLaMA-Efficient-Tuning](https://github.com/hiyouga/LLaMA-Efficient-Tuning) if you are interested.
 
 [23/05/19] Now we support using the development set to evaluate the model while training. Try `--dev_ratio` argument to specify the size of development set.
 
@@ -139,14 +143,15 @@
 ```
 
 ### Fine-tuning with a Single GPU
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -167,14 +172,15 @@
 ```
 
 ### Training Reward Model
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -186,14 +192,15 @@
 ```
 
 ### Training with RLHF
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -208,53 +215,57 @@
 ```
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
-### CLI Demo
+### API / CLI Demo
 
 ```bash
-python src/cli_demo.py \
+python src/xxx_demo.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### All-in-one Web UI
 
 ```bash
 python src/train_web.py
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.0/README.md` & `glmtuner-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # ChatGLM Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/glmtuner)](https://pypi.org/project/glmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/pulls)
 
 Fine-tuning 🤖[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) model with 🤗[PEFT](https://github.com/huggingface/peft).
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 ## Changelog
 
+[23/07/15] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune ChatGLM-6B model in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) for his efforts in the development.
+
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/25] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in arbitrary ChatGPT-based applications.
 
-[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework! Try `--use_v2` argument to fine-tune and predict that model.
+[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework!
 
 [23/06/05] Now we support 4-bit LoRA training (aka [QLoRA](https://github.com/artidoro/qlora)). Try `--quantization_bit 4` argument to work with 4-bit quantized model. (experimental feature)
 
 [23/06/01] We implemented a framework supporting the efficient tuning of LLaMA and BLOOM models. Please follow [LLaMA-Efficient-Tuning](https://github.com/hiyouga/LLaMA-Efficient-Tuning) if you are interested.
 
 [23/05/19] Now we support using the development set to evaluate the model while training. Try `--dev_ratio` argument to specify the size of development set.
 
@@ -116,14 +119,15 @@
 ```
 
 ### Fine-tuning with a Single GPU
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -144,14 +148,15 @@
 ```
 
 ### Training Reward Model
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -163,14 +168,15 @@
 ```
 
 ### Training with RLHF
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -185,53 +191,57 @@
 ```
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
-### CLI Demo
+### API / CLI Demo
 
 ```bash
-python src/cli_demo.py \
+python src/xxx_demo.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### All-in-one Web UI
 
 ```bash
 python src/train_web.py
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.0/setup.py` & `glmtuner-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/api/app.py` & `glmtuner-0.1.1/src/glmtuner/api/app.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import torch
 import uvicorn
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from contextlib import asynccontextmanager
 from sse_starlette import EventSourceResponse
-from typing import Any, Dict, List
+from typing import List, Tuple
 
-from glmtuner.extras.misc import auto_configure_device_map
-from glmtuner.tuner import get_infer_args, load_model_and_tokenizer
+from glmtuner.tuner import get_infer_args
 from glmtuner.extras.misc import torch_gc
+from glmtuner.chat.stream_chat import ChatModel
 from glmtuner.api.protocol import (
     ModelCard,
     ModelList,
     ChatMessage,
     DeltaMessage,
     ChatCompletionRequest,
     ChatCompletionResponse,
@@ -26,25 +25,15 @@
 @asynccontextmanager
 async def lifespan(app: FastAPI): # collects GPU memory
     yield
     torch_gc()
 
 
 def create_app():
-    model_args, finetuning_args, generating_args = get_infer_args()
-    model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args)
-
-    if torch.cuda.device_count() > 1:
-        from accelerate import dispatch_model
-        device_map = auto_configure_device_map(torch.cuda.device_count(), use_v2=model_args.use_v2)
-        model = dispatch_model(model, device_map)
-    else:
-        model = model.cuda()
-
-    model.eval()
+    chat_model = ChatModel(*get_infer_args())
 
     app = FastAPI(lifespan=lifespan)
 
     app.add_middleware(
         CORSMiddleware,
         allow_origins=["*"],
         allow_credentials=True,
@@ -69,29 +58,21 @@
 
         history = []
         if len(prev_messages) % 2 == 0:
             for i in range(0, len(prev_messages), 2):
                 if prev_messages[i].role == "user" and prev_messages[i+1].role == "assistant":
                     history.append([prev_messages[i].content, prev_messages[i+1].content])
 
-        gen_kwargs = generating_args.to_dict()
-        gen_kwargs.update({
-            "temperature": request.temperature if request.temperature else gen_kwargs["temperature"],
-            "top_p": request.top_p if request.top_p else gen_kwargs["top_p"]
-        })
-
-        if request.max_tokens:
-            gen_kwargs.pop("max_length", None)
-            gen_kwargs["max_new_tokens"] = request.max_tokens
-
         if request.stream:
-            generate = predict(query, history, gen_kwargs, request.model)
+            generate = predict(query, history, request)
             return EventSourceResponse(generate, media_type="text/event-stream")
 
-        response, _ = model.chat(tokenizer, query, history=history, **gen_kwargs)
+        response = chat_model.chat(
+            query, history, temperature=request.temperature, top_p=request.top_p, max_new_tokens=request.max_tokens
+        )
 
         usage = ChatCompletionResponseUsage( # too complex to compute
             prompt_tokens=1,
             completion_tokens=1,
             total_tokens=2
         )
 
@@ -99,47 +80,43 @@
             index=0,
             message=ChatMessage(role="assistant", content=response),
             finish_reason="stop"
         )
 
         return ChatCompletionResponse(model=request.model, choices=[choice_data], usage=usage, object="chat.completion")
 
-
-    async def predict(query: str, history: List[List[str]], gen_kwargs: Dict[str, Any], model_id: str):
+    async def predict(query: str, history: List[Tuple[str, str]], request: ChatCompletionRequest):
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(role="assistant"),
             finish_reason=None
         )
-        chunk = ChatCompletionStreamResponse(model=model_id, choices=[choice_data], object="chat.completion.chunk")
+        chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
         yield chunk.json(exclude_unset=True, ensure_ascii=False)
 
-        current_length = 0
-
-        for new_response, _ in model.stream_chat(tokenizer, query, history, **gen_kwargs):
-            if len(new_response) == current_length:
+        for new_text in chat_model.stream_chat(
+            query, history, temperature=request.temperature, top_p=request.top_p, max_new_tokens=request.max_tokens
+        ):
+            if len(new_text) == 0:
                 continue
 
-            new_text = new_response[current_length:]
-            current_length = len(new_response)
-
             choice_data = ChatCompletionResponseStreamChoice(
                 index=0,
                 delta=DeltaMessage(content=new_text),
                 finish_reason=None
             )
-            chunk = ChatCompletionStreamResponse(model=model_id, choices=[choice_data], object="chat.completion.chunk")
+            chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
             yield chunk.json(exclude_unset=True, ensure_ascii=False)
 
         choice_data = ChatCompletionResponseStreamChoice(
             index=0,
             delta=DeltaMessage(),
             finish_reason="stop"
         )
-        chunk = ChatCompletionStreamResponse(model=model_id, choices=[choice_data], object="chat.completion.chunk")
+        chunk = ChatCompletionStreamResponse(model=request.model, choices=[choice_data], object="chat.completion.chunk")
         yield chunk.json(exclude_unset=True, ensure_ascii=False)
         yield "[DONE]"
 
     return app
 
 
 if __name__ == "__main__":
```

### Comparing `glmtuner-0.1.0/src/glmtuner/api/protocol.py` & `glmtuner-0.1.1/src/glmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/dsets/collator.py` & `glmtuner-0.1.1/src/glmtuner/dsets/collator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,25 @@
     r"""
     Data collator for ChatGLM. It is capable of dynamically padding for batched data.
     """
     def __init__(
         self,
         tokenizer: PreTrainedTokenizer,
         model: PreTrainedModel,
-        ignore_pad_token_for_loss: Optional[bool] = False,
-        use_v2: Optional[bool] = False
+        ignore_pad_token_for_loss: Optional[bool] = False
     ):
         super().__init__(tokenizer, padding=True)
         self.model = model
         self.label_pad_token_id = IGNORE_INDEX if ignore_pad_token_for_loss else tokenizer.pad_token_id
-        if use_v2:
-            self.get_attention_masks = self.get_attention_masks_v2
-            self.get_position_ids = self.get_position_ids_v2
-        else:
+        if tokenizer.eos_token_id == 130005:
             self.get_attention_masks = self.get_attention_masks_v1
             self.get_position_ids = self.get_position_ids_v1
+        else:
+            self.get_attention_masks = self.get_attention_masks_v2
+            self.get_position_ids = self.get_position_ids_v2
 
     def get_attention_masks_v1(self, input_ids: torch.Tensor, device: torch.device) -> torch.Tensor:
         r"""
         Generates attention masks for left-padded sequences.
 
         Note that ChatGLM assigns False on token to be attended in attention mask. In general settings, it should be True.
```

### Comparing `glmtuner-0.1.0/src/glmtuner/dsets/loader.py` & `glmtuner-0.1.1/src/glmtuner/dsets/loader.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/dsets/preprocess.py` & `glmtuner-0.1.1/src/glmtuner/dsets/preprocess.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/extras/callbacks.py` & `glmtuner-0.1.1/src/glmtuner/extras/callbacks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,71 @@
-import os
-import json
-import time
-from datetime import timedelta
-
-from transformers import (
-    TrainerCallback,
-    TrainerControl,
-    TrainerState,
-    TrainingArguments
-)
-
-
-class LogCallback(TrainerCallback):
-
-    def __init__(self, runner=None):
-        self.runner = runner
-        self.start_time = time.time()
-        self.tracker = {}
-
-    def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
-        r"""
-        Event called at the beginning of a training step. If using gradient accumulation, one training step
-        might take several inputs.
-        """
-        if self.runner is not None and self.runner.aborted:
-            control.should_epoch_stop = True
-            control.should_training_stop = True
-
-    def on_substep_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
-        r"""
-        Event called at the end of an substep during gradient accumulation.
-        """
-        if self.runner is not None and self.runner.aborted:
-            control.should_epoch_stop = True
-            control.should_training_stop = True
-
-    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
-        r"""
-        Event called after logging the last logs.
-        """
-        if "loss" not in state.log_history[-1]:
-            return
-        cur_time = time.time()
-        cur_steps = state.log_history[-1].get("step")
-        elapsed_time = cur_time - self.start_time
-        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
-        remaining_steps = state.max_steps - cur_steps
-        remaining_time = remaining_steps * avg_time_per_step
-        self.tracker = {
-            "current_steps": cur_steps,
-            "total_steps": state.max_steps,
-            "loss": state.log_history[-1].get("loss", None),
-            "reward": state.log_history[-1].get("reward", None),
-            "learning_rate": state.log_history[-1].get("learning_rate", None),
-            "epoch": state.log_history[-1].get("epoch", None),
-            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
-            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
-            "remaining_time": str(timedelta(seconds=int(remaining_time)))
-        }
-        os.makedirs(args.output_dir, exist_ok=True)
-        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a", encoding="utf-8") as f:
-            f.write(json.dumps(self.tracker) + "\n")
+import os
+import json
+import time
+from datetime import timedelta
+
+from transformers import (
+    TrainerCallback,
+    TrainerControl,
+    TrainerState,
+    TrainingArguments
+)
+from transformers.trainer_callback import TrainerControl, TrainerState
+from transformers.training_args import TrainingArguments
+
+
+class LogCallback(TrainerCallback):
+
+    def __init__(self, runner=None):
+        self.runner = runner
+        self.start_time = time.time()
+        self.tracker = {}
+
+    def on_train_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the beginning of training.
+        """
+        self.start_time = time.time()
+
+    def on_step_begin(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the beginning of a training step. If using gradient accumulation, one training step
+        might take several inputs.
+        """
+        if self.runner is not None and self.runner.aborted:
+            control.should_epoch_stop = True
+            control.should_training_stop = True
+
+    def on_substep_end(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs):
+        r"""
+        Event called at the end of an substep during gradient accumulation.
+        """
+        if self.runner is not None and self.runner.aborted:
+            control.should_epoch_stop = True
+            control.should_training_stop = True
+
+    def on_log(self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs) -> None:
+        r"""
+        Event called after logging the last logs.
+        """
+        cur_time = time.time()
+        cur_steps = state.log_history[-1].get("step")
+        elapsed_time = cur_time - self.start_time
+        avg_time_per_step = elapsed_time / cur_steps if cur_steps != 0 else 0
+        remaining_steps = state.max_steps - cur_steps
+        remaining_time = remaining_steps * avg_time_per_step
+        self.tracker = {
+            "current_steps": cur_steps,
+            "total_steps": state.max_steps,
+            "loss": state.log_history[-1].get("loss", None),
+            "eval_loss": state.log_history[-1].get("eval_loss", None),
+            "predict_loss": state.log_history[-1].get("predict_loss", None),
+            "reward": state.log_history[-1].get("reward", None),
+            "learning_rate": state.log_history[-1].get("learning_rate", None),
+            "epoch": state.log_history[-1].get("epoch", None),
+            "percentage": round(cur_steps / state.max_steps * 100, 2) if state.max_steps != 0 else 100,
+            "elapsed_time": str(timedelta(seconds=int(elapsed_time))),
+            "remaining_time": str(timedelta(seconds=int(remaining_time)))
+        }
+        os.makedirs(args.output_dir, exist_ok=True)
+        with open(os.path.join(args.output_dir, "trainer_log.jsonl"), "a", encoding="utf-8") as f:
+            f.write(json.dumps(self.tracker) + "\n")
```

### Comparing `glmtuner-0.1.0/src/glmtuner/extras/logging.py` & `glmtuner-0.1.1/src/glmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/extras/misc.py` & `glmtuner-0.1.1/src/glmtuner/extras/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,20 +58,20 @@
     print("trainable params: {:d} || all params: {:d} || trainable%: {:.4f}".format(
                 trainable_params, all_param, 100 * trainable_params / all_param))
 
 
 # Includes: (1) cast the layernorm in fp32 (2) make output embedding layer require grads (3) upcast the lm_head to fp32
 # Inspired by: https://github.com/huggingface/peft/blob/c0209c35abbf88c63aa267800d98a8e212ed0a42/src/peft/utils/other.py#L35
 def prepare_model_for_training(
-        model: PreTrainedModel,
-        finetuning_type: str,
-        output_embedding_base_layer: torch.nn.Module,
-        output_embedding_layer_name: Optional[str] = "lm_head",
-        use_gradient_checkpointing: Optional[bool] = True,
-        layer_norm_names: Optional[List[str]] = LAYERNORM_NAMES
+    model: PreTrainedModel,
+    finetuning_type: str,
+    output_embedding_base_layer: torch.nn.Module,
+    output_embedding_layer_name: Optional[str] = "lm_head",
+    use_gradient_checkpointing: Optional[bool] = True,
+    layer_norm_names: Optional[List[str]] = LAYERNORM_NAMES
 ) -> PreTrainedModel:
 
     for name, param in model.named_parameters():
         if param.ndim == 1 and any(layer_norm_name in name for layer_norm_name in layer_norm_names):
             param.data = param.data.to(torch.float32)
 
     if use_gradient_checkpointing:
```

### Comparing `glmtuner-0.1.0/src/glmtuner/extras/ploting.py` & `glmtuner-0.1.1/src/glmtuner/extras/ploting.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from glmtuner.extras.logging import get_logger
 
 
 logger = get_logger(__name__)
 
 
 def smooth(scalars: List[float], weight: Optional[float] = 0.9) -> List[float]:
-    """
+    r"""
     EMA implementation according to TensorBoard.
     """
     last = scalars[0]
     smoothed = list()
     for next_val in scalars:
         smoothed_val = last * weight + (1 - weight) * next_val
         smoothed.append(smoothed_val)
```

### Comparing `glmtuner-0.1.0/src/glmtuner/extras/save_and_load.py` & `glmtuner-0.1.1/src/glmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/hparams/data_args.py` & `glmtuner-0.1.1/src/glmtuner/hparams/data_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @dataclass
 class DataArguments:
     """
     Arguments pertaining to what data we are going to input our model for training and evaluation.
     """
     dataset: Optional[str] = field(
         default="alpaca_zh",
-        metadata={"help": "The name of provided dataset(s) to use. Use comma to separate multiple datasets."}
+        metadata={"help": "The name of provided dataset(s) to use. Use commas to separate multiple datasets."}
     )
     dataset_dir: Optional[str] = field(
         default="data",
         metadata={"help": "The name of the folder containing datasets."}
     )
     split: Optional[str] = field(
         default="train",
```

### Comparing `glmtuner-0.1.0/src/glmtuner/hparams/finetuning_args.py` & `glmtuner-0.1.1/src/glmtuner/hparams/finetuning_args.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     )
     lora_dropout: Optional[float] = field(
         default=0.1,
         metadata={"help": "Dropout rate for the LoRA fine-tuning."}
     )
     lora_target: Optional[str] = field(
         default="query_key_value",
-        metadata={"help": "Name(s) of target modules to apply LoRA. Use comma to separate multiple modules."}
+        metadata={"help": "Name(s) of target modules to apply LoRA. Use commas to separate multiple modules."}
     )
 
     def __post_init__(self):
         if isinstance(self.lora_target, str):
             self.lora_target = [target.strip() for target in self.lora_target.split(",")] # support custom target modules of LoRA
 
         if self.num_layer_trainable > 0: # fine-tuning the last n layers if num_layer_trainable > 0
```

### Comparing `glmtuner-0.1.0/src/glmtuner/hparams/generating_args.py` & `glmtuner-0.1.1/src/glmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/hparams/model_args.py` & `glmtuner-0.1.1/src/glmtuner/hparams/model_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,14 @@
     """
     Arguments pertaining to which model/config/tokenizer we are going to fine-tune.
     """
     model_name_or_path: Optional[str] = field(
         default="THUDM/chatglm-6b",
         metadata={"help": "Path to pretrained model or model identifier from huggingface.co/models."}
     )
-    use_v2: Optional[bool] = field(
-        default=False,
-        metadata={"help": "Whether to use ChatGLM2 or not."}
-    )
     config_name: Optional[str] = field(
         default=None,
         metadata={"help": "Pretrained config name or path if not the same as model_name."}
     )
     tokenizer_name: Optional[str] = field(
         default=None,
         metadata={"help": "Pretrained tokenizer name or path if not the same as model_name."}
@@ -70,15 +66,15 @@
     )
     plot_loss: Optional[bool] = field(
         default=False,
         metadata={"help": "Whether to plot the training loss after fine-tuning or not."}
     )
 
     def __post_init__(self):
-        if self.use_v2 and self.model_name_or_path == "THUDM/chatglm-6b":
-            self.model_name_or_path = "THUDM/chatglm2-6b"
+        if not self.checkpoint_dir:
+            self.checkpoint_dir = None
 
         if self.checkpoint_dir is not None: # support merging lora weights
             self.checkpoint_dir = [cd.strip() for cd in self.checkpoint_dir.split(",")]
 
         if self.quantization_bit is not None:
             assert self.quantization_bit in [4, 8], "We only accept 4-bit or 8-bit quantization."
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/core/adapter.py` & `glmtuner-0.1.1/src/glmtuner/tuner/core/adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from glmtuner.hparams import ModelArguments, FinetuningArguments
 
 
 logger = get_logger(__name__)
 
 
 def init_adapter(
-        model: PreTrainedModel,
-        model_args: ModelArguments,
-        finetuning_args: FinetuningArguments,
-        is_trainable: bool
+    model: PreTrainedModel,
+    model_args: ModelArguments,
+    finetuning_args: FinetuningArguments,
+    is_trainable: bool
 ) -> PreTrainedModel:
     r"""
     Initializes the adapters.
 
     Support full-parameter, freeze, P-Tuning v2 and LoRA training.
 
     Note that the trainable parameters must be cast to float32.
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/core/loader.py` & `glmtuner-0.1.1/src/glmtuner/tuner/core/loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     AutoConfig,
     AutoModel,
     AutoTokenizer,
     BitsAndBytesConfig
 )
 from transformers.utils import check_min_version
 from transformers.utils.versions import require_version
-from transformers.modeling_utils import PreTrainedModel
+from transformers.modeling_utils import PretrainedConfig, PreTrainedModel
 from transformers.tokenization_utils import PreTrainedTokenizer
 from trl import AutoModelForCausalLMWithValueHead
 
 from glmtuner.extras.logging import get_logger
 from glmtuner.extras.misc import prepare_model_for_training, print_trainable_params
 from glmtuner.extras.save_and_load import load_valuehead_params
 from glmtuner.hparams import ModelArguments, FinetuningArguments
@@ -28,18 +28,18 @@
 require_version("datasets>=2.10.0", "To fix: pip install datasets>=2.10.0")
 require_version("accelerate>=0.19.0", "To fix: pip install accelerate>=0.19.0")
 require_version("peft>=0.3.0", "To fix: pip install peft>=0.3.0")
 require_version("trl>=0.4.4", "To fix: pip install trl>=0.4.4")
 
 
 def load_model_and_tokenizer(
-        model_args: ModelArguments,
-        finetuning_args: FinetuningArguments,
-        is_trainable: Optional[bool] = False,
-        stage: Optional[Literal["sft", "rm", "ppo"]] = "sft"
+    model_args: ModelArguments,
+    finetuning_args: FinetuningArguments,
+    is_trainable: Optional[bool] = False,
+    stage: Optional[Literal["sft", "rm", "ppo"]] = "sft"
 ) -> Tuple[PreTrainedModel, PreTrainedTokenizer]:
     r"""
     Loads pretrained model and tokenizer.
 
     Support both training and inference.
     """
 
@@ -114,30 +114,31 @@
     else:
         model_to_load = model_args.model_name_or_path
 
     # Load and prepare pretrained models (without valuehead).
     model = AutoModel.from_pretrained(model_to_load, config=config, **config_kwargs)
 
     # Register auto class to save the custom code files.
-    if hasattr(config, "auto_map") and "AutoConfig" in config.auto_map:
+    if hasattr(config, "auto_map") and "AutoConfig" in config.auto_map and isinstance(config, PretrainedConfig):
         config.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoTokenizer" in config.auto_map:
+    if hasattr(config, "auto_map") and "AutoTokenizer" in config.auto_map and isinstance(tokenizer, PreTrainedTokenizer):
         tokenizer.__class__.register_for_auto_class()
-    if hasattr(config, "auto_map") and "AutoModel" in config.auto_map:
+    if hasattr(config, "auto_map") and "AutoModel" in config.auto_map and isinstance(model, PreTrainedModel):
         model.__class__.register_for_auto_class()
 
-    if model_args.use_v2:
-        assert tokenizer.eos_token_id is not None, "Please update the *.json and *.py files of ChatGLM2-6B from HuggingFace."
+    if tokenizer.eos_token_id == 130005: # ChatGLM-6B
+        output_embedding_base_layer = model
+        output_embedding_layer_name = "lm_head"
+    elif tokenizer.eos_token_id == 2: # ChatGLM2-6B
+        assert hasattr(model, "transformer"), "Please update the model files of ChatGLM-6B."
         model.lm_head = model.transformer.output_layer
         output_embedding_base_layer = model.transformer
         output_embedding_layer_name = "output_layer"
     else:
-        assert tokenizer.eos_token_id == 130005, "Please specify `use_v2` argument while using ChatGLM2-6B."
-        output_embedding_base_layer = model
-        output_embedding_layer_name = "lm_head"
+        raise ValueError("Please update the model files of ChatGLM2-6B.")
 
     # Initialize adapters
     model = prepare_model_for_training(
         model,
         finetuning_args.finetuning_type,
         output_embedding_base_layer,
         output_embedding_layer_name
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/core/parser.py` & `glmtuner-0.1.1/src/glmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/core/trainer.py` & `glmtuner-0.1.1/src/glmtuner/tuner/core/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import torch
 from typing import Dict, Optional
 
 from transformers import Seq2SeqTrainer
-
 from transformers.trainer import TRAINING_ARGS_NAME
 from transformers.modeling_utils import unwrap_model
 
 from glmtuner.extras.constants import FINETUNING_ARGS_NAME, VALUE_HEAD_FILE_NAME
 from glmtuner.extras.logging import get_logger
 from glmtuner.extras.save_and_load import get_state_dict, load_trainable_params, load_valuehead_params
 from glmtuner.hparams import FinetuningArguments
@@ -20,14 +19,17 @@
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

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/ppo/trainer.py` & `glmtuner-0.1.1/src/glmtuner/tuner/ppo/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import math
 import torch
 from tqdm import tqdm
 from typing import Callable, Dict, List, Optional
 
-from transformers import Seq2SeqTrainingArguments, TrainerState
+from transformers import Seq2SeqTrainingArguments, TrainerState, TrainerControl
 from transformers.modeling_utils import PreTrainedModel
 
 from trl import PPOTrainer, AutoModelForCausalLMWithValueHead
 from trl.core import LengthSampler
 from trl.trainer.ppo_trainer import PPODecorators, logprobs_from_logits
 
 from glmtuner.extras.callbacks import LogCallback
@@ -35,15 +35,17 @@
         **kwargs
     ):
         PPOTrainer.__init__(self, **kwargs)
         self.args = training_args
         self.finetuning_args = finetuning_args
         self.log_callback = callbacks[0]
         self.state = TrainerState()
+        self.control = TrainerControl()
         self.data_collator = self.accelerator.prepare(kwargs["data_collator"]) # override the data collator of PPOTrainer
+        self._remove_log()
 
     def ppo_train(self, max_target_length: int) -> None:
         r"""
         Implements training loop for the PPO stage, like _inner_training_loop() in Huggingface's Trainer.
         """
 
         total_train_batch_size = self.config.batch_size * self.config.gradient_accumulation_steps * self.args.world_size
@@ -80,16 +82,17 @@
         output_length_sampler = LengthSampler(max_target_length // 2, max_target_length)
         unwrapped_model: PreTrainedModel = self.accelerator.unwrap_model(self.model)
 
         dataiter = iter(self.dataloader)
         steps_trained = 0
         loss_meter = AverageMeter()
         reward_meter = AverageMeter()
+        self.log_callback.on_train_begin(self.args, self.state, self.control)
 
-        for step in tqdm(range(max_steps), disable=not self.is_world_process_zero()):
+        for step in tqdm(range(max_steps), disable=not self.is_world_process_zero(), leave=False):
 
             for _ in range(self.config.gradient_accumulation_steps):
 
                 batch = next(dataiter)
                 steps_trained += 1
 
                 unwrapped_model.gradient_checkpointing_disable()
@@ -121,35 +124,41 @@
                 unwrapped_model.config.use_cache = False
 
                 stats = self.step(queries, responses, rewards)
 
                 loss_meter.update(stats["ppo/loss/total"], n=len(rewards))
                 reward_meter.update(torch.stack(rewards).mean().item(), n=len(rewards))
 
+                if self.control.should_epoch_stop or self.control.should_training_stop:
+                    break
+
                 if steps_trained == len_dataloader:
                     dataiter = iter(self.dataloader)
                     steps_trained = 0
 
             if self.is_world_process_zero() and (step+1) % self.args.logging_steps == 0:
                 logs = {
                     "loss": round(loss_meter.avg, 4),
                     "reward": round(reward_meter.avg, 4),
                     "learning_rate": stats["ppo/learning_rate"],
                     "epoch": round(step / num_steps_per_epoch, 2)
                 }
                 print(logs)
                 logs["step"] = step
                 self.state.log_history.append(logs)
-                self.log_callback.on_log(self.args, self.state, None)
+                self.log_callback.on_log(self.args, self.state, self.control)
                 loss_meter.reset()
                 reward_meter.reset()
 
             if (step+1) % self.args.save_steps == 0: # save checkpoint
                 self.save_model(os.path.join(self.args.output_dir, f"checkpoint-{step+1}"))
 
+            if self.control.should_training_stop:
+                break
+
     @torch.no_grad()
     def generate(
         self,
         inputs: Dict[str, torch.Tensor],
         length_sampler: Optional[Callable] = None,
         return_prompt: Optional[bool] = True,
         **generation_kwargs
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/ppo/utils.py` & `glmtuner-0.1.1/src/glmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/ppo/workflow.py` & `glmtuner-0.1.1/src/glmtuner/tuner/ppo/workflow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/sentiment/scripts/gpt-neox-20b_peft/gpt-neo-20b_sentiment_peft.py
 
-
 import math
 from trl import PPOConfig
 from torch.optim import AdamW
-from transformers import Seq2SeqTrainingArguments
+from typing import Optional, List
+from transformers import Seq2SeqTrainingArguments, TrainerCallback
 from transformers.optimization import get_scheduler
 
 from glmtuner.dsets import DataCollatorForChatGLM, get_dataset, preprocess_dataset
 from glmtuner.extras.callbacks import LogCallback
 from glmtuner.extras.ploting import plot_loss
 from glmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from glmtuner.tuner.core import load_model_and_tokenizer
 from glmtuner.tuner.ppo.trainer import PPOTrainerForChatGLM
 
 
 def run_ppo(
-        model_args: ModelArguments,
-        data_args: DataArguments,
-        training_args: Seq2SeqTrainingArguments,
-        finetuning_args: FinetuningArguments
+    model_args: ModelArguments,
+    data_args: DataArguments,
+    training_args: Seq2SeqTrainingArguments,
+    finetuning_args: FinetuningArguments,
+    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="ppo")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="ppo")
-    data_collator = DataCollatorForChatGLM(tokenizer, model.pretrained_model, use_v2=model_args.use_v2)
+    data_collator = DataCollatorForChatGLM(tokenizer, model.pretrained_model)
 
     ppo_config = PPOConfig(
         model_name=model_args.model_name_or_path,
         learning_rate=training_args.learning_rate,
         mini_batch_size=training_args.per_device_train_batch_size,
         batch_size=training_args.per_device_train_batch_size,
         gradient_accumulation_steps=training_args.gradient_accumulation_steps,
@@ -47,15 +48,15 @@
         num_training_steps=(training_args.num_train_epochs * math.ceil(len(dataset) / total_train_batch_size))
     )
 
     # Initialize our Trainer
     ppo_trainer = PPOTrainerForChatGLM(
         training_args=training_args,
         finetuning_args=finetuning_args,
-        callbacks=[LogCallback()],
+        callbacks=callbacks,
         config=ppo_config,
         model=model,
         ref_model=None,
         tokenizer=tokenizer,
         dataset=dataset,
         data_collator=data_collator,
         optimizer=optimizer,
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/rm/collator.py` & `glmtuner-0.1.1/src/glmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/rm/workflow.py` & `glmtuner-0.1.1/src/glmtuner/tuner/rm/workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Inspired by:
 # https://github.com/lvwerra/trl/blob/main/examples/summarization/scripts/reward_summarization.py
 # https://github.com/CarperAI/trlx/blob/main/examples/summarize_rlhf/reward_model/train_reward_model_gptj.py
 
-
-from transformers import Seq2SeqTrainingArguments
+from typing import Optional, List
+from transformers import Seq2SeqTrainingArguments, TrainerCallback
 
 from glmtuner.dsets import get_dataset, preprocess_dataset
 from glmtuner.extras.callbacks import LogCallback
 from glmtuner.extras.ploting import plot_loss
 from glmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments
 from glmtuner.tuner.core import load_model_and_tokenizer
 from glmtuner.tuner.rm.metric import compute_accuracy
@@ -15,20 +15,21 @@
 from glmtuner.tuner.rm.trainer import PairwiseTrainerForChatGLM
 
 
 def run_rm(
     model_args: ModelArguments,
     data_args: DataArguments,
     training_args: Seq2SeqTrainingArguments,
-    finetuning_args: FinetuningArguments
+    finetuning_args: FinetuningArguments,
+    callbacks: Optional[List[TrainerCallback]] = [LogCallback()]
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="rm")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="rm")
-    data_collator = PairwiseDataCollatorForChatGLM(tokenizer, model.pretrained_model, use_v2=model_args.use_v2)
+    data_collator = PairwiseDataCollatorForChatGLM(tokenizer, model.pretrained_model)
 
     training_args.remove_unused_columns = False # Important for pairwise dataset
 
     # Split the dataset
     if training_args.do_train:
         if data_args.dev_ratio > 1e-6:
             dataset = dataset.train_test_split(test_size=data_args.dev_ratio)
@@ -41,15 +42,15 @@
     # Initialize our Trainer
     trainer = PairwiseTrainerForChatGLM(
         finetuning_args=finetuning_args,
         model=model,
         args=training_args,
         tokenizer=tokenizer,
         data_collator=data_collator,
-        callbacks=[LogCallback()],
+        callbacks=callbacks,
         compute_metrics=compute_accuracy,
         **trainer_kwargs
     )
 
     # Training
     if training_args.do_train:
         train_result = trainer.train()
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/sft/metric.py` & `glmtuner-0.1.1/src/glmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/sft/trainer.py` & `glmtuner-0.1.1/src/glmtuner/tuner/sft/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,32 +27,30 @@
         ignore_keys: Optional[List[str]] = None,
     ) -> Tuple[Optional[float], Optional[torch.Tensor], Optional[torch.Tensor]]:
         r"""
         Removes the prompt part in the generated tokens.
 
         Subclass and override to inject custom behavior.
         """
-
         input_ids = inputs["input_ids"]
         loss, generated_tokens, labels = super().prediction_step(
             model, inputs, prediction_loss_only=prediction_loss_only, ignore_keys=ignore_keys
         )
         generated_tokens = generated_tokens[:, input_ids.size(-1):] if generated_tokens is not None else None
         return (loss, generated_tokens, labels)
 
     def save_predictions(
-            self,
-            predict_results: PredictionOutput
+        self,
+        predict_results: PredictionOutput
     ) -> None:
         r"""
         Saves model predictions to `output_dir`.
 
         A custom behavior that not contained in Seq2SeqTrainer.
         """
-
         if not self.is_world_process_zero():
             return
 
         output_prediction_file = os.path.join(self.args.output_dir, "generated_predictions.jsonl")
         logger.info(f"Saving prediction results to {output_prediction_file}")
 
         preds = np.where(predict_results.predictions != IGNORE_INDEX, predict_results.predictions, self.tokenizer.pad_token_id)
```

### Comparing `glmtuner-0.1.0/src/glmtuner/tuner/sft/workflow.py` & `glmtuner-0.1.1/src/glmtuner/tuner/sft/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 ):
     dataset = get_dataset(model_args, data_args)
     model, tokenizer = load_model_and_tokenizer(model_args, finetuning_args, training_args.do_train, stage="sft")
     dataset = preprocess_dataset(dataset, tokenizer, data_args, training_args, stage="sft")
     data_collator = DataCollatorForChatGLM(
         tokenizer=tokenizer,
         model=model,
-        ignore_pad_token_for_loss=(data_args.ignore_pad_token_for_loss and not training_args.predict_with_generate),
-        use_v2=model_args.use_v2
+        ignore_pad_token_for_loss=(data_args.ignore_pad_token_for_loss and not training_args.predict_with_generate)
     )
 
     # Override the decoding parameters of Seq2SeqTrainer
     training_args.generation_max_length = training_args.generation_max_length if \
                 training_args.generation_max_length is not None else data_args.max_target_length
     training_args.generation_num_beams = data_args.eval_num_beams if \
                 data_args.eval_num_beams is not None else training_args.generation_num_beams
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/common.py` & `glmtuner-0.1.1/src/glmtuner/webui/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,46 @@
-import os
 import json
+import os
+from typing import Dict, List, Tuple
+
 import gradio as gr
-from typing import List, Tuple
-from transformers.trainer import WEIGHTS_NAME, WEIGHTS_INDEX_NAME
 from peft.utils import WEIGHTS_NAME as PEFT_WEIGHTS_NAME
+from transformers.trainer import WEIGHTS_NAME, WEIGHTS_INDEX_NAME
 
-
-CACHE_DIR = "cache" # to save models
+CACHE_DIR = "cache"
 DATA_DIR = "data"
 SAVE_DIR = "saves"
+USER_CONFIG = "user.config"
+
+
+def get_config_path():
+    return os.path.join(CACHE_DIR, USER_CONFIG)
+
+
+def load_config() -> Dict[str, str]:
+    if not os.path.exists(get_config_path()):
+        return {}
+
+    with open(get_config_path(), "r", encoding="utf-8") as f:
+        try:
+            user_config = json.load(f)
+            return user_config
+        except:
+            return {}
+
+
+def save_config(model_name: str, model_path: str) -> None:
+    os.makedirs(CACHE_DIR, exist_ok=True)
+    user_config = dict(model_name=model_name, model_path=model_path)
+    with open(get_config_path(), "w", encoding="utf-8") as f:
+        json.dump(user_config, f, ensure_ascii=False)
 
 
 def get_save_dir(model_name: str) -> str:
-    return os.path.join(SAVE_DIR, model_name)
+    return os.path.join(SAVE_DIR, os.path.split(model_name)[-1])
 
 
 def add_model(model_list: list, model_name: str, model_path: str) -> Tuple[list, str, str]:
     model_list = model_list + [[model_name, model_path]]
     return model_list, "", ""
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/components/data.py` & `glmtuner-0.1.1/src/glmtuner/webui/components/data.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import gradio as gr
-from typing import Tuple
 from gradio.components import Component
+from typing import Tuple
 
 
 def create_preview_box() -> Tuple[Component, Component, Component]:
     with gr.Box(visible=False, elem_classes="modal-box") as preview_box:
         with gr.Row():
             preview_count = gr.Number(label="Count", interactive=False)
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/components/infer.py` & `glmtuner-0.1.1/src/glmtuner/webui/components/infer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,71 @@
-import gradio as gr
 from typing import Tuple
+
+import gradio as gr
 from gradio.components import Component
 
-from glmtuner.webui.chat import ChatModel
+from glmtuner.webui.chat import WebChatModel
 
 
-def create_chat_box(chat_model: ChatModel) -> Tuple[Component, Component, Component]:
+def create_chat_box(chat_model: WebChatModel) -> Tuple[Component, Component, Component]:
     with gr.Box(visible=False) as chat_box:
         chatbot = gr.Chatbot()
 
         with gr.Row():
             with gr.Column(scale=4):
                 with gr.Column(scale=12):
                     query = gr.Textbox(show_label=False, placeholder="Input...", lines=10)
 
                 with gr.Column(min_width=32, scale=1):
-                    submit = gr.Button("Submit", variant="primary")
+                    submit_btn = gr.Button("Submit", variant="primary")
 
             with gr.Column(scale=1):
-                clear = gr.Button("Clear History")
+                clear_btn = gr.Button("Clear History")
                 max_length = gr.Slider(
-                    10, 2048, value=chat_model.gen_args.max_length, step=1.0, label="Maximum length", interactive=True
+                    10, 2048, value=chat_model.generating_args.max_length, step=1.0,
+                    label="Maximum length", interactive=True
                 )
                 top_p = gr.Slider(
-                    0, 1, value=chat_model.gen_args.top_p, step=0.01, label="Top P", interactive=True
+                    0, 1, value=chat_model.generating_args.top_p, step=0.01,
+                    label="Top P", interactive=True
                 )
                 temperature = gr.Slider(
-                    0, 1.5, value=chat_model.gen_args.temperature, step=0.01, label="Temperature", interactive=True
+                    0, 1.5, value=chat_model.generating_args.temperature, step=0.01,
+                    label="Temperature", interactive=True
                 )
 
     history = gr.State([])
 
-    submit.click(
+    submit_btn.click(
         chat_model.predict,
         [chatbot, query, history, max_length, top_p, temperature],
         [chatbot, history],
         show_progress=True
     ).then(
         lambda: gr.update(value=""), outputs=[query]
     )
 
-    clear.click(lambda: ([], []), outputs=[chatbot, history], show_progress=True)
+    clear_btn.click(lambda: ([], []), outputs=[chatbot, history], show_progress=True)
 
     return chat_box, chatbot, history
 
 
-def create_infer_tab(base_model: Component, model_list: Component, checkpoints: Component) -> None:
+def create_infer_tab(model_name: Component, model_path: Component, checkpoints: Component) -> None:
     info_box = gr.Markdown(value="Model unloaded, please load a model first.")
 
-    chat_model = ChatModel()
+    chat_model = WebChatModel()
     chat_box, chatbot, history = create_chat_box(chat_model)
 
     with gr.Row():
         load_btn = gr.Button("Load model")
         unload_btn = gr.Button("Unload model")
-        use_v2 = gr.Checkbox(label="use ChatGLM2", value=True)
+        quantization_bit = gr.Dropdown([8, 4], label="Quantization bit", info="Quantize model to 4/8-bit mode.")
 
     load_btn.click(
-        chat_model.load_model, [base_model, model_list, checkpoints, use_v2], [info_box]
+        chat_model.load_model, [model_name, model_path, checkpoints, quantization_bit], [info_box]
     ).then(
         lambda: gr.update(visible=(chat_model.model is not None)), outputs=[chat_box]
     )
 
     unload_btn.click(
         chat_model.unload_model, outputs=[info_box]
     ).then(
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/components/sft.py` & `glmtuner-0.1.1/src/glmtuner/webui/components/sft.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import gradio as gr
 from gradio.components import Component
 from transformers.trainer_utils import SchedulerType
 
-from glmtuner.webui.components.data import create_preview_box
 from glmtuner.webui.common import list_datasets
+from glmtuner.webui.components.data import create_preview_box
 from glmtuner.webui.runner import Runner
 from glmtuner.webui.utils import can_preview, get_preview, get_time, gen_plot
 
 
-def create_sft_tab(base_model: Component, model_list: Component, checkpoints: Component, runner: Runner) -> None:
+def create_sft_tab(model_name: Component, model_path: Component, checkpoints: Component, runner: Runner) -> None:
     with gr.Row():
         finetuning_type = gr.Dropdown(
-            label="Finetuning method", value="lora", choices=["full", "freeze", "p_tuning", "lora"], interactive=True
+            label="Finetuning method", value="lora",
+            choices=["full", "freeze", "p_tuning", "lora"], interactive=True, scale=2
         )
-
-    with gr.Row():
-        dataset = gr.Dropdown(label="Dataset", choices=list_datasets(), multiselect=True, interactive=True, scale=4)
-        preview = gr.Button("Preview", visible=False, scale=1)
+        dataset = gr.Dropdown(label="Dataset", choices=list_datasets(), multiselect=True, interactive=True, scale=2)
+        preview_btn = gr.Button("Preview", interactive=False, scale=1)
 
     preview_box, preview_count, preview_samples = create_preview_box()
 
-    dataset.change(can_preview, [dataset], [preview])
-    preview.click(
+    dataset.change(can_preview, [dataset], [preview_btn])
+    preview_btn.click(
         get_preview, [dataset], [preview_count, preview_samples]
     ).then(
         lambda: gr.update(visible=True), outputs=[preview_box]
     )
 
     with gr.Row():
         learning_rate = gr.Textbox(
@@ -33,57 +32,59 @@
         )
         num_train_epochs = gr.Textbox(
             label="Epochs", value="3.0", info="Total number of training epochs to perform.", interactive=True
         )
         max_samples = gr.Textbox(
             label="Max samples", value="100000", info="Number of samples for training.", interactive=True
         )
-        use_v2 = gr.Checkbox(label="use ChatGLM2", value=True)
+        quantization_bit = gr.Dropdown([8, 4], label="Quantization bit", info="Quantize model to 4/8-bit mode.")
 
     with gr.Row():
         per_device_train_batch_size = gr.Slider(
-            label="Batch size", value=4, minimum=1, maximum=128, step=1, info="Train batch size.", interactive=True
+            label="Batch size", value=4, minimum=1, maximum=128, step=1,
+            info="Train batch size.", interactive=True
         )
         gradient_accumulation_steps = gr.Slider(
-            label="Gradient accumulation", value=4, minimum=1, maximum=16, step=1, info='Accumulation steps.', interactive=True
+            label="Gradient accumulation", value=4, minimum=1, maximum=32, step=1,
+            info="Accumulation steps.", interactive=True
         )
         lr_scheduler_type = gr.Dropdown(
             label="LR Scheduler", value="cosine", info="Scheduler type.",
             choices=[scheduler.value for scheduler in SchedulerType], interactive=True
         )
         fp16 = gr.Checkbox(label="fp16", value=True)
 
     with gr.Row():
         logging_steps = gr.Slider(
-            label="Logging steps", value=1, minimum=1, maximum=1000, step=10,
+            label="Logging steps", value=5, minimum=5, maximum=1000, step=5,
             info="Number of update steps between two logs.", interactive=True
         )
         save_steps = gr.Slider(
             label="Save steps", value=100, minimum=10, maximum=2000, step=10,
             info="Number of updates steps before two checkpoint saves.", interactive=True
         )
 
     with gr.Row():
-        start = gr.Button("Start training")
-        stop = gr.Button("Abort")
+        start_btn = gr.Button("Start training")
+        stop_btn = gr.Button("Abort")
 
     with gr.Row():
         with gr.Column(scale=4):
             output_dir = gr.Textbox(label="Checkpoint name", value=get_time(), interactive=True)
             output_info = gr.Markdown(value="Ready")
 
         with gr.Column(scale=1):
             loss_viewer = gr.Plot(label="Loss")
 
-    start.click(
+    start_btn.click(
         runner.run_train,
         [
-            base_model, model_list, checkpoints, output_dir, finetuning_type,
+            model_name, model_path, checkpoints, output_dir, finetuning_type,
             dataset, learning_rate, num_train_epochs, max_samples,
-            fp16, use_v2, per_device_train_batch_size, gradient_accumulation_steps,
+            fp16, quantization_bit, per_device_train_batch_size, gradient_accumulation_steps,
             lr_scheduler_type, logging_steps, save_steps
         ],
         output_info
     )
-    stop.click(runner.set_abort, queue=False)
+    stop_btn.click(runner.set_abort, queue=False)
 
-    output_info.change(gen_plot, [base_model, output_dir], loss_viewer, queue=False)
+    output_info.change(gen_plot, [model_name, output_dir], loss_viewer, queue=False)
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/interface.py` & `glmtuner-0.1.1/src/glmtuner/webui/interface.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import gradio as gr
 from transformers.utils.versions import require_version
 
-from glmtuner.webui.css import CSS
-from glmtuner.webui.runner import Runner
 from glmtuner.webui.components import (
     create_model_tab,
     create_sft_tab,
     create_eval_tab,
     create_infer_tab
 )
+from glmtuner.webui.css import CSS
+from glmtuner.webui.runner import Runner
 
 
 require_version("gradio>=3.36.0", "To fix: pip install gradio>=3.36.0")
 
 
 def create_ui() -> gr.Blocks:
     runner = Runner()
 
     with gr.Blocks(title="Web Tuner", css=CSS) as demo:
-        base_model, model_list, checkpoints = create_model_tab()
+        model_name, model_path, checkpoints = create_model_tab()
 
         with gr.Tab("SFT"):
-            create_sft_tab(base_model, model_list, checkpoints, runner)
+            create_sft_tab(model_name, model_path, checkpoints, runner)
 
         with gr.Tab("Evaluate"):
-            create_eval_tab(base_model, model_list, checkpoints, runner)
+            create_eval_tab(model_name, model_path, checkpoints, runner)
 
         with gr.Tab("Inference"):
-            create_infer_tab(base_model, model_list, checkpoints)
+            create_infer_tab(model_name, model_path, checkpoints)
 
     return demo
 
 
 if __name__ == "__main__":
     demo = create_ui()
     demo.queue()
-    demo.launch(server_name="0.0.0.0", share=True, inbrowser=True)
+    demo.launch(server_name="0.0.0.0", share=False, inbrowser=True)
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/runner.py` & `glmtuner-0.1.1/src/glmtuner/webui/runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import os
-import time
 import logging
+import os
 import threading
+import time
 import transformers
 from typing import Optional, Tuple
 
-from glmtuner.extras.misc import torch_gc
 from glmtuner.extras.callbacks import LogCallback
+from glmtuner.extras.constants import SUPPORTED_MODELS
 from glmtuner.extras.logging import LoggerHandler
+from glmtuner.extras.misc import torch_gc
 from glmtuner.tuner import get_train_args, run_sft
 from glmtuner.webui.common import get_save_dir, DATA_DIR
 from glmtuner.webui.utils import format_info, get_eval_results
 
 
 class Runner:
 
@@ -19,82 +20,87 @@
         self.aborted = False
         self.running = False
 
     def set_abort(self):
         self.aborted = True
         self.running = False
 
-    def initialize(self, base_model: str, model_list: list, dataset: list) -> Tuple[str, LoggerHandler, LogCallback]:
+    def initialize(self, model_name: str, model_path: str, dataset: list) -> Tuple[str, str, LoggerHandler, LogCallback]:
         if self.running:
-            return "A process is in running, please abort it firstly.", None, None
+            return None, "A process is in running, please abort it firstly.", None, None
 
-        if not base_model:
-            return "Please select a model.", None, None
+        if not model_name:
+            return None, "Please select a model.", None, None
 
-        if len(model_list) == 0:
-            return "No model detected.", None, None
+        if model_path:
+            if not os.path.isdir(model_path):
+                return None, "Cannot find model directory in local disk.", None, None
+            model_name_or_path = model_path
+        elif model_name in SUPPORTED_MODELS: # TODO: use list in gr.State
+            model_name_or_path = SUPPORTED_MODELS[model_name]["hf_path"]
+        else:
+            return None, "Invalid model.", None, None
 
         if len(dataset) == 0:
-            return "Please choose datasets.", None, None
+            return None, "Please choose datasets.", None, None
 
         self.aborted = False
         self.running = True
 
         logger_handler = LoggerHandler()
         logger_handler.setLevel(logging.INFO)
         logging.root.addHandler(logger_handler)
         transformers.logging.add_handler(logger_handler)
         trainer_callback = LogCallback(self)
 
-        return "", logger_handler, trainer_callback
+        return model_name_or_path, "", logger_handler, trainer_callback
 
     def finalize(self, finish_info: Optional[str] = None) -> str:
         self.running = False
         torch_gc()
         if self.aborted:
             return "Ready"
         else:
             return finish_info if finish_info is not None else "Finished"
 
     def run_train(
-        self, base_model, model_list, checkpoints, output_dir, finetuning_type,
+        self, model_name, model_path, checkpoints, output_dir, finetuning_type,
         dataset, learning_rate, num_train_epochs, max_samples,
-        fp16, use_v2, per_device_train_batch_size, gradient_accumulation_steps,
+        fp16, quantization_bit, per_device_train_batch_size, gradient_accumulation_steps,
         lr_scheduler_type, logging_steps, save_steps
     ):
-        error, logger_handler, trainer_callback = self.initialize(base_model, model_list, dataset)
+        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(model_name, model_path, dataset)
         if error:
             yield error
             return
 
-        model_path = [path for name, path in model_list if name == base_model]
-        if get_save_dir(base_model) and checkpoints:
-            checkpoint_dir = ",".join([os.path.join(get_save_dir(base_model), checkpoint) for checkpoint in checkpoints])
+        if checkpoints:
+            checkpoint_dir = ",".join([os.path.join(get_save_dir(model_name), checkpoint) for checkpoint in checkpoints])
         else:
             checkpoint_dir = None
 
         args = dict(
-            model_name_or_path=model_path[0],
+            model_name_or_path=model_name_or_path,
             do_train=True,
             finetuning_type=finetuning_type,
             dataset=",".join(dataset),
             dataset_dir=DATA_DIR,
             max_samples=int(max_samples),
-            output_dir=os.path.join(get_save_dir(base_model), output_dir),
+            output_dir=os.path.join(get_save_dir(model_name), output_dir),
             checkpoint_dir=checkpoint_dir,
             overwrite_cache=True,
             per_device_train_batch_size=per_device_train_batch_size,
             gradient_accumulation_steps=gradient_accumulation_steps,
             lr_scheduler_type=lr_scheduler_type,
             logging_steps=logging_steps,
             save_steps=save_steps,
             learning_rate=float(learning_rate),
             num_train_epochs=float(num_train_epochs),
             fp16=fp16,
-            use_v2=use_v2
+            quantization_bit=int(quantization_bit) if quantization_bit else None
         )
         model_args, data_args, training_args, finetuning_args, _ = get_train_args(args)
 
         run_args = dict(
             model_args=model_args,
             data_args=data_args,
             training_args=training_args,
@@ -110,41 +116,41 @@
                 yield "Aborted, wait for terminating..."
             else:
                 yield format_info(logger_handler.log, trainer_callback.tracker)
 
         yield self.finalize()
 
     def run_eval(
-        self, base_model, model_list, checkpoints, dataset, max_samples, per_device_eval_batch_size, use_v2
+        self, model_name, model_path, checkpoints, dataset, max_samples, per_device_eval_batch_size,
+        quantization_bit
     ):
-        error, logger_handler, trainer_callback = self.initialize(base_model, model_list, dataset)
+        model_name_or_path, error, logger_handler, trainer_callback = self.initialize(model_name, model_path, dataset)
         if error:
             yield error
             return
 
-        model_path = [path for name, path in model_list if name == base_model]
-        if get_save_dir(base_model) and checkpoints:
-            checkpoint_dir = ",".join([os.path.join(get_save_dir(base_model), checkpoint) for checkpoint in checkpoints])
-            output_dir = os.path.join(get_save_dir(base_model), "eval_" + "_".join(checkpoints))
+        if checkpoints:
+            checkpoint_dir = ",".join([os.path.join(get_save_dir(model_name), checkpoint) for checkpoint in checkpoints])
+            output_dir = os.path.join(get_save_dir(model_name), "eval_" + "_".join(checkpoints))
         else:
             checkpoint_dir = None
-            output_dir = os.path.join(get_save_dir(base_model), "eval_base")
+            output_dir = os.path.join(get_save_dir(model_name), "eval_base")
 
         args = dict(
-            model_name_or_path=model_path[0],
+            model_name_or_path=model_name_or_path,
             do_eval=True,
             dataset=",".join(dataset),
             dataset_dir=DATA_DIR,
             max_samples=int(max_samples),
             output_dir=output_dir,
             checkpoint_dir=checkpoint_dir,
             overwrite_cache=True,
             predict_with_generate=True,
             per_device_eval_batch_size=per_device_eval_batch_size,
-            use_v2=use_v2
+            quantization_bit=int(quantization_bit) if quantization_bit else None
         )
         model_args, data_args, training_args, finetuning_args, _ = get_train_args(args)
 
         run_args = dict(
             model_args=model_args,
             data_args=data_args,
             training_args=training_args,
```

### Comparing `glmtuner-0.1.0/src/glmtuner/webui/utils.py` & `glmtuner-0.1.1/src/glmtuner/webui/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import os
 import json
+import os
+from datetime import datetime
+from typing import Tuple
+
 import gradio as gr
 import matplotlib.figure
 import matplotlib.pyplot as plt
-from typing import Tuple
-from datetime import datetime
 
 from glmtuner.extras.ploting import smooth
 from glmtuner.webui.common import get_save_dir, DATA_DIR
 
 
 def format_info(log: str, tracker: dict) -> str:
     info = log
@@ -27,17 +28,17 @@
     with open(os.path.join(DATA_DIR, "dataset_info.json"), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
     if (
         len(dataset) > 0
         and "file_name" in dataset_info[dataset[0]]
         and os.path.isfile(os.path.join(DATA_DIR, dataset_info[dataset[0]]["file_name"]))
     ):
-        return gr.update(visible=True)
+        return gr.update(interactive=True)
     else:
-        return gr.update(visible=False)
+        return gr.update(interactive=False)
 
 
 def get_preview(dataset: list) -> Tuple[int, list]:
     with open(os.path.join(DATA_DIR, "dataset_info.json"), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
     data_file = dataset_info[dataset[0]]["file_name"]
     with open(os.path.join(DATA_DIR, data_file), "r", encoding="utf-8") as f:
@@ -59,15 +60,16 @@
     plt.close("all")
     fig = plt.figure()
     ax = fig.add_subplot(111)
     steps, losses = [], []
     with open(log_file, "r", encoding="utf-8") as f:
         for line in f:
             log_info = json.loads(line)
-            steps.append(log_info["current_steps"])
-            losses.append(log_info["loss"])
+            if log_info.get("loss", None):
+                steps.append(log_info["current_steps"])
+                losses.append(log_info["loss"])
     ax.plot(steps, losses, alpha=0.4, label="original")
     ax.plot(steps, smooth(losses), label="smoothed")
     ax.legend()
     ax.set_xlabel("step")
     ax.set_ylabel("loss")
     return fig
```

### Comparing `glmtuner-0.1.0/src/glmtuner.egg-info/PKG-INFO` & `glmtuner-0.1.1/src/glmtuner.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glmtuner
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fine-tuning ChatGLM-6B with PEFT
 Home-page: https://github.com/hiyouga/ChatGLM-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: ChatGLM,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -16,35 +16,39 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # ChatGLM Efficient Tuning
 
-![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)
-![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)
-![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)
+[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/ChatGLM-Efficient-Tuning?style=social)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/stargazers)
+[![GitHub Code License](https://img.shields.io/github/license/hiyouga/ChatGLM-Efficient-Tuning)](LICENSE)
+[![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/ChatGLM-Efficient-Tuning)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/commits/main)
+[![PyPI](https://img.shields.io/pypi/v/glmtuner)](https://pypi.org/project/glmtuner/)
+[![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/ChatGLM-Efficient-Tuning/pulls)
 
 Fine-tuning 🤖[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) model with 🤗[PEFT](https://github.com/huggingface/peft).
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
 \[ English | [中文](README_zh.md) \]
 
 ## Changelog
 
+[23/07/15] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune ChatGLM-6B model in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) for his efforts in the development.
+
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
 [23/06/25] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in arbitrary ChatGPT-based applications.
 
-[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework! Try `--use_v2` argument to fine-tune and predict that model.
+[23/06/25] Now we support fine-tuning the [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B) model with our framework!
 
 [23/06/05] Now we support 4-bit LoRA training (aka [QLoRA](https://github.com/artidoro/qlora)). Try `--quantization_bit 4` argument to work with 4-bit quantized model. (experimental feature)
 
 [23/06/01] We implemented a framework supporting the efficient tuning of LLaMA and BLOOM models. Please follow [LLaMA-Efficient-Tuning](https://github.com/hiyouga/LLaMA-Efficient-Tuning) if you are interested.
 
 [23/05/19] Now we support using the development set to evaluate the model while training. Try `--dev_ratio` argument to specify the size of development set.
 
@@ -139,14 +143,15 @@
 ```
 
 ### Fine-tuning with a Single GPU
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -167,14 +172,15 @@
 ```
 
 ### Training Reward Model
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset comparison_gpt4_en \
     --finetuning_type lora \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
@@ -186,14 +192,15 @@
 ```
 
 ### Training with RLHF
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_train \
     --dataset alpaca_gpt4_en \
     --finetuning_type lora \
     --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
@@ -208,53 +215,57 @@
 ```
 
 ### Evaluation (BLEU and ROUGE_CHINESE)
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
 ### Predict
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
+    --model_name_or_path path_to_your_chatglm_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 50 \
     --predict_with_generate
 ```
 
-### CLI Demo
+### API / CLI Demo
 
 ```bash
-python src/cli_demo.py \
+python src/xxx_demo.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### All-in-one Web UI
 
 ```bash
 python src/train_web.py
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
+    --model_name_or_path path_to_your_chatglm_model \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
 ### Hardware Requirements
 
 | Fine-tune method | Batch size | Mode |  GRAM  | Speed |
```

### Comparing `glmtuner-0.1.0/src/glmtuner.egg-info/SOURCES.txt` & `glmtuner-0.1.1/src/glmtuner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 src/glmtuner/__init__.py
 src/glmtuner.egg-info/PKG-INFO
 src/glmtuner.egg-info/SOURCES.txt
 src/glmtuner.egg-info/dependency_links.txt
 src/glmtuner.egg-info/requires.txt
 src/glmtuner.egg-info/top_level.txt
 src/glmtuner/api/__init__.py
 src/glmtuner/api/app.py
 src/glmtuner/api/protocol.py
+src/glmtuner/chat/__init__.py
+src/glmtuner/chat/stream_chat.py
 src/glmtuner/dsets/__init__.py
 src/glmtuner/dsets/collator.py
 src/glmtuner/dsets/loader.py
 src/glmtuner/dsets/preprocess.py
 src/glmtuner/extras/__init__.py
 src/glmtuner/extras/callbacks.py
 src/glmtuner/extras/constants.py
```

