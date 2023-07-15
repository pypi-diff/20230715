# Comparing `tmp/alpaca_eval-0.2.2.tar.gz` & `tmp/alpaca_eval-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.2.tar", last modified: Thu Jul 13 13:08:58 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.3.tar", last modified: Sat Jul 15 16:24:00 2023, max compression
```

## Comparing `alpaca_eval-0.2.2.tar` & `alpaca_eval-0.2.3.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65548 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.437964 alpaca_eval-0.2.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.425964 alpaca_eval-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.441964 alpaca_eval-0.2.2/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-13 13:08:38.000000 alpaca_eval-0.2.2/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23087 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15292 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.445964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.449964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_2/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.453964 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.429964 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.437964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.457965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude-2/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/claude-2/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.461964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.465964 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.469965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.441964 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 13:08:58.000000 alpaca_eval-0.2.2/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 13:08:58.473965 alpaca_eval-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-13 13:08:20.000000 alpaca_eval-0.2.2/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65813 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.410025 alpaca_eval-0.2.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.402025 alpaca_eval-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-15 16:23:45.000000 alpaca_eval-0.2.3/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25039 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.418026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.422026 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.406025 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21848 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.410025 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude-2/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/claude-2/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.426027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.430027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.414026 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    66635 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 16:24:00.000000 alpaca_eval-0.2.3/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 16:24:00.434027 alpaca_eval-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-15 16:23:33.000000 alpaca_eval-0.2.3/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.2/LICENSE` & `alpaca_eval-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/PKG-INFO` & `alpaca_eval-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.2
+Version: 0.2.3
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -17,36 +17,36 @@
 Provides-Extra: analysis
 Provides-Extra: dev
 Provides-Extra: local
 Provides-Extra: api
 Provides-Extra: all
 License-File: LICENSE
 
-# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
+# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
-Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
+Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations) like the preference for longer outputs.
 AlpacaEval provides the following:
 
+- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
+  evaluation set. **Caution**: Automatic evaluator (e.g. GPT4) may be biased towards models that generate longer outputs and/or that were fine-tuned on the model underlying the evaluator (e.g. GPT4).
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
   measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
   over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
-- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-  evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
   on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
   evaluation set. 2.5K of these are cross-annotations (4 humans annotating the same 650 examples).
 - [**AlpacaEval dataset**](#data-release): a simplification
```

#### html2text {}

```diff
@@ -1,51 +1,55 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.2 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.3 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
 Extra: api Provides-Extra: all License-File: LICENSE # [https://
 raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
-AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
-[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
-License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
-[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
-www.python.org/downloads/release/python-3100/) [![discord](https://
-img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
-/discord.gg/GJMxJSVZZM) Evaluation of instruction-following models (e.g.,
-ChatGPT) typically requires human interactions. This is time-consuming,
-expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
-evaluation that is fast, cheap, replicable, and validated against 20K human
-annotations. It is particularly useful for model development. Although we
-improved over prior automatic evaluation pipelines, there are still fundamental
-[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
-evaluator**](#evaluators): an automatic evaluator that has high agreement with
-humans (validated on 20K annotations). We evaluate a model by measuring the
-fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the
-outputs from that model over outputs from a reference model. Our evaluators
-enable caching and output randomization by default. - [**Leaderboard**](https:/
-/tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the
-AlpacaEval evaluation set. - [**Toolkit for building automatic evaluators**]
-(#analysis): a simple interface for building advanced automatic evaluators
-(e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
-price, speed, statistical power, bias, variance etc). - [**Human evaluation
-data**](#data-release): 20K human preferences between a given and reference
-model on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
-evaluation set. 2.5K of these are cross-annotations (4 humans annotating the
-same 650 examples). - [**AlpacaEval dataset**](#data-release): a simplification
-of [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main)
-evaluation set, where "instructions" and " inputs" are merged into one field,
-and reference outputs are longer. **When to use AlpacaEval?** Our automatic
+[AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) : An Automatic Evaluator
+for Instruction-following Language Models [![Code License](https://
+img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/
+tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data License](https://
+img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://
+github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+]
+(https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/
+downloads/release/python-3100/) [![discord](https://img.shields.io/badge/
+discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/
+GJMxJSVZZM) Evaluation of instruction-following models (e.g., ChatGPT)
+typically requires human interactions. This is time-consuming, expensive, and
+hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is
+fast, cheap, replicable, and validated against 20K human annotations. It is
+particularly useful for model development. Although we improved over prior
+automatic evaluation pipelines, there are still fundamental [limitations]
+(#limitations) like the preference for longer outputs. AlpacaEval provides the
+following: - [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a
+leaderboard of common models on the AlpacaEval evaluation set. **Caution**:
+Automatic evaluator (e.g. GPT4) may be biased towards models that generate
+longer outputs and/or that were fine-tuned on the model underlying the
+evaluator (e.g. GPT4). - [**Automatic evaluator**](#evaluators): an automatic
+evaluator that has high agreement with humans (validated on 20K annotations).
+We evaluate a model by measuring the fraction of times an powerful LLM (e.g.
+GPT 4 or Claude or ChatGPT) prefers the outputs from that model over outputs
+from a reference model. Our evaluators enable caching and output randomization
+by default. - [**Toolkit for building automatic evaluators**](#analysis): a
+simple interface for building advanced automatic evaluators (e.g. with caching,
+batching, or multi-annotators) and analyzing them (quality, price, speed,
+statistical power, bias, variance etc). - [**Human evaluation data**](#data-
+release): 20K human preferences between a given and reference model on the
+[AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
+set. 2.5K of these are cross-annotations (4 humans annotating the same 650
+examples). - [**AlpacaEval dataset**](#data-release): a simplification of
+[AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
+set, where "instructions" and " inputs" are merged into one field, and
+reference outputs are longer. **When to use AlpacaEval?** Our automatic
 evaluator is a quick and cheap proxy for human evaluation of simple
 instruction-following tasks. It is useful if you have to run many evaluations
 quickly, e.g., during model development. **When not to use AlpacaEval?** As any
 other automatic evaluator, AlpacaEval should **not replace human evaluation in
 high-stake decision-making**, e.g., to decide on model release. In particular,
 AlpacaEval is limited by the fact that (1) the instructions in the eval set
 might not be representative of advanced usage of LLMs; (2) automatic evaluators
```

### Comparing `alpaca_eval-0.2.2/README.md` & `alpaca_eval-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
+# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
-Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
+Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations) like the preference for longer outputs.
 AlpacaEval provides the following:
 
+- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
+  evaluation set. **Caution**: Automatic evaluator (e.g. GPT4) may be biased towards models that generate longer outputs and/or that were fine-tuned on the model underlying the evaluator (e.g. GPT4).
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
   measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
   over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
-- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-  evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
   on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
   evaluation set. 2.5K of these are cross-annotations (4 humans annotating the same 650 examples).
 - [**AlpacaEval dataset**](#data-release): a simplification
```

#### html2text {}

```diff
@@ -1,31 +1,34 @@
 # [https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/
-AlpacaFarm_small.png] AlpacaEval : An Automatic Evaluator for Instruction-
-following Language Models [![Code License](https://img.shields.io/badge/
-Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/
-blob/main/LICENSE) [![Data License](https://img.shields.io/badge/
-Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/
-alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+](https://img.shields.io/
-badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-
-3100/) [![discord](https://img.shields.io/badge/discord-server-
-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM) Evaluation
-of instruction-following models (e.g., ChatGPT) typically requires human
-interactions. This is time-consuming, expensive, and hard to replicate.
-AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
-replicable, and validated against 20K human annotations. It is particularly
-useful for model development. Although we improved over prior automatic
-evaluation pipelines, there are still fundamental [limitations](#limitations).
-AlpacaEval provides the following: - [**Automatic evaluator**](#evaluators): an
-automatic evaluator that has high agreement with humans (validated on 20K
-annotations). We evaluate a model by measuring the fraction of times an
-powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that
-model over outputs from a reference model. Our evaluators enable caching and
-output randomization by default. - [**Leaderboard**](https://tatsu-
-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-evaluation set. - [**Toolkit for building automatic evaluators**](#analysis): a
+AlpacaFarm_small.png] [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) :
+An Automatic Evaluator for Instruction-following Language Models [![Code
+License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)]
+(https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data License]
+(https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)]
+(https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [![Python
+3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
+www.python.org/downloads/release/python-3100/) [![discord](https://
+img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
+/discord.gg/GJMxJSVZZM) Evaluation of instruction-following models (e.g.,
+ChatGPT) typically requires human interactions. This is time-consuming,
+expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
+evaluation that is fast, cheap, replicable, and validated against 20K human
+annotations. It is particularly useful for model development. Although we
+improved over prior automatic evaluation pipelines, there are still fundamental
+[limitations](#limitations) like the preference for longer outputs. AlpacaEval
+provides the following: - [**Leaderboard**](https://tatsu-lab.github.io/
+alpaca_eval/): a leaderboard of common models on the AlpacaEval evaluation set.
+**Caution**: Automatic evaluator (e.g. GPT4) may be biased towards models that
+generate longer outputs and/or that were fine-tuned on the model underlying the
+evaluator (e.g. GPT4). - [**Automatic evaluator**](#evaluators): an automatic
+evaluator that has high agreement with humans (validated on 20K annotations).
+We evaluate a model by measuring the fraction of times an powerful LLM (e.g.
+GPT 4 or Claude or ChatGPT) prefers the outputs from that model over outputs
+from a reference model. Our evaluators enable caching and output randomization
+by default. - [**Toolkit for building automatic evaluators**](#analysis): a
 simple interface for building advanced automatic evaluators (e.g. with caching,
 batching, or multi-annotators) and analyzing them (quality, price, speed,
 statistical power, bias, variance etc). - [**Human evaluation data**](#data-
 release): 20K human preferences between a given and reference model on the
 [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
 set. 2.5K of these are cross-annotations (4 humans annotating the same 650
 examples). - [**AlpacaEval dataset**](#data-release): a simplification of
```

### Comparing `alpaca_eval-0.2.2/example/outputs.json` & `alpaca_eval-0.2.3/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/setup.py` & `alpaca_eval-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.3/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/annotators/base.py` & `alpaca_eval-0.2.3/src/alpaca_eval/annotators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     Parameters
     ----------
     annotators_config : Path or list of dict, optional
         A dictionary or path to a yaml file containing the configuration for the pool of annotators. If a directory,
         we search for 'configs.yaml' in it. The keys in the first  dictionary should be the annotator's name, and
         the value should be a dictionary of the annotator's configuration which should have the following keys:
-        The path is relative to `evaluators_configs/` directory.
+        The path is relative to `base_dir` directory.
         - prompt_template (str): a prompt template or path to it. The template should contain placeholders for keys in
             the example dictionary, typically {instruction} and {output_1} {output_2}.
         - fn_completions (str): function in `alpaca_farm.decoders` for completions. Needs to accept as first argument
             `prompts` which is a list of string.
         - completions_kwargs (dict): kwargs for fn_completions. E.g. model_name, max_tokens, temperature,
         tokens_to_avoid
         - fn_completion_parser (str) : Function in `completion_parsers.py` to use for parsing the completions into
@@ -41,52 +41,64 @@
     seed : int, optional
         Seed for the random number generator.
 
     is_avoid_reannotations : bool, optional
         Whether to avoid re-annotating examples that have already been annotated by the annotator. This will decrease
         cost but can be slightly slower if there are no annotations that can be reused.
 
-    input_keys : tuple of str, optional
-        Keys use to distinguish inputs.
+    primary_keys : sequence of str, optional
+        Keys use to distinguish the example.
 
-    output_keys : tuple of str, optional
-        Keys use to distinguish outputs.
-
-    other_keys_to_keep : tuple of str, optional
+    other_keys_to_keep : sequence of str, optional
         Other columns to store besides the annotations.
 
     is_store_missing_annotations : bool, optional
         Whether to store missing annotations. If True it avoids trying to reannotate examples that have errors.
 
     base_dir : Path, optional
         Path to the directory containing the annotators configs. I.e. annotators_config will be relative
-        to this directory.
+        to this directory. If None uses self.DEFAULT_BASE_DIR
+
+    is_raise_if_missing_primary_keys : bool, optional
+        Whether to ensure that the primary keys are in the example dictionary. If True, raises an error.
+
+    tmp_missing_annototation : Any, optional
+        Temporary value to use for missing annotations when `is_store_missing_annotations` is True.
+
+    annotation_type : type, optional
+        Type to use for storing the annotations. If None, uses `self.DEFAULT_ANNOTATION_TYPE`.
     """
 
+    DEFAULT_BASE_DIR = constants.EVALUATORS_CONFIG_DIR
+    ANNOTATOR_COLUMN = "annotator"
+    TMP_MISSING_ANNOTATION = -1
+    DEFAULT_ANNOTATION_TYPE = int
+
     def __init__(
         self,
-        input_keys: Sequence[str],
-        output_keys: Sequence[str],
+        primary_keys: Sequence[str],
         annotators_config: Union[utils.AnyPath, list[dict[str, Any]]] = "claude",
         seed: Optional[int] = 0,
         is_avoid_reannotations: bool = True,
         other_keys_to_keep: Sequence[str] = ("price_per_example", "time_per_example"),
         is_store_missing_annotations: bool = True,
-        base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
+        base_dir: Optional[utils.AnyPath] = None,
+        is_raise_if_missing_primary_keys: bool = True,
+        annotation_type: Optional[Type] = None,
     ):
         logging.info(f"Creating the annotator from `{annotators_config}`.")
-        self.base_dir = Path(base_dir)
+        self.base_dir = Path(base_dir or self.DEFAULT_BASE_DIR)
         self.seed = seed
         self.is_avoid_reannotations = is_avoid_reannotations
-        self.input_keys = list(input_keys)
-        self.output_keys = list(output_keys)
-        self.input_output_keys = self.input_keys + self.output_keys
-        self.all_keys = self.input_keys + self.output_keys + ["annotator"]
+        self.primary_keys = list(primary_keys)
+        self.all_keys = self.primary_keys + [self.ANNOTATOR_COLUMN]
         self.other_keys_to_keep = list(other_keys_to_keep)
         self.is_store_missing_annotations = is_store_missing_annotations
+        self.is_raise_if_missing_primary_keys = is_raise_if_missing_primary_keys
+        self.annotation_type = annotation_type or self.DEFAULT_ANNOTATION_TYPE
 
         self.annotators_config = self._initialize_annotators_config(annotators_config)
         self.annotators = self._initialize_annotators()
         self.df_annotations = None
 
     ### Abstract methods ###
 
@@ -98,14 +110,19 @@
 
     #######################
     @property
     def annotation_key(self) -> str:
         """How to refer to the annotations, this will be the key for annotations in the output."""
         return "annotation"
 
+    @property
+    def random_seed_key(self) -> list[str]:
+        """What key / column to seed on for the random generator."""
+        return list(self.primary_keys)
+
     ### Public methods ###
     @property
     def annotator_name(self) -> str:
         return Path(self.annotators_config).parent.name
 
     def __call__(
         self,
@@ -113,23 +130,23 @@
         **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Main function for annotating.
 
         Parameters
         ----------
         to_annotate : list of dict or dataframe
-            Examples to annotate. Each dictionary (or row) should contain all of `self.input_output_keys`.
+            Examples to annotate. Each dictionary (or row) should contain all of `self.primary_keys`.
 
         **decoding_kwargs :
             Additional arguments to pass to `fn_completions`.
 
         Returns
         -------
         annotated : list of dict
-            The annotated examples. Each dict will contain all of `self.input_output_keys` and `self.annotation_key`.
+            The annotated examples. Each dict will contain all of `self.primary_keys` and `self.annotation_key`.
         """
         if len(to_annotate) == 0:
             return []
 
         df_to_annotate = self._preprocess(to_annotate)
         df_annotated = self._annotate(df_to_annotate, **decoding_kwargs)
         annotated = self._postprocess_and_store_(df_annotated, to_annotate)
@@ -143,42 +160,58 @@
         annotators_config = self.base_dir / annotators_config
 
         if annotators_config.is_dir():
             annotators_config = annotators_config / "configs.yaml"
 
         return annotators_config
 
-    def _initialize_annotators(self) -> dict[str, Type["SingleAnnotator"]]:
+    def _initialize_annotators(self) -> dict[str, "SingleAnnotator"]:
         """Load all the configs and prompts if necessary."""
         annotators_config = utils.load_configs(self.annotators_config)
+        try:
+            # in case a path is given we make it relative to that path
+            base_dir = self.annotators_config.parents[1]
+        except:
+            base_dir = self.base_dir
+
         return {
             name: self.SingleAnnotator(
-                seed=self.seed, base_dir=self.base_dir, annotation_column=self.annotation_key, **annotator_config
+                seed=self.seed, base_dir=base_dir, annotation_column=self.annotation_key, **annotator_config
             )
             for name, annotator_config in annotators_config.items()
         }
 
+    def _add_missing_primary_keys_(self, df: pd.DataFrame):
+        missing_primary_keys = [c for c in self.primary_keys if c not in df.columns]
+        if self.is_raise_if_missing_primary_keys:
+            if len(missing_primary_keys) > 0:
+                raise ValueError(f"Missing primary keys: {missing_primary_keys}")
+        else:
+            for c in missing_primary_keys:
+                df[c] = None
+
     def _preprocess(self, to_annotate: utils.AnyData) -> pd.DataFrame:
         """Preprocess the examples to annotate. In particular takes care of filtering unnecessary examples."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate).copy()
+        self._add_missing_primary_keys_(df_to_annotate)
 
         for c in self.other_keys_to_keep + [self.annotation_key]:
             if c in df_to_annotate.columns:
                 logging.warning(f"""{c} column is already in the dataframe. We will overwrite it.""")
-                df_to_annotate[c] = np.nan
+                df_to_annotate[c] = None
 
         # remove duplicates because you only need to annotate one of them
-        df_to_annotate = df_to_annotate.drop_duplicates(subset=self.input_output_keys)
+        df_to_annotate = df_to_annotate.drop_duplicates(subset=self.primary_keys)
 
         # set the annotater for each example
-        df_to_annotate["annotator"] = df_to_annotate.apply(
+        df_to_annotate[self.ANNOTATOR_COLUMN] = df_to_annotate.apply(
             lambda x: utils.random_seeded_choice(
                 # we add "annotator" at the beginning to not use the same seed for all tasks
-                seed="annotator" + x["instruction"] + str(self.seed),
+                seed="annotator" + "".join(x[self.random_seed_key]) + str(self.seed),
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
 
         if self.is_avoid_reannotations:
             df_to_annotate = self._apply_cached_annotations(df_to_annotate)
@@ -187,15 +220,17 @@
 
     def _annotate(self, df_to_annotate: pd.DataFrame, **decoding_kwargs) -> pd.DataFrame:
         """Annotate the examples."""
 
         df_annotated = df_to_annotate
         for annotator in self.annotators.keys():
             # only annotate examples that have not been annotated yet
-            curr_idcs = (df_annotated["annotator"] == annotator) & df_annotated[self.annotation_key].isna()
+            curr_idcs = df_annotated[self.ANNOTATOR_COLUMN] == annotator
+            if self.annotation_key in df_annotated.columns:
+                curr_idcs &= df_annotated[self.annotation_key].isna()
 
             logging.info(f"Annotating {curr_idcs.sum()} examples with {annotator}")
 
             # actual annotation
             curr_annotated = self.annotators[annotator](df_annotated.loc[curr_idcs, self.all_keys], **decoding_kwargs)
 
             df_annotated = self._merge_annotations(df_annotated, curr_annotated)
@@ -206,37 +241,40 @@
         self,
         df_annotated: pd.DataFrame,
         to_annotate: Union[Sequence[dict[str, Any]], pd.DataFrame],
     ) -> list[dict[str, Any]]:
         """Convert the dataframe into a list of dictionaries to be returned, and store current anntations."""
 
         df_to_annotate = utils.convert_to_dataframe(to_annotate)
+        self._add_missing_primary_keys_(df_to_annotate)
 
         # select available annotations
         if self.is_store_missing_annotations:
-            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].fillna(-1)
+            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].fillna(self.TMP_MISSING_ANNOTATION)
         else:
-            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].replace(-1, np.nan)
+            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].replace(
+                self.TMP_MISSING_ANNOTATION, None
+            )
 
         df_annotated = df_annotated[~df_annotated[self.annotation_key].isna()].copy()
 
-        # try converting to int now that no nan
-        df_annotated[self.annotation_key] = pd.to_numeric(
-            df_annotated[self.annotation_key], downcast="integer", errors="ignore"
-        )
+        # try converting to int now that no nan. Note this will only do so if possible
+        df_annotated[self.annotation_key] = df_annotated[self.annotation_key].astype(self.annotation_type)
 
         df_annotated = self._filter_annotations_before_storing(df_annotated)
         self._store_annotations_(df_annotated)
 
         if self.is_store_missing_annotations:
-            # put back np.nan
-            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].replace(-1, np.nan)
+            # put back None
+            df_annotated[self.annotation_key] = df_annotated[self.annotation_key].replace(
+                self.TMP_MISSING_ANNOTATION, None
+            )
 
         # need to merge with df_to_annotate in case you dropped duplicates
-        on = list(self.input_keys + self.output_keys)
+        on = list(self.primary_keys)
         df_annotated = df_annotated[self._get_all_keys_to_keep(df_to_annotate)]
         df_to_annotate = df_to_annotate[[c for c in df_to_annotate.columns if c not in df_annotated.columns or c in on]]
         # need to remove all other columns before merging if not you will
         df_annotated = df_to_annotate.merge(df_annotated, on=on, how="outer")
 
         annotated = df_annotated.to_dict(orient="records")
 
@@ -316,14 +354,15 @@
 
     def __init__(self, *args, caching_path: Optional[utils.AnyPath] = "auto", **kwargs):
         super().__init__(*args, **kwargs)
         self.caching_path = self._initialize_cache(caching_path)
 
     def save(self, path: Optional[utils.AnyPath] = None):
         """Save all annotations to json."""
+
         path = path or self.caching_path
         if path is not None:
             logging.info(f"Saving all annotations to {path}.")
             # to make sure that we don't overwrite the annotations we load again from file (ideally would use a DB)
             self._refresh_annotations_()
             if not self.is_store_missing_annotations:
                 self.df_annotations = self.df_annotations[~self.df_annotations[self.annotation_key].isna()]
@@ -371,17 +410,18 @@
     Parameters
     ----------
     prompt_template : str or path
         A prompt template that will be given to `fn_prompter` or path to those prompts. Path is relative to
         `evaluators_configs/`
 
     fn_completion_parser : callable or str
-        Function in `completion_parsers.py` to use for parsing the completions into annotations. For each completion,
-        the number of annotations should be equal to the batch_size if not we set all the annotations in that batch to
-        NaN.
+        Function that maps (parses) the completion to a list of annotations. If a string, it should be a function in
+        `completion_parsers.py` to use for parsing the completions into annotations. For each completion, the number of
+        annotations (lenght of list) should be equal to the batch_size if not we set all the annotations in that batch
+        to NaN.
 
     completion_parser_kwargs : dict
         Kwargs for fn_completion_parser.
 
     fn_completions : callable or str
         Function in `decoders.py` to use for decoding the output.
 
@@ -404,29 +444,31 @@
     annotation_column : str, optional
         Name of the annotation column in the output dataframe.
     """
 
     def __init__(
         self,
         prompt_template: utils.AnyPath,
-        fn_completion_parser: Union[Callable, str] = "regex_parser",
+        fn_completion_parser: Optional[Union[Callable, str]] = "regex_parser",
         completion_parser_kwargs: Optional[dict[str, Any]] = None,
         fn_completions: Union[Callable, str] = "openai_completions",
         completions_kwargs: Optional[dict[str, Any]] = None,
         is_shuffle: bool = True,
         seed: Optional[int] = 123,
         batch_size: int = 1,
         base_dir: utils.AnyPath = constants.EVALUATORS_CONFIG_DIR,
         annotation_column: str = "annotation",
     ):
         self.base_dir = Path(base_dir)
         self.prompt_template = self._get_prompt_template(prompt_template)
 
-        if isinstance(fn_completion_parser, str):
-            fn_completion_parser = getattr(completion_parsers, fn_completion_parser)
+        if fn_completion_parser is None:
+            fn_completion_parser = lambda x: [x]
+        elif isinstance(fn_completion_parser, str):
+            fn_completion_parser = self._search_fn_completion_parser(fn_completion_parser)
         completion_parser_kwargs = completion_parser_kwargs or {}
         self.fn_completion_parser = partial(fn_completion_parser, **completion_parser_kwargs)
 
         self.fn_completions = get_fn_completions(fn_completions)
         self.completions_kwargs = completions_kwargs or {}
         self.seed = seed
         self.is_shuffle = is_shuffle
@@ -470,14 +512,18 @@
         df_annotated = self._postprocess(df_to_annotate)
 
         return df_annotated
 
     ######################
 
     ### Private methods ###
+    def _search_fn_completion_parser(self, name: str) -> Callable:
+        """Search for a completion parser by name."""
+        return getattr(completion_parsers, name)
+
     def _get_prompt_template(self, prompt_template: utils.AnyPath):
         return utils.read_or_return(self.base_dir / prompt_template)
 
     def _make_prompts(
         self, df_to_annotate: pd.DataFrame, prompt_template: Optional[str] = None
     ) -> tuple[list[str], pd.DataFrame]:
         """Make all the prompts for the given examples.
@@ -506,26 +552,25 @@
         """Preprocess the examples before annotating. In particular, takes care of all the randomization."""
 
         if self.is_shuffle:
             df_to_annotate = df_to_annotate.sample(frac=1, random_state=self.seed)
 
         return df_to_annotate
 
-    def _parse_completions(self, completions: list[str]) -> list[int]:
+    def _parse_completions(self, completions: list[str]) -> list[Any]:
         """Converts the completions into annotations."""
         all_annotations = []
         for completion in completions:
-            # use a regex to match all outputs on a line. Assumes that there is at most one output to match per line
-            batch_annotations = self.fn_completion_parser(completion)
+            batch_annotations = list(self.fn_completion_parser(completion))
             if len(batch_annotations) != self.batch_size:
                 logging.warning(
                     f"Found {len(batch_annotations)} annotations in:'''\n{completion}\n''' but expected"
-                    f" {self.batch_size}. We are setting all annotations to np.nan."
+                    f" {self.batch_size}. We are setting all annotations to None."
                 )
-                batch_annotations = [np.nan] * self.batch_size
+                batch_annotations = [None] * self.batch_size
             all_annotations += batch_annotations
         return all_annotations
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         """Postprocess the annotated examples."""
 
         # remove padding examples when using batch_size > 1
@@ -535,12 +580,10 @@
         if arr_is_na.any():
             logging.warning(
                 f"{arr_is_na.sum().item()} samples had no auto annotation. We are filtering them for now. "
                 f"If you are using chain of thought it might be that max_tokens limit is too low. "
             )
             df_annotated = df_annotated[~arr_is_na]
 
-        assert set(df_annotated[self.annotation_column].unique().tolist()) <= {0, 1, 2}
-
         return df_annotated
 
     #######################
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.3/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,72 @@
 import logging
+from functools import partial
 from pathlib import Path
-from typing import Any, Callable, Optional, Sequence, Union
+from typing import Any, Callable, Optional, Sequence, Type, Union
 
 import numpy as np
 import pandas as pd
 
 from .. import utils
-from .base import BaseAnnotatorJSON, SingleAnnotator
+from .base import BaseAnnotator, BaseAnnotatorJSON, SingleAnnotator
 
 __all__ = ["PairwiseAnnotator", "SinglePairwiseAnnotator"]
 
-
-class PairwiseAnnotator(BaseAnnotatorJSON):
-    __doc__ = (
-        BaseAnnotatorJSON.__doc__.replace("Base class", "Class")
-        + """
+PAIRWISE_ADDED_DOCSTRING = """
     
     p_label_flip : float, optional
         Probability of flipping the label (ie adds noise by taking a mixture between predicted label and
         2*p_label_flip of independent coin flip). If None, will not flip the label. In AlpacaFarm we use 0.25
         for training. You can set this later on using `set_noise`.
         
+    input_keys : sequence of str, optional
+        Keys use to distinguish inputs.
+
+    output_keys : sequence of str, optional
+        Keys use to distinguish outputs.
+        
     Notes
     -----
     There are three main functions for annotations depending on how the outputs to compare are given:
         - annotate_pairs: annotate a sequence of examples that contain the pair of outputs `"output_1"` and `"output_2"`
         - annotate_samples: annotate a sequence of examples that contain `"output"` from which we will sample a pair of
             outputs. Useful for collecting pairwise preferences for RLHF.
         - annotate_head2head: annotate a pair of sequence of outputs, each containing `"output"` which will be merged
             into a single sequence of paired outputs. Useful for evaluation against a reference.
     """
-    )
+
+
+class PairwiseAnnotatorLocal(BaseAnnotator):
+    __doc__ = BaseAnnotator.__doc__.replace("Base class", "Class") + PAIRWISE_ADDED_DOCSTRING
 
     def __init__(
         self,
         *args,
         input_keys: Sequence[str] = ("instruction",),
         output_keys: Sequence[str] = ("output_1", "output_2"),
         p_label_flip: Optional[float] = None,
         **kwargs,
     ):
-        super().__init__(*args, **kwargs, input_keys=input_keys, output_keys=output_keys)
+        self.input_keys = list(input_keys)
+        self.output_keys = list(output_keys)
+        super().__init__(*args, **kwargs, primary_keys=self.input_keys + self.output_keys)
         self.p_label_flip = p_label_flip
 
     @property
-    def SingleAnnotator(self) -> SingleAnnotator:
-        return SinglePairwiseAnnotator
+    def SingleAnnotator(self) -> Type["SingleAnnotator"]:
+        return partial(SinglePairwiseAnnotator, random_seed_column=self.random_seed_key)
 
     @property
     def annotation_key(self) -> str:
         return "preference"
 
+    @property
+    def random_seed_key(self) -> list[str]:
+        return list(self.input_keys)
+
     def annotate_samples(
         self,
         all_outputs: utils.AnyData,
         keys_to_sample_output_2: Optional[Sequence] = None,
         is_unique_instructions: bool = True,
         p_label_flip: Optional[float] = None,
         is_multisample_list: bool = True,
@@ -233,23 +245,23 @@
         **decoding_kwargs,
     ) -> list[dict[str, Any]]:
         """Annotates the given examples, which contain both `"output_1"` and `"output_2"` keys.
 
         Parameters
         ----------
         to_annotate : list of dict or dataframe
-            Examples to annotate. Each dictionary (or row) should contain all of `self.input_output_keys`.
+            Examples to annotate. Each dictionary (or row) should contain all of `self.primary_keys`.
 
         **decoding_kwargs :
             Additional arguments to pass to `fn_completions`.
 
         Returns
         -------
         annotated : list of dict
-            The annotated examples. Each dictionary will contain all of `self.input_output_keys` and `"preference"`.
+            The annotated examples. Each dictionary will contain all of `self.primary_keys` and `"preference"`.
             Preference will be 0 if output_1 == output_2, 1 if output_1 is preferred, and 2 if output_2 is preferred.
         """
         # `annotate_pairs` is used for backward compatibility
         return self.__call__(to_annotate, **decoding_kwargs)
 
     def set_noise(self, p_label_flip: float):
         """Set the noise level for the annotators.
@@ -272,15 +284,15 @@
         if self.p_label_flip:
             logging.info(f"Adding random noise to the labels p_label_flip={self.p_label_flip}.")
             # if you have 25% change of flipping the label, you have 50% chance of selecting random label
             p_noise = self.p_label_flip * 2
             noisy_preference = df_to_annotate.apply(
                 # we add "noisy_label" at the beginning to use ~independent seeds between tasks
                 lambda x: utils.random_seeded_choice(  # seed on inputs for reproducibility
-                    seed="noisy_preference" + x["instruction"] + str(self.seed),
+                    seed="noisy_preference" + "".join(x[self.random_seed_key]) + str(self.seed),
                     choices=[np.nan, 1, 2],
                     weights=[1 - p_noise, self.p_label_flip, self.p_label_flip],
                 ),
                 axis=1,
             )
             df_to_annotate["is_noisy_label"] = ~noisy_preference.isna()
             # keeps previously annotated examples when you did not add noise
@@ -301,55 +313,67 @@
             # don't store noisy labels
             df_annotated = df_annotated.query("is_noisy_label == False").drop(columns=["is_noisy_label"])
 
         df_annotated = super()._filter_annotations_before_storing(df_annotated)
         return df_annotated
 
 
+# Note: we separate local and json to make it easier to inherit e.g. for having a database version
+class PairwiseAnnotator(PairwiseAnnotatorLocal, BaseAnnotatorJSON):
+    __doc__ = BaseAnnotatorJSON.__doc__.replace("Base class", "Class") + PAIRWISE_ADDED_DOCSTRING
+
+
 class SinglePairwiseAnnotator(SingleAnnotator):
     __doc__ = (
         SingleAnnotator.__doc__.replace(
             "A helper class for a single auto annotator.",
             "A helper class for a single pairwise auto annotator.",
         )
         + """
     is_randomize_output_order : bool
         Whether to randomize output_1, output_2 when formatting.
+        
+    random_seed_key : str
+        The column to use to seed the randomization of output_1, output_2.
     """
     )
 
     def __init__(
         self,
         *args,
         is_randomize_output_order: bool = True,
         annotation_column: str = "preference",
+        random_seed_column: Sequence[str] = ("instruction",),
         **kwargs,
     ):
         super().__init__(*args, annotation_column=annotation_column, **kwargs)
         self.is_randomize_output_order = is_randomize_output_order
+        self.random_seed_column = list(random_seed_column)
 
     def _preprocess(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
         if self.is_randomize_output_order:
             # randomize order of output_1, output_2 base on inputs
             df_to_annotate["is_switched_outputs"] = df_to_annotate.apply(
                 # we add "is_switched_outputs" at the beginning to not use the same seed for all tasks
                 lambda x: utils.random_seeded_choice(
-                    seed="is_switched_outputs" + x["instruction"] + str(self.seed),
+                    seed="is_switched_outputs" + "".join(x[self.random_seed_column]) + str(self.seed),
                     choices=[False, True],
                 ),
                 axis=1,
             )
             df_to_annotate = utils.shuffle_pairwise_preferences(df_to_annotate, df_to_annotate["is_switched_outputs"])
 
         df_to_annotate = super()._preprocess(df_to_annotate)
 
         return df_to_annotate
 
     def _postprocess(self, df_annotated: pd.DataFrame) -> pd.DataFrame:
         df_annotated = super()._postprocess(df_annotated)
 
+        assert set(df_annotated[self.annotation_column].unique().tolist()) <= {0, 1, 2}
+
         if self.is_randomize_output_order:
             # unshuffles output 1 and output 2. For binary preference, unshuffling is equivalent to reshuffling
             df_annotated = utils.shuffle_pairwise_preferences(df_annotated, df_annotated["is_switched_outputs"])
             df_annotated = df_annotated.drop(columns=["is_switched_outputs"])
 
         return df_annotated
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.3/src/alpaca_eval/completion_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         # avoid matching the same output twice
         completion = completion[match.end() :]
     return responses
 
 
 # modified from: https://github.com/lm-sys/FastChat/blob/main/fastchat/eval/eval_gpt_review.py#L47
 # does not work with batched completions
-def lmsys_parser(completion: str):
+def lmsys_parser(completion: str) -> list[Any]:
     r"""Parse a pair of scores from a single completion and returns which is better.
 
     Examples
     --------
     >>> lmsys_parser("1 7\n ...")
     [2]
     >>> lmsys_parser("7 1\n more text")
@@ -90,15 +90,15 @@
         else:
             raise Exception("Invalid score pair.")
     except Exception as e:
         logging.error(f"{e}\nContent: {completion}\n" "You must manually fix the score pair.")
         return [np.nan]
 
 
-def ranking_parser(completion):
+def ranking_parser(completion: str) -> list[Any]:
     r"""Parse a completion that contains a list of dictionary and returns the name of the preferred model.
 
     Examples
     --------
     >>> ranking_parser("[{'model': 'model_1', 'rank': 1}, {'model': 'model_2', 'rank': 2}]")
     [1]
     >>> ranking_parser("[{'model': 'model_1', 'rank': 2}, {'model': 'model_2', 'rank': 1}]")
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.3/src/alpaca_eval/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 DATASETS_FORCE_DOWNLOAD = os.environ.get("DATASETS_FORCE_DOWNLOAD", False)
 ########################
 
 DEFAULT_CACHE_DIR = None
 CURRENT_DIR = Path(__file__).parent
 EVALUATORS_CONFIG_DIR = CURRENT_DIR / "evaluators_configs"
 MODELS_CONFIG_DIR = CURRENT_DIR / "models_configs"
+BASE_DIR = Path(__file__).parents[2]
+RESULTS_DIR = BASE_DIR / "results"
 
 MINIMAL_MODELS = (
     "gpt4",
     "claude",
     "claude-2",
     "chatgpt",
     "wizardlm-13b",
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
     num_procs : int, optional
         Number of parallel processes to use for decoding.
 
     decoding_kwargs :
         Additional kwargs to pass to `anthropic.Client.completion`.
     """
+
     n_examples = len(prompts)
     if n_examples == 0:
         logging.info("No samples to annotate.")
         return []
     else:
         logging.info(f"Using `anthropic_completions` on {n_examples} prompts using {model_name}.")
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.3/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 alpaca_eval_gpt4_fn:
   prompt_template: "alpaca_eval_gpt4_fn/alpaca_eval_fn.txt"
   fn_completions: "openai_completions"
   completions_kwargs:
-    model_name: "gpt-4-0613" # TODO: need to update to gpt-4 on the 26th of june
+    model_name: "gpt-4" # TODO: need to update to gpt-4 on the 26th of june
     max_tokens: 100
     temperature: 0
     function_call:
       name: "make_leaderboard"
     functions:
       - name: "make_leaderboard"
         description: "Make a leaderboard of models given a list of the models ordered by the preference of their outputs."
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.3/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
-gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32
-claude-2,91.35572139303483,0.9897323784630048,minimal,1,804,734,69
-vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86
-claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89
-openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102
-wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108
-chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109
-openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120
-vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143
-openchat-13b,80.8695652173913,1.3843738653129234,community,2,805,650,153
-ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155
-openchat8192-13b,79.53980099502488,1.4222439886269744,community,1,804,639,164
-opencoderplus-15b,78.69565217391305,1.440029529188432,community,3,805,632,170
-vicuna-7b-v1.3,76.8414481897628,1.487520320531845,verified,3,801,614,184
-wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194
-airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202
-airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212
-guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227
-vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237
-baize-v2-13b,66.95652173913044,1.6565358231309506,community,2,805,538,265
-oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268
-minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271
-guanaco-33b,65.96273291925466,1.67108537053247,verified,0,805,531,274
-nous-hermes-13b,65.46583850931677,1.669962276077284,verified,6,805,524,275
-vicuna-7b,64.40993788819875,1.6851107260487883,verified,3,805,517,285
-baize-v2-7b,63.85093167701863,1.6945981855442178,community,0,805,514,291
-oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,verified,13,805,436,356
-guanaco-13b,52.60869565217391,1.7576690299699242,verified,3,805,422,380
-text_davinci_003,50.0,0.0,minimal,805,805,0,0
-guanaco-7b,46.58385093167702,1.7570464905413992,verified,2,805,374,429
-falcon-40b-instruct,45.71428571428572,1.7524717060805597,minimal,4,805,366,435
-alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,verified,10,805,350,445
-pythia-12b-mix-sft,41.86335403726708,1.737637146007538,verified,2,805,336,467
-alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,minimal,8,805,328,469
-cohere-chat,29.565217391304348,1.5949050483247118,community,12,805,232,561
-cohere,28.385093167701864,1.5717547121761728,community,15,805,221,569
-alpaca-7b,26.459627329192543,1.535711469748,minimal,16,805,205,584
-oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,verified,16,805,201,588
-falcon-7b-instruct,23.60248447204969,1.4898235369056625,verified,6,805,187,612
-text_davinci_001,15.17412935323383,1.235107892276849,minimal,20,804,112,672
+,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base,avg_length
+gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32,1365
+claude-2,91.35572139303484,0.9897323784630048,minimal,1,804,734,69,1069
+vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86,1479
+claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89,1082
+openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102,1566
+wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108,1525
+chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109,811
+openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120,1564
+vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143,1132
+openchat-13b,80.8695652173913,1.3843738653129234,community,2,805,650,153,1632
+ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155,1087
+openchat8192-13b,79.53980099502488,1.4222439886269744,community,1,804,639,164,1664
+opencoderplus-15b,78.69565217391305,1.440029529188432,community,3,805,632,170,1628
+vicuna-7b-v1.3,76.8414481897628,1.487520320531845,verified,3,801,614,184,1110
+wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194,985
+airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202,1512
+airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212,1514
+guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227,1249
+vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237,1037
+baize-v2-13b,66.95652173913044,1.6565358231309506,community,2,805,538,265,930
+oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268,1079
+minotaur-13b,66.02484472049689,1.6645545328264226,community,5,805,529,271,881
+guanaco-33b,65.96273291925466,1.67108537053247,verified,0,805,531,274,1311
+nous-hermes-13b,65.46583850931677,1.669962276077284,verified,6,805,524,275,844
+vicuna-7b,64.40993788819875,1.6851107260487883,verified,3,805,517,285,1044
+baize-v2-7b,63.85093167701863,1.6945981855442178,community,0,805,514,291,1127
+oasst-sft-llama-33b,54.96894409937888,1.7402667933686875,verified,13,805,436,356,748
+guanaco-13b,52.60869565217391,1.7576690299699242,verified,3,805,422,380,1774
+text_davinci_003,50.0,0.0,minimal,805,805,0,0,307
+guanaco-7b,46.58385093167702,1.7570464905413992,verified,2,805,374,429,1364
+falcon-40b-instruct,45.71428571428572,1.7524717060805597,minimal,4,805,366,435,662
+alpaca-farm-ppo-sim-gpt4-20k,44.099378881987576,1.7399772578861137,verified,10,805,350,445,511
+pythia-12b-mix-sft,41.86335403726708,1.737637146007538,verified,2,805,336,467,913
+alpaca-farm-ppo-human,41.24223602484472,1.7271813123250834,minimal,8,805,328,469,803
+cohere-chat,29.565217391304348,1.5949050483247118,community,12,805,232,561,779
+cohere,28.385093167701864,1.5717547121761728,community,15,805,221,569,682
+alpaca-7b,26.459627329192543,1.535711469748,minimal,16,805,205,584,396
+oasst-sft-pythia-12b,25.962732919254663,1.5261079289535309,verified,16,805,201,588,726
+falcon-7b-instruct,23.60248447204969,1.4898235369056625,verified,6,805,187,612,478
+text_davinci_001,15.17412935323383,1.235107892276849,minimal,20,804,112,672,296
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-,win_rate,standard_error,n_wins,n_wins_base,n_draws,n_total,mode
-gpt4,73.7888198757764,1.5359801545073597,588,205,12,805,minimal
-claude,70.37267080745342,1.599519507147828,562,234,9,805,minimal
-chatgpt,66.08695652173913,1.6626479994330317,529,270,6,805,minimal
-wizardlm-13b,65.15527950310559,1.670034107787565,520,276,9,805,minimal
-vicuna-13b,64.09937888198758,1.6895185863153146,515,288,2,805,minimal
-guanaco-65b,62.36024844720497,1.7086348811605765,502,303,0,805,minimal
-oasst-rlhf-llama-33b,62.0496894409938,1.7080028976103514,498,304,3,805,minimal
-alpaca-farm-ppo-human,60.24844720496895,1.7169496733548772,481,316,8,805,minimal
-falcon-40b-instruct,56.52173913043478,1.7438750520312944,453,348,4,805,minimal
-text_davinci_003,50.0,0.0,0,0,805,805,minimal
-alpaca-7b,45.21739130434783,1.7375846781579476,356,433,16,805,minimal
-text_davinci_001,28.07453416149068,1.5602183426587484,216,569,20,805,minimal
+,win_rate,standard_error,n_wins,n_wins_base,n_draws,n_total,mode,avg_length
+gpt4,73.7888198757764,1.5359801545073597,588,205,12,805,minimal,1365
+claude,70.37267080745342,1.599519507147828,562,234,9,805,minimal,1082
+chatgpt,66.08695652173913,1.6626479994330317,529,270,6,805,minimal,811
+wizardlm-13b,65.15527950310559,1.670034107787565,520,276,9,805,minimal,985
+vicuna-13b,64.09937888198758,1.6895185863153146,515,288,2,805,minimal,1037
+guanaco-65b,62.36024844720497,1.7086348811605765,502,303,0,805,minimal,1249
+oasst-rlhf-llama-33b,62.0496894409938,1.7080028976103514,498,304,3,805,minimal,1079
+alpaca-farm-ppo-human,60.24844720496895,1.7169496733548772,481,316,8,805,minimal,803
+falcon-40b-instruct,56.52173913043478,1.7438750520312944,453,348,4,805,minimal,662
+text_davinci_003,50.0,0.0,0,0,805,805,minimal,307
+alpaca-7b,45.21739130434783,1.7375846781579476,356,433,16,805,minimal,396
+text_davinci_001,28.07453416149068,1.5602183426587484,216,569,20,805,minimal,296
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
-gpt4,77.01863354037268,1.46803688292698,minimal,12,805,614,179
-claude,75.83850931677019,1.4981004247868313,minimal,9,805,606,190
-vicuna-33b-v1.3,72.36024844720497,1.5710737760483915,verified,5,805,580,220
-chatgpt,67.70186335403726,1.642111587090117,minimal,6,805,542,257
-vicuna-13b-v1.3,66.2111801242236,1.6657907370589309,verified,2,805,532,271
-wizardlm-13b,66.14906832298136,1.6584088766540706,minimal,9,805,528,268
-vicuna-13b,63.22981366459627,1.698243477332765,minimal,2,805,508,295
-guanaco-65b,62.60869565217392,1.7063755171155923,minimal,0,805,504,301
-vicuna-7b-v1.3,62.54658385093168,1.7035470981976453,verified,3,805,502,300
-nous-hermes-13b,60.86956521739131,1.7144465955143962,verified,6,805,487,312
-guanaco-33b,57.88819875776397,1.7412811662531051,verified,0,805,466,339
-vicuna-7b,57.329192546583855,1.7409917994657298,verified,3,805,460,342
-oasst-rlhf-llama-33b,57.329192546583855,1.7409917994657302,minimal,3,805,460,342
-guanaco-13b,53.36239103362392,1.7582560332920765,verified,3,803,427,373
-oasst-sft-llama-33b,51.24223602484472,1.748518981999294,verified,13,805,406,386
-text_davinci_003,50.0,0.0,minimal,805,805,0,0
-alpaca-farm-ppo-sim-gpt4-20k,48.19875776397515,1.7512254507446705,verified,10,805,383,412
-guanaco-7b,47.5776397515528,1.7590989434689512,verified,2,805,382,421
-falcon-40b-instruct,46.70807453416149,1.7551420072945083,minimal,4,805,374,427
-alpaca-farm-ppo-human,46.45962732919255,1.750131850347461,minimal,8,805,370,427
-pythia-12b-mix-sft,43.22981366459627,1.7449120766669366,verified,2,805,347,456
-oasst-sft-pythia-12b,32.79503105590062,1.6369108459870174,verified,16,805,256,533
-cohere-chat,32.79503105590062,1.6416235300873216,community,12,805,258,535
-cohere,32.608695652173914,1.635641080422956,community,15,805,255,535
-alpaca-7b,32.298136645962735,1.630307861230374,minimal,16,805,252,537
-falcon-7b-instruct,29.565217391304348,1.6021542242903124,verified,6,805,235,564
-text_davinci_001,21.490683229813666,1.421716368655911,minimal,20,805,163,622
+,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base,output_length,avg_length
+gpt4,77.01863354037268,1.46803688292698,minimal,12,805,614,179,,1365
+claude,75.83850931677019,1.4981004247868313,minimal,9,805,606,190,,1082
+vicuna-33b-v1.3,72.36024844720497,1.5710737760483915,verified,5,805,580,220,,1479
+claude-2,71.98757763975155,1.5824915958976835,minimal,1,805,579,225,1069.0,1069
+chatgpt,67.70186335403726,1.642111587090117,minimal,6,805,542,257,,811
+vicuna-13b-v1.3,66.2111801242236,1.6657907370589309,verified,2,805,532,271,,1132
+wizardlm-13b,66.14906832298136,1.6584088766540706,minimal,9,805,528,268,,985
+vicuna-13b,63.22981366459627,1.698243477332765,minimal,2,805,508,295,,1037
+guanaco-65b,62.60869565217392,1.7063755171155923,minimal,0,805,504,301,,1249
+vicuna-7b-v1.3,62.54658385093168,1.7035470981976453,verified,3,805,502,300,,1110
+nous-hermes-13b,60.86956521739131,1.7144465955143962,verified,6,805,487,312,,844
+guanaco-33b,57.88819875776397,1.7412811662531051,verified,0,805,466,339,,1311
+vicuna-7b,57.329192546583855,1.7409917994657298,verified,3,805,460,342,,1044
+oasst-rlhf-llama-33b,57.329192546583855,1.7409917994657302,minimal,3,805,460,342,,1079
+guanaco-13b,53.36239103362392,1.7582560332920765,verified,3,803,427,373,,1774
+oasst-sft-llama-33b,51.24223602484472,1.748518981999294,verified,13,805,406,386,,748
+text_davinci_003,50.0,0.0,minimal,805,805,0,0,,307
+alpaca-farm-ppo-sim-gpt4-20k,48.19875776397515,1.7512254507446705,verified,10,805,383,412,,511
+guanaco-7b,47.5776397515528,1.7590989434689512,verified,2,805,382,421,,1364
+falcon-40b-instruct,46.70807453416149,1.7551420072945083,minimal,4,805,374,427,,662
+alpaca-farm-ppo-human,46.45962732919255,1.750131850347461,minimal,8,805,370,427,,803
+pythia-12b-mix-sft,43.22981366459627,1.7449120766669366,verified,2,805,347,456,,913
+oasst-sft-pythia-12b,32.79503105590062,1.6369108459870174,verified,16,805,256,533,,726
+cohere-chat,32.79503105590062,1.6416235300873216,community,12,805,258,535,,779
+cohere,32.608695652173914,1.635641080422956,community,15,805,255,535,,682
+alpaca-7b,32.298136645962735,1.630307861230374,minimal,16,805,252,537,,396
+falcon-7b-instruct,29.565217391304348,1.6021542242903124,verified,6,805,235,564,,478
+text_davinci_001,21.490683229813666,1.421716368655911,minimal,20,805,163,622,,296
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.3/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/main.py` & `alpaca_eval-0.2.3/src/alpaca_eval/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
             )
 
             if isinstance(fn_metric, str):
                 fn_metric = getattr(metrics, fn_metric)
 
             leaderboard[name] = fn_metric(preferences=[a["preference"] for a in annotations])
             leaderboard[name]["mode"] = current_leaderboard_mode
+            leaderboard[name]["avg_length"] = int(model_outputs["output"].str.len().mean())
         else:
             logging.info(f"Skipping evaluation of {name} as it is already in the precomputed leaderboard.")
 
     output_path = utils.get_output_path(output_path, model_outputs, name)
 
     df_leaderboard = pd.DataFrame.from_dict(leaderboard, orient="index").sort_values(by=sort_by, ascending=False)
     df_leaderboard = df_leaderboard[
@@ -172,15 +173,15 @@
     if is_return_instead_of_print:
         return df_leaderboard, annotations
     else:
         utils.print_leaderboard(
             df_leaderboard,
             leaderboard_mode_to_print,
             current_name=name,
-            cols_to_print=["win_rate", "standard_error", "n_total"],
+            cols_to_print=["win_rate", "standard_error", "n_total", "avg_length"],  #
         )
 
 
 def evaluate_from_model(
     model_configs: Union[AnyPath, dict],
     reference_model_configs: Optional[Union[AnyPath, dict]] = None,
     evaluation_dataset: Union[AnyPath, AnyData, Callable] = constants.ALPACAEVAL_REFERENCE_OUTPUTS,
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.3/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.3/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.3/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.2
+Version: 0.2.3
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -17,36 +17,36 @@
 Provides-Extra: analysis
 Provides-Extra: dev
 Provides-Extra: local
 Provides-Extra: api
 Provides-Extra: all
 License-File: LICENSE
 
-# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
+# <a href="https://tatsu-lab.github.io/alpaca_eval/" target="_blank"><img src="https://raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png" width="35"></a> [AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) : An Automatic Evaluator for Instruction-following Language Models
 
 [![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE)
 [![Data License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE)
 [![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
 [![discord](https://img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/GJMxJSVZZM)
 
 Evaluation of instruction-following models (e.g., ChatGPT) typically requires human interactions. This is
 time-consuming, expensive, and hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is fast, cheap,
 replicable, and validated against 20K human annotations.
 It is particularly useful for model development.
-Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations).
+Although we improved over prior automatic evaluation pipelines, there are still fundamental [limitations](#limitations) like the preference for longer outputs.
 AlpacaEval provides the following:
 
+- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
+  evaluation set. **Caution**: Automatic evaluator (e.g. GPT4) may be biased towards models that generate longer outputs and/or that were fine-tuned on the model underlying the evaluator (e.g. GPT4).
 - [**Automatic evaluator**](#evaluators): an automatic evaluator that has high agreement with humans (validated on 20K
   annotations). We evaluate a
   model by
   measuring the fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the outputs from that model
   over
   outputs from a reference model. Our evaluators enable caching and output randomization by default.
-- [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the AlpacaEval
-  evaluation set.
 - [**Toolkit for building automatic evaluators**](#analysis): a simple interface for
   building advanced automatic evaluators (e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
   price, speed, statistical power, bias, variance etc).
 - [**Human evaluation data**](#data-release): 20K human preferences between a given and reference model
   on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
   evaluation set. 2.5K of these are cross-annotations (4 humans annotating the same 650 examples).
 - [**AlpacaEval dataset**](#data-release): a simplification
```

#### html2text {}

```diff
@@ -1,51 +1,55 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.2 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.3 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Requires-Python: >=3.10 Description-Content-Type: text/markdown
 Provides-Extra: analysis Provides-Extra: dev Provides-Extra: local Provides-
 Extra: api Provides-Extra: all License-File: LICENSE # [https://
 raw.githubusercontent.com/tatsu-lab/alpaca_eval/main/docs/AlpacaFarm_small.png]
-AlpacaEval : An Automatic Evaluator for Instruction-following Language Models
-[![Code License](https://img.shields.io/badge/Code%20License-Apache_2.0-
-green.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data
-License](https://img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-
-red.svg)](https://github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [!
-[Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://
-www.python.org/downloads/release/python-3100/) [![discord](https://
-img.shields.io/badge/discord-server-blue?logo=discord&logoColor=white)](https:/
-/discord.gg/GJMxJSVZZM) Evaluation of instruction-following models (e.g.,
-ChatGPT) typically requires human interactions. This is time-consuming,
-expensive, and hard to replicate. AlpacaEval in an LLM-based automatic
-evaluation that is fast, cheap, replicable, and validated against 20K human
-annotations. It is particularly useful for model development. Although we
-improved over prior automatic evaluation pipelines, there are still fundamental
-[limitations](#limitations). AlpacaEval provides the following: - [**Automatic
-evaluator**](#evaluators): an automatic evaluator that has high agreement with
-humans (validated on 20K annotations). We evaluate a model by measuring the
-fraction of times an powerful LLM (e.g. GPT 4 or Claude or ChatGPT) prefers the
-outputs from that model over outputs from a reference model. Our evaluators
-enable caching and output randomization by default. - [**Leaderboard**](https:/
-/tatsu-lab.github.io/alpaca_eval/): a leaderboard of common models on the
-AlpacaEval evaluation set. - [**Toolkit for building automatic evaluators**]
-(#analysis): a simple interface for building advanced automatic evaluators
-(e.g. with caching, batching, or multi-annotators) and analyzing them (quality,
-price, speed, statistical power, bias, variance etc). - [**Human evaluation
-data**](#data-release): 20K human preferences between a given and reference
-model on the [AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main)
-evaluation set. 2.5K of these are cross-annotations (4 humans annotating the
-same 650 examples). - [**AlpacaEval dataset**](#data-release): a simplification
-of [AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main)
-evaluation set, where "instructions" and " inputs" are merged into one field,
-and reference outputs are longer. **When to use AlpacaEval?** Our automatic
+[AlpacaEval](https://tatsu-lab.github.io/alpaca_eval/) : An Automatic Evaluator
+for Instruction-following Language Models [![Code License](https://
+img.shields.io/badge/Code%20License-Apache_2.0-green.svg)](https://github.com/
+tatsu-lab/alpaca_farm/blob/main/LICENSE) [![Data License](https://
+img.shields.io/badge/Data%20License-CC%20By%20NC%204.0-red.svg)](https://
+github.com/tatsu-lab/alpaca_farm/blob/main/DATA_LICENSE) [![Python 3.10+]
+(https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/
+downloads/release/python-3100/) [![discord](https://img.shields.io/badge/
+discord-server-blue?logo=discord&logoColor=white)](https://discord.gg/
+GJMxJSVZZM) Evaluation of instruction-following models (e.g., ChatGPT)
+typically requires human interactions. This is time-consuming, expensive, and
+hard to replicate. AlpacaEval in an LLM-based automatic evaluation that is
+fast, cheap, replicable, and validated against 20K human annotations. It is
+particularly useful for model development. Although we improved over prior
+automatic evaluation pipelines, there are still fundamental [limitations]
+(#limitations) like the preference for longer outputs. AlpacaEval provides the
+following: - [**Leaderboard**](https://tatsu-lab.github.io/alpaca_eval/): a
+leaderboard of common models on the AlpacaEval evaluation set. **Caution**:
+Automatic evaluator (e.g. GPT4) may be biased towards models that generate
+longer outputs and/or that were fine-tuned on the model underlying the
+evaluator (e.g. GPT4). - [**Automatic evaluator**](#evaluators): an automatic
+evaluator that has high agreement with humans (validated on 20K annotations).
+We evaluate a model by measuring the fraction of times an powerful LLM (e.g.
+GPT 4 or Claude or ChatGPT) prefers the outputs from that model over outputs
+from a reference model. Our evaluators enable caching and output randomization
+by default. - [**Toolkit for building automatic evaluators**](#analysis): a
+simple interface for building advanced automatic evaluators (e.g. with caching,
+batching, or multi-annotators) and analyzing them (quality, price, speed,
+statistical power, bias, variance etc). - [**Human evaluation data**](#data-
+release): 20K human preferences between a given and reference model on the
+[AlpacaFarm](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
+set. 2.5K of these are cross-annotations (4 humans annotating the same 650
+examples). - [**AlpacaEval dataset**](#data-release): a simplification of
+[AlpacaFarm's](https://github.com/tatsu-lab/alpaca_farm/tree/main) evaluation
+set, where "instructions" and " inputs" are merged into one field, and
+reference outputs are longer. **When to use AlpacaEval?** Our automatic
 evaluator is a quick and cheap proxy for human evaluation of simple
 instruction-following tasks. It is useful if you have to run many evaluations
 quickly, e.g., during model development. **When not to use AlpacaEval?** As any
 other automatic evaluator, AlpacaEval should **not replace human evaluation in
 high-stake decision-making**, e.g., to decide on model release. In particular,
 AlpacaEval is limited by the fact that (1) the instructions in the eval set
 might not be representative of advanced usage of LLMs; (2) automatic evaluators
```

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.3/src/alpaca_eval.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/tests/test_analyze.py` & `alpaca_eval-0.2.3/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/tests/test_decoders_unit.py` & `alpaca_eval-0.2.3/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.2/tests/test_main.py` & `alpaca_eval-0.2.3/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         main.evaluate(model_outputs, reference_outputs, annotators_config="test", is_avoid_reannotations=False)
 
         # Capture the stdout
         captured = capsys.readouterr()
         printed_string = captured.out.strip()
         printed_string = re.sub(r"\s+", " ", printed_string)
 
-        assert printed_string == "win_rate standard_error n_total Current model 0.00 0.00 3"
+        assert printed_string == "win_rate standard_error n_total avg_length Current model 0.00 0.00 3 1"
 
     clean_up()
 
 
 def test_evaluate_basic(model_outputs, reference_outputs, expected_annotations):
     mock_function = _get_mock_annotate()
     name = "Current model"
```

### Comparing `alpaca_eval-0.2.2/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.3/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

