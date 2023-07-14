# Comparing `tmp/council_ai-0.0.5.tar.gz` & `tmp/council_ai-0.0.6.tar.gz`

## Comparing `council_ai-0.0.5.tar` & `council_ai-0.0.6.tar`

### file list

```diff
@@ -1,157 +1,157 @@
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/Makefile
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.5/engine_flow.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.5/requirements.txt
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/__init__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agent_tests/__init__.py
--rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agent_tests/agent_tests.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/__init__.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent_chain.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/agents/agent_result.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/chains/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/chains/chain.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/cancellation_token.py
--rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/execution_context.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/contexts/messages.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/basic_controller.py
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/controller_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/execution_unit.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/controllers/llm_controller.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/basic_evaluator.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/evaluator_base.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/evaluators/llm_evaluator.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/__init__.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/azure_llm.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/azure_llm_configuration.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_base.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_configuration_base.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_exception.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/llm_message.py
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_chat_completions_llm.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_llm.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/llm/openai_llm_configuration.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/mocks/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/prompt/__init__.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/prompt/prompt_builder.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/budget.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/errrors.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/if_runner.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/loop_runner_base.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/parallel.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/parallel_for.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/runner_base.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/runner_executor.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/sequential.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/skill_runner_base.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/runners/types.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/__init__.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/llm_similarity_scorer.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/scorer_base.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/scorers/scorer_exception.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/__init__.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/llm_skill.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/skill_base.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/__init__.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_news_skill.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_search_skill.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/__init__.py
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/context_provider.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/google_news.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/google_search.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/skills/google/google_context/schemas.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/env.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/option.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.5/council/utils/result.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/.gitignore
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/.readthedocs.yaml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/Makefile
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/README.md
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/docker-compose.yaml
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/dockerfile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/make.bat
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/requirements.txt
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/conf.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/index.rst
--rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/_static/00_chainml_logo.png
--rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/_static/02_chainml_logo_black.png
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/contributing/contributing.md
--rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/getting_started/first_example.ipynb
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/getting_started/installation.md
--rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/engine_flow.png
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/key_concepts.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/key_features.md
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/introduction/welcome.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/chains.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts.rst
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators.rst
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm.rst
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents/agent.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/agents/agent_result.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/chains/chain.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/agent_context.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/agent_message.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chain_context.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chain_history.rst
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_history.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_message_base.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/chat_message_kind.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/iteration_context.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/scored_agent_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_context.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_error_message.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_message.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/skill_success_message.rst
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/contexts/user_message.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/basic_controller.rst
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/controller_base.rst
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/controllers/llm_controller.rst
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/basic_evaluator.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/evaluator_base.rst
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/evaluators/llm_evaluator.rst
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/azure_llm.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/azure_llm_configuration.rst
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_base.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_configuration_base.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_message.rst
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/llm_message_role.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/openai_llm.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/llm/openai_llm_configuration.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/budget.rst
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/errors.rst
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/if.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/loop_runner_base.rst
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/parallel.rst
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/parallel_for.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/runner_base.rst
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/runner_executor.rst
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/sequential.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/runners/skill_runner_base.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/llm_similarity_scorer.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/scorer_base.rst
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/scorers/scorer_exception.rst
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google.rst
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/llm_skill.rst
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/skill_base.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google/google_news_skill.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/skills/google/google_search_skill.rst
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils/option.rst
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/reference/utils/option_exception.rst
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/use_cases/langchain_llm_integration.ipynb
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 council_ai-0.0.5/docs/source/use_cases/multi_chain_agent.ipynb
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.5/stubs/GoogleNews.pyi
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.5/LICENSE
--rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 council_ai-0.0.5/README.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 council_ai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/Makefile
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.6/engine_flow.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 council_ai-0.0.6/requirements.txt
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agent_tests/__init__.py
+-rw-r--r--   0        0        0     6616 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agent_tests/agent_tests.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/__init__.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent_chain.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/agents/agent_result.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/chains/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/chains/chain.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/cancellation_token.py
+-rw-r--r--   0        0        0     9517 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/execution_context.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/contexts/messages.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/basic_controller.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/controller_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/execution_unit.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/controllers/llm_controller.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/basic_evaluator.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/evaluator_base.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/__init__.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/azure_llm.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/azure_llm_configuration.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_base.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_configuration_base.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_exception.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/llm_message.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_chat_completions_llm.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_llm.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/llm/openai_llm_configuration.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/mocks/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/prompt/__init__.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/prompt/prompt_builder.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/budget.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/errrors.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/if_runner.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/loop_runner_base.py
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/parallel.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/parallel_for.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/runner_base.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/runner_executor.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/sequential.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/skill_runner_base.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/runners/types.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/__init__.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/llm_similarity_scorer.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/scorer_base.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/scorers/scorer_exception.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/__init__.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/llm_skill.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/skill_base.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/__init__.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_news_skill.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_search_skill.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/__init__.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/context_provider.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/google_news.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/google_search.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/skills/google/google_context/schemas.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/env.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/option.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 council_ai-0.0.6/council/utils/result.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/.gitignore
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/README.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/docker-compose.yaml
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/dockerfile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/make.bat
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/requirements.txt
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/conf.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/index.rst
+-rw-r--r--   0        0        0    17142 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/_static/00_chainml_logo.png
+-rw-r--r--   0        0        0    18827 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/_static/02_chainml_logo_black.png
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/contributing/contributing.md
+-rw-r--r--   0        0        0     5185 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/getting_started/first_example.ipynb
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/getting_started/installation.md
+-rw-r--r--   0        0        0    34335 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/engine_flow.png
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/key_concepts.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/key_features.md
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/introduction/welcome.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/chains.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators.rst
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm.rst
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents/agent.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/agents/agent_result.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/chains/chain.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/agent_context.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/agent_message.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chain_context.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chain_history.rst
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_history.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_message_base.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/chat_message_kind.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/iteration_context.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/scored_agent_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_context.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_error_message.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_message.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/skill_success_message.rst
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/contexts/user_message.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/basic_controller.rst
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/controller_base.rst
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/controllers/llm_controller.rst
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/basic_evaluator.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/evaluator_base.rst
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/evaluators/llm_evaluator.rst
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/azure_llm.rst
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/azure_llm_configuration.rst
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_base.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_configuration_base.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_message.rst
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/llm_message_role.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/openai_llm.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/llm/openai_llm_configuration.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/budget.rst
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/errors.rst
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/if.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/loop_runner_base.rst
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/parallel.rst
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/parallel_for.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/runner_base.rst
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/runner_executor.rst
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/sequential.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/runners/skill_runner_base.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/llm_similarity_scorer.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/scorer_base.rst
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/scorers/scorer_exception.rst
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google.rst
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/llm_skill.rst
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/skill_base.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google/google_news_skill.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/skills/google/google_search_skill.rst
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils/option.rst
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/reference/utils/option_exception.rst
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/use_cases/langchain_llm_integration.ipynb
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 council_ai-0.0.6/docs/source/use_cases/multi_chain_agent.ipynb
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 council_ai-0.0.6/stubs/GoogleNews.pyi
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 council_ai-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 council_ai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     9277 2020-02-02 00:00:00.000000 council_ai-0.0.6/README.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 council_ai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 council_ai-0.0.6/PKG-INFO
```

### Comparing `council_ai-0.0.5/engine_flow.png` & `council_ai-0.0.6/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/agent_tests/agent_tests.py` & `council_ai-0.0.6/council/agent_tests/agent_tests.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/agents/agent.py` & `council_ai-0.0.6/council/agents/agent.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/agents/agent_chain.py` & `council_ai-0.0.6/council/agents/agent_chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/agents/agent_result.py` & `council_ai-0.0.6/council/agents/agent_result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/chains/chain.py` & `council_ai-0.0.6/council/chains/chain.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/contexts/execution_context.py` & `council_ai-0.0.6/council/contexts/execution_context.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/contexts/messages.py` & `council_ai-0.0.6/council/contexts/messages.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/controllers/basic_controller.py` & `council_ai-0.0.6/council/controllers/basic_controller.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/controllers/controller_base.py` & `council_ai-0.0.6/council/controllers/controller_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/controllers/llm_controller.py` & `council_ai-0.0.6/council/controllers/llm_controller.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/evaluators/basic_evaluator.py` & `council_ai-0.0.6/council/evaluators/basic_evaluator.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/evaluators/evaluator_base.py` & `council_ai-0.0.6/council/evaluators/evaluator_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/evaluators/llm_evaluator.py` & `council_ai-0.0.6/council/evaluators/llm_evaluator.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/azure_llm.py` & `council_ai-0.0.6/council/llm/azure_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/azure_llm_configuration.py` & `council_ai-0.0.6/council/llm/azure_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/llm_base.py` & `council_ai-0.0.6/council/llm/llm_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/llm_configuration_base.py` & `council_ai-0.0.6/council/llm/llm_configuration_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/llm_message.py` & `council_ai-0.0.6/council/llm/llm_message.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/openai_chat_completions_llm.py` & `council_ai-0.0.6/council/llm/openai_chat_completions_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/openai_llm.py` & `council_ai-0.0.6/council/llm/openai_llm.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/llm/openai_llm_configuration.py` & `council_ai-0.0.6/council/llm/openai_llm_configuration.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/mocks/__init__.py` & `council_ai-0.0.6/council/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/prompt/prompt_builder.py` & `council_ai-0.0.6/council/prompt/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/__init__.py` & `council_ai-0.0.6/council/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/budget.py` & `council_ai-0.0.6/council/runners/budget.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/errrors.py` & `council_ai-0.0.6/council/runners/errrors.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/if_runner.py` & `council_ai-0.0.6/council/runners/if_runner.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/parallel.py` & `council_ai-0.0.6/council/runners/parallel.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/parallel_for.py` & `council_ai-0.0.6/council/runners/parallel_for.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/runner_base.py` & `council_ai-0.0.6/council/runners/runner_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/sequential.py` & `council_ai-0.0.6/council/runners/sequential.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/runners/skill_runner_base.py` & `council_ai-0.0.6/council/runners/skill_runner_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/scorers/llm_similarity_scorer.py` & `council_ai-0.0.6/council/scorers/llm_similarity_scorer.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/scorers/scorer_base.py` & `council_ai-0.0.6/council/scorers/scorer_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/llm_skill.py` & `council_ai-0.0.6/council/skills/llm_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/skill_base.py` & `council_ai-0.0.6/council/skills/skill_base.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_news_skill.py` & `council_ai-0.0.6/council/skills/google/google_news_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_search_skill.py` & `council_ai-0.0.6/council/skills/google/google_search_skill.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_context/context_provider.py` & `council_ai-0.0.6/council/skills/google/google_context/context_provider.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_context/google_news.py` & `council_ai-0.0.6/council/skills/google/google_context/google_news.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_context/google_search.py` & `council_ai-0.0.6/council/skills/google/google_context/google_search.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/skills/google/google_context/schemas.py` & `council_ai-0.0.6/council/skills/google/google_context/schemas.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/utils/env.py` & `council_ai-0.0.6/council/utils/env.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/utils/option.py` & `council_ai-0.0.6/council/utils/option.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/council/utils/result.py` & `council_ai-0.0.6/council/utils/result.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/.readthedocs.yaml` & `council_ai-0.0.6/docs/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/Makefile` & `council_ai-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/make.bat` & `council_ai-0.0.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/conf.py` & `council_ai-0.0.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/index.rst` & `council_ai-0.0.6/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/_static/00_chainml_logo.png` & `council_ai-0.0.6/docs/source/_static/00_chainml_logo.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/_static/02_chainml_logo_black.png` & `council_ai-0.0.6/docs/source/_static/02_chainml_logo_black.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/getting_started/first_example.ipynb` & `council_ai-0.0.6/docs/source/getting_started/first_example.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/getting_started/installation.md` & `council_ai-0.0.6/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/introduction/engine_flow.png` & `council_ai-0.0.6/docs/source/introduction/engine_flow.png`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/introduction/key_concepts.md` & `council_ai-0.0.6/docs/source/introduction/key_concepts.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/introduction/key_features.md` & `council_ai-0.0.6/docs/source/introduction/key_features.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/introduction/welcome.md` & `council_ai-0.0.6/docs/source/introduction/welcome.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/reference/runners.rst` & `council_ai-0.0.6/docs/source/reference/runners.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/reference/runners/parallel_for.rst` & `council_ai-0.0.6/docs/source/reference/runners/parallel_for.rst`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/use_cases/langchain_llm_integration.ipynb` & `council_ai-0.0.6/docs/source/use_cases/langchain_llm_integration.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/docs/source/use_cases/multi_chain_agent.ipynb` & `council_ai-0.0.6/docs/source/use_cases/multi_chain_agent.ipynb`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/stubs/GoogleNews.pyi` & `council_ai-0.0.6/stubs/GoogleNews.pyi`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/LICENSE` & `council_ai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/README.md` & `council_ai-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `council_ai-0.0.5/pyproject.toml` & `council_ai-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "council-ai"
-version = "0.0.5"
+version = "0.0.6"
 description = "Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = []
 license = "Apache-2.0"
 
 dynamic = ["dependencies"]
```

### Comparing `council_ai-0.0.5/PKG-INFO` & `council_ai-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: council-ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: Council is an open-source framework for the rapid development and robust deployment of customized generative AI applications
 Project-URL: Source, https://github.com/chain-ml/council
 Project-URL: Documentation, https://council.dev
 License-Expression: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: google-api-python-client-stubs
```

