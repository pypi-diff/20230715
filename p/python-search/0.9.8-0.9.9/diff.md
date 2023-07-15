# Comparing `tmp/python_search-0.9.8.tar.gz` & `tmp/python_search-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_search-0.9.8.tar", max compression
+gzip compressed data, was "python_search-0.9.9.tar", max compression
```

## Comparing `python_search-0.9.8.tar` & `python_search-0.9.9.tar`

### file list

```diff
@@ -1,115 +1,120 @@
--rw-r--r--   0        0        0    11398 2022-10-01 09:12:26.670473 python_search-0.9.8/LICENSE
--rw-r--r--   0        0        0     2971 2023-01-03 16:35:00.438470 python_search-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     8196 2022-11-19 17:37:31.483827 python_search-0.9.8/python_search/.DS_Store
--rw-r--r--   0        0        0       15 2022-10-01 09:12:26.671734 python_search-0.9.8/python_search/__init__.py
--rw-r--r--   0        0        0      251 2022-10-01 09:12:26.671776 python_search-0.9.8/python_search/acronyms.py
--rw-r--r--   0        0        0       59 2022-10-01 09:12:26.671838 python_search-0.9.8/python_search/apps/README.md
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.671859 python_search-0.9.8/python_search/apps/__init__.py
--rwxr-xr-x   0        0        0      112 2022-10-01 09:12:26.671907 python_search-0.9.8/python_search/apps/apps.py
--rw-r--r--   0        0        0     1146 2022-12-23 14:47:49.486069 python_search-0.9.8/python_search/apps/browser.py
--rw-r--r--   0        0        0     1944 2023-01-03 09:57:40.151609 python_search-0.9.8/python_search/apps/clipboard.py
--rw-r--r--   0        0        0     1913 2022-12-13 21:04:16.717295 python_search-0.9.8/python_search/apps/collect_input.py
--rw-r--r--   0        0        0      457 2022-12-23 14:47:49.486559 python_search-0.9.8/python_search/apps/notification_ui.py
--rw-r--r--   0        0        0     1428 2022-10-01 09:12:26.672267 python_search-0.9.8/python_search/apps/terminal.py
--rw-r--r--   0        0        0     1696 2022-10-01 09:12:26.672324 python_search-0.9.8/python_search/apps/window_manager.py
--rw-r--r--   0        0        0     6947 2023-01-03 08:39:20.309493 python_search-0.9.8/python_search/cli.py
--rw-r--r--   0        0        0     5456 2022-12-29 18:58:43.553100 python_search-0.9.8/python_search/config.py
--rwxr-xr-x   0        0        0     3438 2022-12-30 09:02:14.416306 python_search-0.9.8/python_search/container.py
--rw-r--r--   0        0        0     1338 2022-10-13 17:07:39.032520 python_search-0.9.8/python_search/context.py
--rw-r--r--   0        0        0     1679 2022-10-13 17:20:14.018311 python_search-0.9.8/python_search/core_entities.py
--rw-r--r--   0        0        0     1622 2022-12-23 14:47:49.487856 python_search-0.9.8/python_search/data_collector.py
--rw-r--r--   0        0        0     1587 2022-12-23 14:47:49.488152 python_search-0.9.8/python_search/data_exporter.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.672706 python_search-0.9.8/python_search/data_ui/__init__.py
--rw-r--r--   0        0        0     1403 2022-12-23 14:47:49.488383 python_search-0.9.8/python_search/data_ui/app_functions.py
--rw-r--r--   0        0        0     2882 2022-12-28 16:49:13.785711 python_search-0.9.8/python_search/data_ui/entries_page.py
--rw-r--r--   0        0        0     1465 2022-12-23 14:47:49.488894 python_search-0.9.8/python_search/data_ui/main.py
--rw-r--r--   0        0        0     3148 2022-11-11 11:59:08.979894 python_search-0.9.8/python_search/data_ui/results_page.py
--rw-r--r--   0        0        0      552 2022-11-11 11:59:08.966918 python_search-0.9.8/python_search/data_ui/training_page.py
--rw-r--r--   0        0        0     2151 2022-10-01 09:12:26.673012 python_search-0.9.8/python_search/entries_group.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.673055 python_search-0.9.8/python_search/entry_capture/__init__.py
--rw-r--r--   0        0        0     2839 2022-12-23 14:47:49.489375 python_search-0.9.8/python_search/entry_capture/edit_content.py
--rw-r--r--   0        0        0     6061 2022-12-23 14:47:49.489705 python_search-0.9.8/python_search/entry_capture/entry_inserter_gui.py
--rw-r--r--   0        0        0     3098 2022-12-23 14:47:49.490014 python_search-0.9.8/python_search/entry_capture/filesystem_entry_inserter.py
--rw-r--r--   0        0        0     4072 2022-12-13 21:33:35.027266 python_search-0.9.8/python_search/entry_capture/register_new.py
--rw-r--r--   0        0        0      881 2022-10-01 09:12:26.673375 python_search-0.9.8/python_search/entry_capture/ui.py
--rw-r--r--   0        0        0        0 2022-11-14 22:10:50.074354 python_search-0.9.8/python_search/entry_description_generator/__init__.py
--rw-r--r--   0        0        0     2196 2022-12-23 14:47:49.490251 python_search-0.9.8/python_search/entry_description_generator/description_geneartor.py
--rw-r--r--   0        0        0     4387 2022-12-23 14:47:49.490475 python_search-0.9.8/python_search/entry_description_generator/pipeline.py
--rw-r--r--   0        0        0     4302 2022-12-23 14:47:49.490719 python_search-0.9.8/python_search/entry_runner.py
--rw-r--r--   0        0        0        0 2022-10-25 22:57:35.357775 python_search-0.9.8/python_search/entry_type/__init__.py
--rw-r--r--   0        0        0     3718 2022-12-23 14:47:49.490972 python_search-0.9.8/python_search/entry_type/classifier_inference.py
--rw-r--r--   0        0        0     1179 2022-10-27 11:22:43.268652 python_search-0.9.8/python_search/entry_type/entity.py
--rw-r--r--   0        0        0     6868 2022-12-23 14:47:49.491214 python_search-0.9.8/python_search/entry_type/entry_type_pipeline.py
--rw-r--r--   0        0        0       76 2022-10-01 09:12:26.673482 python_search-0.9.8/python_search/environment.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.673530 python_search-0.9.8/python_search/events/__init__.py
--rwxr-xr-x   0        0        0      822 2022-10-13 17:20:14.029602 python_search-0.9.8/python_search/events/latest_used_entries.py
--rw-r--r--   0        0        0     1448 2022-12-23 14:47:49.491458 python_search-0.9.8/python_search/events/ranking_generated/__init__.py
--rw-r--r--   0        0        0      103 2022-12-13 21:33:35.028835 python_search-0.9.8/python_search/events/run_performed/__init__.py
--rw-r--r--   0        0        0     1616 2022-12-29 18:28:49.423597 python_search-0.9.8/python_search/events/run_performed/clean.py
--rw-r--r--   0        0        0     1959 2022-12-29 18:34:15.251539 python_search-0.9.8/python_search/events/run_performed/dataset.py
--rw-r--r--   0        0        0      699 2022-12-13 21:33:35.029494 python_search-0.9.8/python_search/events/run_performed/entity.py
--rw-r--r--   0        0        0      854 2022-12-23 14:47:49.491965 python_search-0.9.8/python_search/events/run_performed/writer.py
--rw-r--r--   0        0        0     1568 2022-12-13 21:04:16.721761 python_search-0.9.8/python_search/exceptions.py
--rw-r--r--   0        0        0     1292 2022-10-10 20:17:32.106360 python_search-0.9.8/python_search/feature_toggle.py
--rw-r--r--   0        0        0      977 2022-10-13 17:20:14.045859 python_search-0.9.8/python_search/features.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.673993 python_search-0.9.8/python_search/infrastructure/__init__.py
--rw-r--r--   0        0        0     1297 2022-12-23 14:47:49.492187 python_search-0.9.8/python_search/infrastructure/arize.py
--rwxr-xr-x   0        0        0     3473 2022-12-28 13:13:54.310711 python_search-0.9.8/python_search/infrastructure/infrastructure.py
--rw-r--r--   0        0        0      791 2022-10-01 09:12:26.674111 python_search-0.9.8/python_search/infrastructure/performance.py
--rw-r--r--   0        0        0      437 2022-12-23 14:47:49.492333 python_search-0.9.8/python_search/infrastructure/redis.py
--rw-r--r--   0        0        0      345 2022-10-01 09:12:26.674202 python_search-0.9.8/python_search/infrastructure/report.py
--rwxr-xr-x   0        0        0     2347 2022-12-13 21:04:16.722803 python_search-0.9.8/python_search/init/entries_main.py
--rw-r--r--   0        0        0     1531 2022-10-18 16:14:55.666794 python_search-0.9.8/python_search/init/install_dependencies.py
--rw-r--r--   0        0        0     1464 2022-10-13 17:20:14.067698 python_search-0.9.8/python_search/init/project.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.674407 python_search-0.9.8/python_search/interpreter/__init__.py
--rw-r--r--   0        0        0     3145 2022-10-01 09:12:26.674473 python_search-0.9.8/python_search/interpreter/base.py
--rw-r--r--   0        0        0     3530 2022-12-23 14:47:49.492606 python_search-0.9.8/python_search/interpreter/cmd.py
--rw-r--r--   0        0        0     1937 2022-12-29 12:55:48.417490 python_search-0.9.8/python_search/interpreter/file.py
--rw-r--r--   0        0        0      978 2022-10-01 09:12:26.674651 python_search-0.9.8/python_search/interpreter/group.py
--rw-r--r--   0        0        0     3901 2022-10-01 09:12:26.674717 python_search-0.9.8/python_search/interpreter/interpreter_matcher.py
--rw-r--r--   0        0        0      594 2022-10-01 09:12:26.674785 python_search-0.9.8/python_search/interpreter/python.py
--rw-r--r--   0        0        0      836 2022-11-02 18:06:13.948755 python_search-0.9.8/python_search/interpreter/snippet.py
--rw-r--r--   0        0        0     1278 2022-12-23 14:47:49.493163 python_search-0.9.8/python_search/interpreter/url.py
--rw-r--r--   0        0        0     1579 2022-12-23 14:47:49.493376 python_search-0.9.8/python_search/logger.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.675154 python_search-0.9.8/python_search/plugins/__init__.py
--rw-r--r--   0        0        0     1550 2022-12-23 14:47:49.493553 python_search-0.9.8/python_search/plugins/reminders.py
--rw-r--r--   0        0        0        0 2022-11-11 11:09:52.505942 python_search-0.9.8/python_search/sdk/__init__.py
--rw-r--r--   0        0        0     1205 2022-12-23 14:47:49.493837 python_search-0.9.8/python_search/sdk/web_api_sdk.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.675279 python_search-0.9.8/python_search/search/__init__.py
--rw-r--r--   0        0        0      357 2022-10-01 09:12:26.675351 python_search-0.9.8/python_search/search/entries_loader.py
--rw-r--r--   0        0        0     2440 2022-12-23 14:47:49.494021 python_search-0.9.8/python_search/search/models.py
--rw-r--r--   0        0        0       72 2022-10-01 09:12:26.675558 python_search-0.9.8/python_search/search/next_item_predictor/README.md
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.675585 python_search-0.9.8/python_search/search/next_item_predictor/__init__.py
--rw-r--r--   0        0        0     1738 2022-11-11 11:59:09.034649 python_search-0.9.8/python_search/search/next_item_predictor/evaluator.py
--rw-r--r--   0        0        0        0 2022-10-17 16:59:43.849988 python_search-0.9.8/python_search/search/next_item_predictor/features/__init__.py
--rw-r--r--   0        0        0     2587 2022-12-13 21:04:16.725181 python_search-0.9.8/python_search/search/next_item_predictor/features/entry_embeddings/__init__.py
--rwxr-xr-x   0        0        0     4147 2022-11-10 21:59:16.817461 python_search-0.9.8/python_search/search/next_item_predictor/features/entry_embeddings/entry_embeddings.py
--rw-r--r--   0        0        0      863 2022-12-13 21:33:35.031081 python_search-0.9.8/python_search/search/next_item_predictor/features/times_used.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.675810 python_search-0.9.8/python_search/search/next_item_predictor/inference/__init__.py
--rw-r--r--   0        0        0     3127 2022-12-30 09:22:40.360128 python_search-0.9.8/python_search/search/next_item_predictor/inference/inference.py
--rw-r--r--   0        0        0     2016 2022-11-11 11:59:09.045220 python_search-0.9.8/python_search/search/next_item_predictor/inference/input.py
--rw-r--r--   0        0        0      296 2022-10-25 11:43:14.088968 python_search-0.9.8/python_search/search/next_item_predictor/inference/label.py
--rw-r--r--   0        0        0      598 2022-11-18 11:12:19.472903 python_search-0.9.8/python_search/search/next_item_predictor/mlflow_logger.py
--rwxr-xr-x   0        0        0     4013 2022-12-30 09:15:26.315291 python_search-0.9.8/python_search/search/next_item_predictor/next_item_pipeline.py
--rw-r--r--   0        0        0     2639 2022-11-11 11:59:09.086652 python_search-0.9.8/python_search/search/next_item_predictor/offline_evaluation.py
--rw-r--r--   0        0        0     2169 2022-11-03 12:18:07.400405 python_search-0.9.8/python_search/search/next_item_predictor/train_keras.py
--rw-r--r--   0        0        0     1690 2022-10-25 11:43:14.126549 python_search-0.9.8/python_search/search/next_item_predictor/train_xgboost.py
--rw-r--r--   0        0        0    10352 2022-12-13 21:33:35.031271 python_search-0.9.8/python_search/search/next_item_predictor/training_dataset.py
--rw-r--r--   0        0        0     5496 2022-12-13 21:04:16.726745 python_search-0.9.8/python_search/search/next_item_predictor/transform.py
--rw-r--r--   0        0        0      450 2022-12-13 21:04:16.727305 python_search-0.9.8/python_search/search/ranked_entries.py
--rw-r--r--   0        0        0     3200 2022-12-23 14:47:49.494174 python_search-0.9.8/python_search/search/results.py
--rw-r--r--   0        0        0     5014 2022-12-23 14:47:49.494336 python_search-0.9.8/python_search/search/search.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.676707 python_search-0.9.8/python_search/search_ui/__init__.py
--rw-r--r--   0        0        0     5065 2022-12-29 19:37:32.445636 python_search-0.9.8/python_search/search_ui/fzf_kitty.py
--rw-r--r--   0        0        0     4123 2022-12-23 14:47:49.494790 python_search-0.9.8/python_search/search_ui/preview.py
--rw-r--r--   0        0        0      529 2022-12-23 14:47:49.494936 python_search-0.9.8/python_search/search_ui/serialized_entry.py
--rw-r--r--   0        0        0        0 2022-10-01 09:12:26.676934 python_search-0.9.8/python_search/shortcut/__init__.py
--rw-r--r--   0        0        0      875 2023-01-03 08:38:42.077071 python_search-0.9.8/python_search/shortcut/generator.py
--rwxr-xr-x   0        0        0     3747 2022-10-01 09:12:26.677065 python_search-0.9.8/python_search/shortcut/gnome.py
--rw-r--r--   0        0        0     1901 2022-11-11 11:59:09.070328 python_search-0.9.8/python_search/shortcut/i3.py
--rw-r--r--   0        0        0     3264 2023-01-03 12:32:01.345559 python_search-0.9.8/python_search/shortcut/mac.py
--rw-r--r--   0        0        0     5394 2022-10-01 09:12:26.677239 python_search-0.9.8/python_search/shortcuts.py
--rw-r--r--   0        0        0     3479 2022-12-23 14:47:49.495128 python_search-0.9.8/python_search/web_api.py
--rwxr-xr-x   0        0        0      742 2022-12-28 12:54:18.307265 python_search-0.9.8/wrap_log_command.sh
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 python_search-0.9.8/setup.py
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 python_search-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11398 2023-01-12 08:40:19.386972 python_search-0.9.9/LICENSE
+-rw-r--r--   0        0        0     3036 2023-01-12 08:40:19.386972 python_search-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     8196 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/.DS_Store
+-rw-r--r--   0        0        0       15 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/__init__.py
+-rw-r--r--   0        0        0      251 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/acronyms.py
+-rw-r--r--   0        0        0       59 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/README.md
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/__init__.py
+-rwxr-xr-x   0        0        0      112 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/apps.py
+-rw-r--r--   0        0        0     1146 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/browser.py
+-rw-r--r--   0        0        0     1941 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/clipboard.py
+-rw-r--r--   0        0        0     1913 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/collect_input.py
+-rw-r--r--   0        0        0      457 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/notification_ui.py
+-rw-r--r--   0        0        0     1428 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/terminal.py
+-rw-r--r--   0        0        0     1696 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/apps/window_manager.py
+-rw-r--r--   0        0        0     1128 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/chat_gpt.py
+-rw-r--r--   0        0        0     6954 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/cli.py
+-rw-r--r--   0        0        0     1682 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/config.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/configuration/__init__.py
+-rw-r--r--   0        0        0     3176 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/configuration/configuration.py
+-rw-r--r--   0        0        0     1795 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/configuration/loader.py
+-rwxr-xr-x   0        0        0     3875 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/container.py
+-rw-r--r--   0        0        0     1338 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/context.py
+-rw-r--r--   0        0        0     1826 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/core_entities.py
+-rw-r--r--   0        0        0     1623 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_collector.py
+-rw-r--r--   0        0        0     1601 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_exporter.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_ui/__init__.py
+-rw-r--r--   0        0        0     1403 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_ui/app_functions.py
+-rw-r--r--   0        0        0     2896 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_ui/entries_page.py
+-rw-r--r--   0        0        0     1465 2023-01-12 08:40:19.386972 python_search-0.9.9/python_search/data_ui/main.py
+-rw-r--r--   0        0        0     3112 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/data_ui/results_page.py
+-rw-r--r--   0        0        0      528 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/data_ui/training_page.py
+-rw-r--r--   0        0        0     2165 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entries_group.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/__init__.py
+-rw-r--r--   0        0        0     2830 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/edit_content.py
+-rw-r--r--   0        0        0     6859 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/entry_inserter_gui.py
+-rw-r--r--   0        0        0     3119 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/filesystem_entry_inserter.py
+-rw-r--r--   0        0        0     4116 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/register_new.py
+-rw-r--r--   0        0        0      881 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_capture/ui.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_description_generator/__init__.py
+-rw-r--r--   0        0        0     2196 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_description_generator/description_geneartor.py
+-rw-r--r--   0        0        0     4380 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_description_generator/pipeline.py
+-rw-r--r--   0        0        0     4493 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_runner.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_type/__init__.py
+-rw-r--r--   0        0        0     3711 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_type/classifier_inference.py
+-rw-r--r--   0        0        0     1179 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_type/entity.py
+-rw-r--r--   0        0        0     6886 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/entry_type/entry_type_pipeline.py
+-rw-r--r--   0        0        0       76 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/environment.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/__init__.py
+-rwxr-xr-x   0        0        0      822 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/latest_used_entries.py
+-rw-r--r--   0        0        0     1448 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/ranking_generated/__init__.py
+-rw-r--r--   0        0        0      103 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/run_performed/__init__.py
+-rw-r--r--   0        0        0     1616 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/run_performed/clean.py
+-rw-r--r--   0        0        0     1959 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/run_performed/dataset.py
+-rw-r--r--   0        0        0      699 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/run_performed/entity.py
+-rw-r--r--   0        0        0      854 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/events/run_performed/writer.py
+-rw-r--r--   0        0        0     1568 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/exceptions.py
+-rw-r--r--   0        0        0     1292 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/feature_toggle.py
+-rw-r--r--   0        0        0      977 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/features.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/infrastructure/__init__.py
+-rw-r--r--   0        0        0     1297 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/infrastructure/arize.py
+-rwxr-xr-x   0        0        0     3473 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/infrastructure/infrastructure.py
+-rw-r--r--   0        0        0      791 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/infrastructure/performance.py
+-rw-r--r--   0        0        0      437 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/infrastructure/redis.py
+-rwxr-xr-x   0        0        0     2367 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/init/entries_main.py
+-rw-r--r--   0        0        0     1531 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/init/install_dependencies.py
+-rw-r--r--   0        0        0     1464 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/init/project.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/__init__.py
+-rw-r--r--   0        0        0     3145 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/base.py
+-rw-r--r--   0        0        0     3530 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/cmd.py
+-rw-r--r--   0        0        0     1982 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/file.py
+-rw-r--r--   0        0        0      978 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/group.py
+-rw-r--r--   0        0        0     4225 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/interpreter_matcher.py
+-rw-r--r--   0        0        0      594 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/python.py
+-rw-r--r--   0        0        0      836 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/snippet.py
+-rw-r--r--   0        0        0     1278 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/interpreter/url.py
+-rw-r--r--   0        0        0     1900 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/logger.py
+-rw-r--r--   0        0        0       72 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/README.md
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/__init__.py
+-rw-r--r--   0        0        0     1738 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/evaluator.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/features/__init__.py
+-rw-r--r--   0        0        0     2580 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/features/entry_embeddings/__init__.py
+-rwxr-xr-x   0        0        0     4161 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/features/entry_embeddings/entry_embeddings.py
+-rw-r--r--   0        0        0      863 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/features/times_used.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/inference/__init__.py
+-rw-r--r--   0        0        0     2734 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/inference/inference.py
+-rw-r--r--   0        0        0     2009 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/inference/input.py
+-rw-r--r--   0        0        0      296 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/inference/label.py
+-rw-r--r--   0        0        0      598 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/mlflow_logger.py
+-rw-r--r--   0        0        0      705 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/model_interface.py
+-rw-r--r--   0        0        0     6032 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/next_item_model_v1.py
+-rw-r--r--   0        0        0     5849 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/next_item_model_v2.py
+-rwxr-xr-x   0        0        0     4027 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/next_item_pipeline.py
+-rw-r--r--   0        0        0     2800 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/offline_evaluation.py
+-rw-r--r--   0        0        0     2169 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/train_keras.py
+-rw-r--r--   0        0        0     1690 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/train_xgboost.py
+-rw-r--r--   0        0        0    10338 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/next_item_predictor/training_dataset.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/plugins/__init__.py
+-rw-r--r--   0        0        0     1617 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/plugins/reminders.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/sdk/__init__.py
+-rw-r--r--   0        0        0     1205 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/sdk/web_api_sdk.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/__init__.py
+-rw-r--r--   0        0        0      371 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/entries_loader.py
+-rw-r--r--   0        0        0     2440 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/models.py
+-rw-r--r--   0        0        0      450 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/ranked_entries.py
+-rw-r--r--   0        0        0     3376 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/results.py
+-rw-r--r--   0        0        0     4919 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search/search.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search_ui/__init__.py
+-rw-r--r--   0        0        0     5045 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search_ui/fzf_kitty.py
+-rw-r--r--   0        0        0     4583 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search_ui/preview.py
+-rw-r--r--   0        0        0      526 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/search_ui/serialized_entry.py
+-rw-r--r--   0        0        0        0 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcut/__init__.py
+-rw-r--r--   0        0        0      875 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcut/generator.py
+-rwxr-xr-x   0        0        0     3747 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcut/gnome.py
+-rw-r--r--   0        0        0     1901 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcut/i3.py
+-rw-r--r--   0        0        0     3264 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcut/mac.py
+-rw-r--r--   0        0        0     5394 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/shortcuts.py
+-rw-r--r--   0        0        0     3365 2023-01-12 08:40:19.390972 python_search-0.9.9/python_search/web_api.py
+-rwxr-xr-x   0        0        0      742 2023-01-12 08:40:19.394972 python_search-0.9.9/wrap_log_command.sh
+-rw-r--r--   0        0        0     3814 1970-01-01 00:00:00.000000 python_search-0.9.9/setup.py
+-rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 python_search-0.9.9/PKG-INFO
```

### Comparing `python_search-0.9.8/LICENSE` & `python_search-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/pyproject.toml` & `python_search-0.9.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-search"
-version = "0.9.8"
+version = "0.9.9"
 
 description = "Build your knowledge database in python and retrieve it efficiently"
 authors = ["Jean Carlo Machado <machado.c.jean@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 fire = "^0.4.0"
@@ -46,15 +46,16 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 python_search = 'python_search.cli:main'
-next_item_pipeline = 'python_search.search.next_item_predictor.next_item_pipeline:main'
+next_item_pipeline = 'python_search.next_item_predictor.next_item_pipeline:main'
+next_item = 'python_search.next_item_predictor.next_item_pipeline:main'
 collect_input = 'python_search.apps.collect_input:main'
 clipboard = 'python_search.apps.clipboard:main'
 notify_send = 'python_search.apps.notification_ui:main'
 python_search_infra = 'python_search.infrastructure.infrastructure:main'
 browser = 'python_search.apps.browser:main'
 python_search_webapi = 'python_search.web_api:main'
 run_entry = 'python_search.cli:_run_key_bin'
```

### Comparing `python_search-0.9.8/python_search/.DS_Store` & `python_search-0.9.9/python_search/.DS_Store`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/apps/browser.py` & `python_search-0.9.9/python_search/apps/browser.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/apps/clipboard.py` & `python_search-0.9.9/python_search/apps/clipboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             import sys
             content = sys.stdin.read()
 
         if not content:
             raise Exception("Tryring to set empty to clipboard")
 
         def shellquote(s):
-            return "'" + s.replace("'", "'\\''") + "'"
+            return "'" + s.replace("'", "\'") + "'"
 
         sanitized = shellquote(content)
 
         clipboard_cmd = "xsel --clipboard --primary --input"
         if is_mac():
             clipboard_cmd = "pbcopy"
```

### Comparing `python_search-0.9.8/python_search/apps/collect_input.py` & `python_search-0.9.9/python_search/apps/collect_input.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/apps/terminal.py` & `python_search-0.9.9/python_search/apps/terminal.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/apps/window_manager.py` & `python_search-0.9.9/python_search/apps/window_manager.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/cli.py` & `python_search-0.9.9/python_search/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
+from typing import Optional
 
 from python_search.apps.window_manager import WindowManager
-from python_search.config import ConfigurationLoader, PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
+from python_search.configuration.loader import ConfigurationLoader
+from python_search.core_entities import Key
 from python_search.entry_runner import EntryRunner
 from python_search.environment import is_mac
 from python_search.events.run_performed import RunPerformed
 from python_search.events.run_performed.writer import LogRunPerformedClient
 from python_search.search_ui.fzf_kitty import FzfInKitty
 from python_search.search_ui.preview import Preview
 from python_search.exceptions import notify_exception
@@ -20,15 +23,15 @@
 
     # all commands that are not self-explanatory should not be part of the main api, thus are marked as private.
 
     configuration: PythonSearchConfiguration
 
     @staticmethod
     def install_dependencies():
-        """install dependenceis"""
+        """install dependencies"""
         from python_search.init.install_dependencies import InstallDependencies
 
         InstallDependencies().install_all()
 
     @staticmethod
     def new_project(project_name: str):
         """Create a new project in the current directory with the given name"""
@@ -39,15 +42,15 @@
     @staticmethod
     def set_project_location(location: str):
         """For existing """
         from python_search.init.project import Project
 
         Project().set_current_project(location)
 
-    def __init__(self, configuration: PythonSearchConfiguration = None):
+    def __init__(self, configuration: Optional[PythonSearchConfiguration] = None):
         """
         Keep this constructor small and import dependencies inside the functions
         so they keep being fast
         """
         if not configuration:
             logging.debug("No _configuration provided, using default")
             try:
@@ -78,33 +81,32 @@
         """Starts the UI for collecting a new entry into pythonsearch"""
         from python_search.entry_capture.register_new import RegisterNew
 
         return RegisterNew(self.configuration)
 
     def edit_key(self, entry_str):
         """Opens the key in the source code using the IDE specified in the config, defaults to vim"""
-        from python_search.entry_capture.edit_content import EditKey
+        key = str(Key.from_fzf(entry_str))
 
-        result = EditKey(self.configuration).edit_key(entry_str, dry_run=False)
-        key = entry_str.split(":")[0]
+        from python_search.entry_capture.edit_content import EditKey
+        result = EditKey(self.configuration).edit_key(key, dry_run=False)
         LogRunPerformedClient().send(
             RunPerformed(key=key, query_input="", shortcut=False)
         )
         return result
 
     def _copy_entry_content(self, entry_str: str):
         """
         Copies the content of the provided key to the clipboard.
         Used by fzf to provide Ctrl-c functionality.
         """
         from python_search.interpreter.interpreter_matcher import InterpreterMatcher
+        key = str(Key.from_fzf(entry_str))
 
-        key = entry_str.split(":")[0]
         InterpreterMatcher.build_instance(self.configuration).clipboard(key)
-        print(f"Key: {key}")
         LogRunPerformedClient().send(
             RunPerformed(key=key, query_input="", shortcut=False)
         )
 
     def _copy_key_only(self, entry_str: str):
         """
         Copies to clipboard the key
@@ -171,18 +173,14 @@
 
     def _preview_entry(self, entry_text: str):
         """
         Recives entries from fzf and show them formatted for the preview window
         """
         Preview().display(entry_text)
 
-    def _infra_report(self):
-        from python_search.infrastructure.report import Report
-
-        return Report()
 
     def _entry_type_classifier(self):
 
         from python_search.entry_type.classifier_inference import (
             ClassifierInferenceClient,
         )
```

### Comparing `python_search-0.9.8/python_search/config.py` & `python_search-0.9.9/python_search/next_item_predictor/next_item_model_v2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,183 +1,159 @@
-"""
-Clients should depend on a configuration instance (config) rather than in the class,
-the class should only be used for type annotation.
-This way we can have multiple configs depending of the enviroment.
-"""
-import datetime
-import logging
-import os
-from typing import List, Optional, Tuple
-
-from python_search.entries_group import EntriesGroup
-from python_search.environment import is_mac
-from python_search.features import PythonSearchFeaturesSupport
-
-
-
-
-class DataConfig:
-    """
-    Configuration with locations of _entries, models and names of files.
-    """
-
-    # output of the _model
-    base_data_folder = f"{os.environ['HOME']}/.data/data/python_search"
-    BASE_DATA_COLLECTOR_FOLDER = f"{os.environ['HOME']}/.data/data_collection"
-    prediction_batch_location = base_data_folder + "/predict_input_lenght/latest"
-    # a copy of the search run _entries for the feature store
-    entries_dump = base_data_folder + "/entries_dumped/latest"
-    entries_dump_file = base_data_folder + "/entries_dumped/latest/000.parquet"
-    cached_configuration = "/tmp/search_and_run_configuration_cached"
-    # this path exists in the docker container but not necessarily in the host
-    MLFLOW_MODELS_PATH = f"/entries/mlflow"
-    BASELINE_EXPERIMENT_NAME = f"baseline_rank_v0"
-    NEXT_ITEM_EXPERIMENT_NAME = f"next_item_v1"
-    ENTRY_TYPE_CLASSIFIER_EXPERIMENT_NAME = f"entry_type_classifier_v2"
-    DATA_WAREHOUSE_FOLDER = base_data_folder + "/data_warehouse"
-    CLEAN_EVENTS_FOLDER = DATA_WAREHOUSE_FOLDER + "/clean"
-    SEARCH_RUNS_PERFORMED_FOLDER = (
-        base_data_folder + "/data_warehouse/dataframes/SearchRunPerformed"
-    )
-
-
-class MLFlowConfig:
-    port = 5002
-
-class KafkaConfig:
-    default_port: str = "9092"
-    host: str = f"127.0.0.1:{default_port}"
-
-
-class RedisConfig:
-    host = "127.0.0.1" if is_mac() else "host.docker.internal"
-    port = 6379
-
-
-class PythonSearchConfiguration(EntriesGroup):
-    """
-    The main _configuration of Python Search
-    Everything to customize about the application is configurable via code through this class
-    """
-
-    APPLICATION_TITLE = "PythonSearchWindow"
-    commands: dict
-    simple_gui_theme = "SystemDefault1"
-    simple_gui_font_size = 14
-    _default_tags = None
-    tags_dependent_inserter_marks = None
-    _initialization_time = None
-    _default_text_editor = "vim"
-
-    def __init__(
-        self,
-        *,
-        entries: Optional[dict] = None,
-        entries_groups: Optional[List[EntriesGroup]] = None,
-        supported_features: Optional[PythonSearchFeaturesSupport] = None,
-        default_tags=None,
-        tags_dependent_inserter_marks: Optional[dict[str, Tuple[str, str]]] = None,
-        default_text_editor: Optional[str] = None,
-    ):
-        """
-
-        :param entries:
-        :param entries_groups:
-        :param supported_features:
-        :param default_tags:
-        :param tags_dependent_inserter_marks:
-        :param default_text_editor:
-        """
-        if entries:
-            self.commands = entries
-
-        if entries_groups:
-            self.aggregate_commands(entries_groups)
-
-        if supported_features:
-            self.supported_features: PythonSearchFeaturesSupport = supported_features
-        else:
-            self.supported_features: PythonSearchFeaturesSupport = (
-                PythonSearchFeaturesSupport.default()
-            )
-
-        if default_tags:
-            self._default_tags = default_tags
-
-        self.tags_dependent_inserter_marks = tags_dependent_inserter_marks
-
+from typing import Tuple, Dict
 
-        self._initialization_time = datetime.datetime.now()
-        self._default_text_editor = default_text_editor
-
-
-    def get_text_editor(self):
-        return self._default_text_editor
+import numpy as np
+from pandas import DataFrame
+from pyspark.sql import Window
+
+from python_search.configuration.loader import ConfigurationLoader
+from python_search.search.models import PythonSearchMLFlow
+from python_search.next_item_predictor.features.entry_embeddings import InferenceEmbeddingsLoader
+from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import \
+    create_key_indexed_embedding
+from python_search.next_item_predictor.model_interface import ModelInterface
+
+
+class NextItemModelV2(ModelInterface):
+    PRODUCTION_RUN_ID = "07c37a94ccb64c0c8e1eca195ad910cb"
+
+    DIMENSIONS = 384 + 1
+
+    def __init__(self):
+        configuration = ConfigurationLoader().load_config()
+        self._all_keys = configuration.commands.keys()
+        self.inference_embeddings = InferenceEmbeddingsLoader(self._all_keys)
+
+    def build_dataset(self) -> DataFrame:
+        print("Building dataset v2")
+        from python_search.events.ranking_generated import RankingGeneratedDataset
+        import pyspark.sql.functions as F
+
+        rg = RankingGeneratedDataset().load()
+        rg = rg.withColumn("datetime", F.from_unixtime("timestamp"))
+
+        base_entries = rg.select(F.posexplode("ranking").alias('position', 'entry'), "uuid", 'datetime').select("entry",
+                                                                                                                "position",
+                                                                                                                "uuid",
+                                                                                                                "datetime")
+        base_entries = base_entries.withColumn('executed', F.lit(0))
+
+        # clean events
+        from python_search.events.run_performed.dataset import EntryExecutedDataset
+
+        performed_entries = EntryExecutedDataset().load_clean()
+        performed_entries = performed_entries.filter("rank_uuid IS NOT NULL and rank_position IS NOT NULL").select(
+            F.col("key").alias('entry'), F.col("rank_position").alias('position'), F.col("rank_uuid").alias('uuid'),
+            F.col("timestamp").alias('datetime'))
+
+        performed_entries = performed_entries.withColumn('executed', F.lit(1))
+        unioned = base_entries.union(performed_entries)
+        unioned = unioned.withColumn('timestamp', F.unix_timestamp('datetime'))
+        unioned = unioned.withColumnRenamed("executed", "label")
+        unioned = unioned.withColumnRenamed("entry", "key")
+
+
+        window = Window.orderBy(F.col("key"))
+        unioned = unioned.withColumn(
+            "entry_number", F.row_number().over(window)
+        )
+        dataset = unioned.select('entry_number', 'key', 'datetime', 'timestamp', 'position', 'label')
 
-    def get_default_tags(self):
-        return self._default_tags
+        dataset.show(n=10, truncate=False)
 
+        return dataset
 
-class ConfigurationLoader:
-    """
-    Loads the application from the environment.py
-    """
+    def transform_collection(
+            self, dataset: DataFrame
+    ) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        Returns X and Y
+        :param dataset:
+        :return:
+        """
 
-    def load_config(self) -> PythonSearchConfiguration:
+        embeddings_keys = self._create_embeddings_training_dataset(dataset)
+        # one extra for the row number
+        X = np.zeros([dataset.count(), self.DIMENSIONS + 1])
+        Y = np.empty(dataset.count())
+
+        collected_rows = dataset.collect()
+        #timestamp = dataset.select('timestamp').toPandas()['timestamp']
+        #normalized_timestamp = self._NormalizeData(timestamp)
+
+        for i, row in enumerate(collected_rows):
+            X[i] = np.concatenate(
+                [
+                    # adds entry number so we can index and select the right row afterwards
+                    # it gets deleted before training
+                    np.asarray([row.entry_number]),
+                    embeddings_keys[row.key],
+                    np.asarray([row.timestamp])
+                ]
+            )
 
-        folder = self.get_project_root()
-        config_location = f"{folder}/entries_main.py"
+            Y[i] = row.label
 
-        if not os.path.exists(config_location):
-            raise Exception(f"Could not find config file {config_location}")
+        X = np.where(np.isnan(X), 0.5, X)
+        Y = np.where(np.isnan(Y), 0.5, Y)
 
-        import sys
+        return X, Y
 
-        if folder not in sys.path:
-            sys.path.insert(0, folder)
-        import copy
-        from entries_main import config
+    def _NormalizeData(self, data):
+        """normalize a value between 0 and 1 """
+        return (data - np.min(data)) / (np.max(data) - np.min(data))
 
-        return copy.deepcopy(config)
+    def load_mlflow_model(self):
+        raise Exception("Not implemented")
 
-    def reload(self):
+    def transform_single(self, inference_input: dict) -> np.ndarray:
         """
-        reload _entries for when we change it
+        Return X
+        :param inference_input:
+        :return:
         """
-        import importlib
+        inference_input_obj = inference_input['inference_input']
+        all_keys = inference_input['all_keys']
+        from datetime import datetime;
+        timestamp = int(datetime.now().timestamp())
+        #timestamp_normalized = timestamp - 1669663110
+
+        X = np.zeros([len(all_keys), self.DIMENSIONS])
+        for i, key in enumerate(all_keys):
+            key_embedding = self.inference_embeddings.get_embedding_from_key(key)
+            if key_embedding is None:
+                continue
+
+            X[i] = np.concatenate(
+                (
+                    key_embedding,
+                    np.asarray([timestamp])
+                )
+            )
 
-        import entries_main
+        return X
 
-        importlib.reload(entries_main)
+    def load_mlflow_model(self, run_id=None):
+        model = PythonSearchMLFlow().get_next_predictor_model(run_id=run_id)
+        return model
 
-        import copy
+    def get_run_id(self):
+        return self.PRODUCTION_RUN_ID
 
-        import entries_main
 
-        return copy.deepcopy(entries_main.config)
+    def _create_embeddings_training_dataset(
+        self, dataset
+    ) -> Dict[str, np.ndarray]:
+        """
+        create embeddings with all training keys and keep them in memory
+        """
+        print("Creating embeddings of training dataset")
 
-    def get_project_root(self):
-        env_name = "PS_ENTRIES_HOME"
-        current_project_location = (
-            os.environ["HOME"] + "/.config/python_search/current_project"
-        )
+        # add embeddings to the dataset
+        collected_keys = dataset.select("key").collect()
 
-        folder = None
+        all_keys = []
+        for collected_keys in collected_keys:
+            all_keys.append(collected_keys.key)
 
-        if env_name in os.environ:
-            logging.debug(
-                f"Env exists and takes precedence: {env_name}={os.environ[env_name]}"
-            )
-            folder = os.environ[env_name]
 
-        if os.path.isfile(current_project_location):
-            with open(current_project_location) as f:
-                folder = f.readlines()[0].strip()
-
-        if not folder:
-            raise Exception(
-                f"Either {current_project_location} or {env_name} must be set to find _entries"
-            )
-        return folder
 
-    def load_entries(self):
-        return self.load_config().commands
+        return create_key_indexed_embedding(all_keys)
```

### Comparing `python_search-0.9.8/python_search/container.py` & `python_search-0.9.9/python_search/container.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/usr/bin/env python3
 import os
+from typing import Optional
 
 from python_search.config import MLFlowConfig
 
 
 def build():
     result = os.system("docker build . -t ps:latest ")
     if result == 0:
@@ -13,15 +14,26 @@
 
 
 def build_and_run():
     build()
     run()
 
 
-def run(cmd="", entrypoint="", port="", restart=False, extra_env_vars=None):
+def run(cmd="", entrypoint="", port="", restart=False, extra_env_vars=None, name: Optional[str] = None):
+    """
+    Runs inside the docker container
+
+    :param cmd:
+    :param entrypoint:
+    :param port:
+    :param restart:
+    :param extra_env_vars:
+    :param name:
+    :return:
+    """
 
     if entrypoint:
         entrypoint = f" --entrypoint '{entrypoint}'"
 
     restart_exp = ""
     if restart:
         print("Adding restart flag")
@@ -49,19 +61,32 @@
         " -e PS_WEB_PASSWORD=$PS_WEB_PASSWORD",
     ]
 
     env_vars = env_vars + extra_env_vars if extra_env_vars else env_vars
 
     environment_variables = " ".join(env_vars)
 
+    name_expr = ""
+    if name:
+        name_expr = f" --name {name} "
+
     LIMIT_CPU = 8
-    cmd = f"docker run {port} {restart_exp} --expose=8000 --expose 4040 --expose 6380 --cpus={LIMIT_CPU} {environment_variables} -it {volumes} {entrypoint} ps {cmd}"
+    cmd = f"docker run {name_expr} {port} {restart_exp} --expose=8000 --expose 4040 --expose 6380 --cpus={LIMIT_CPU} {environment_variables} -it {volumes} {entrypoint} ps {cmd}"
     print("Cmd: " + cmd)
     os.system(cmd)
 
+def run_webserver():
+    name="python_search_webserver"
+    _stop_and_remove_by_name(name)
+
+    run(
+        cmd="python_search_webapi",
+        port="8000:8000",
+        name=name,
+    )
 
 def sh():
     shell()
 
 
 def shell():
     run(entrypoint="/bin/bash")
@@ -83,28 +108,23 @@
     run(
         cmd=f"mlflow ui --backend-store-uri file:/entries/mlflow --port {MLFlowConfig.port} --host '0.0.0.0' ",
         port=f"{MLFlowConfig.port}:{MLFlowConfig.port}",
         restart=restart,
     )
 
 
-def run_webserver(restart=False, force_restart=False):
-    if restart or force_restart:
-        _restart_by_port(8000)
-
-    run(
-        cmd="python_search_webapi",
-        port="8000:8000",
-        restart=restart,
-    )
 
 def _restart_by_port(port):
     print("Stopping previously running container")
     os.system(f"docker stop $(docker ps | grep -i {port} | cut -d ' ' -f1) ; sleep 3")
 
+def _stop_and_remove_by_name(name):
+    print("Stopping previously running container")
+    os.system(f"docker stop {name} ; docker rm {name}")
+
 def run_streamlit(restart=False, disable_password=False):
 
     if restart:
         _restart_by_port(8501)
 
     run(
         cmd="streamlit run python_search/data_ui/main.py --server.address=0.0.0.0  --server.port=8501",
```

### Comparing `python_search-0.9.8/python_search/context.py` & `python_search-0.9.9/python_search/context.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/core_entities.py` & `python_search-0.9.9/python_search/core_entities.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,28 @@
 
 """
 from __future__ import annotations
 
 from typing import List, Optional
 
 from numpy import ndarray
-from typed_pyspark import Dataframe
+
+class Key:
+    """ Represents a key of an entry """
+    def __init__(self, key):
+        self.key = key
+
+    @staticmethod
+    def from_fzf(entry_text: str) -> Key:
+        key = entry_text.split(":")[0] if ":" in entry_text else entry_text
+        key = key.strip()
+        return Key(key)
+
+    def __str__(self):
+        return self.key
 
 
 class Entry:
     """
     An python dictionary we write in PythonSearch
     """
 
@@ -59,14 +72,7 @@
     def from_entries_dict(dict: dict) -> InvertedIndex:
         instance = InvertedIndex()
         instance.entries = []
         for key, value in dict.items():
             instance.entries.append(Entry(name=key, value=value))
 
         return instance
-
-    def serialize(self) -> str:
-        pass
-
-
-Entries = Dataframe(schema={"key": "String", "position": "Integer"})
-EntriesType = Entries.type_annotation()
```

### Comparing `python_search-0.9.8/python_search/data_collector.py` & `python_search-0.9.9/python_search/data_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         import datetime
 
         file_name = f"{self.data_location(table_name)}/{datetime.datetime.now(datetime.timezone.utc).timestamp()}.json"
 
         with open(file_name, "w") as f:
             f.write(json.dumps(data))
 
-        self.logger.info(f"File {file_name} written successfully with data {data}")
+        #self.logger.info(f"File {file_name} written successfully with data {data}")
 
     def data_location(self, table_name) -> str:
         return f"{GenericDataCollector.BASE_DATA_DESTINATION_DIR}/{table_name}"
 
     def dataframe(self, table_name):
         from pyspark.sql import DataFrame
         from pyspark.sql.session import SparkSession
```

### Comparing `python_search-0.9.8/python_search/data_exporter.py` & `python_search-0.9.9/python_search/data_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.data_ui.entries_page import extract_value_from_entry
 
 
 class DataExporter:
     blacklisted_terms = [
         "http://",
         "https://",
```

### Comparing `python_search-0.9.8/python_search/data_ui/app_functions.py` & `python_search-0.9.9/python_search/data_ui/app_functions.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/data_ui/entries_page.py` & `python_search-0.9.9/python_search/data_ui/entries_page.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         result = str(entry["cmd"])
     if "cli_cmd" in entry:
         result = str(entry["cli_cmd"])
     return result
 
 
 def load_homepage():
-    from python_search.config import ConfigurationLoader
+    from python_search.configuration.loader import ConfigurationLoader
 
     entries = ConfigurationLoader().load_config().commands
 
     col1, col2, col3 = st.columns([1, 1, 1])
 
     with col1:
         if st.button("Sync current host"):
```

### Comparing `python_search-0.9.8/python_search/data_ui/main.py` & `python_search-0.9.9/python_search/data_ui/main.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/data_ui/results_page.py` & `python_search-0.9.9/python_search/data_ui/results_page.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 def load_results_page():
     import pandas as pd
     import streamlit as st
 
-    from python_search.config import ConfigurationLoader
+    from python_search.configuration.loader import ConfigurationLoader
 
     config = ConfigurationLoader().load_config()
 
     keys = config.commands.keys()
 
-    from python_search.search.next_item_predictor.inference.inference import Inference
-    from python_search.search.next_item_predictor.inference.input import ModelInput
+    from python_search.next_item_predictor import Inference
+    from python_search.next_item_predictor import ModelInput
 
     st.write("### Prediction results")
     st.write("##### Production run: " + Inference.PRODUCTION_RUN_ID)
 
     scenarios = {
         "work vs non work typical hours": {
             "a": {
```

### Comparing `python_search-0.9.8/python_search/data_ui/training_page.py` & `python_search-0.9.9/python_search/data_ui/training_page.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import streamlit as st
 
-from python_search.search.next_item_predictor.training_dataset import TrainingDataset
+from python_search.next_item_predictor import TrainingDataset
 
 
 def load_training_page():
     st.write("## Training Dataset")
 
     df = load_dataset()
     pdf = df.toPandas()
```

### Comparing `python_search-0.9.8/python_search/entries_group.py` & `python_search-0.9.9/python_search/entries_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,10 +68,10 @@
         return sys.argv[0]
 
     def get_project_root(self):
         """
         @ deprecated use environment loader instead
         """
 
-        from python_search.config import ConfigurationLoader
+        from python_search.configuration.loader import ConfigurationLoader
 
         return ConfigurationLoader().get_project_root()
```

### Comparing `python_search-0.9.8/python_search/entry_capture/edit_content.py` & `python_search-0.9.9/python_search/entry_capture/edit_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,28 @@
     """
     Set of commands to edit the _entries
     """
 
     def __init__(self, configuration):
         self.configuration = configuration
 
-    def edit_key(self, key, dry_run=False):
+    def edit_key(self, key: str, dry_run=False):
         """
         Edits the _configuration files by searching the text
         """
         print(f"Editing key {key}")
         if not key:
             self.edit_default()
             return
 
-        key = key.split(":")
-
         if not len(key):
+            print('Editing default')
             self.edit_default()
             return
 
-        key = key[0]
         # needs to be case insensitive search
         cmd = f"ack -i '{key}' {self.configuration.get_project_root()} --py || true"
         logging.info(f"Command: {cmd}")
         result_shell = subprocess.check_output(cmd, shell=True, text=True)
 
         if not result_shell:
             logging.info("Could not find match edit main file")
```

### Comparing `python_search-0.9.8/python_search/entry_capture/entry_inserter_gui.py` & `python_search-0.9.9/python_search/entry_capture/entry_inserter_gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,31 @@
 import logging
 import threading
 from dataclasses import dataclass
 from typing import List
 
 import fire
 
-from python_search.config import ConfigurationLoader
+from python_search.chat_gpt import ChatGPT
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.entry_type.classifier_inference import ClassifierInferenceClient
 from python_search.infrastructure.arize import Arize
+from python_search.interpreter.interpreter_matcher import InterpreterMatcher
 from python_search.sdk.web_api_sdk import PythonSearchWebAPISDK
 
 
 class EntryCaptureGUI:
     def __init__(self):
         self._configuration = ConfigurationLoader().load_config()
         self._tags = self._configuration._default_tags
         self._prediction_uuid = None
 
     def launch(
         self,
-        title: str = "Capture Entry",
+        title: str = "New Entry",
         default_key: str = "",
         default_content: str = "",
         serialize_output=False,
         default_type="Snippet",
     ) -> GuiEntryData:
         """
         Launch the _entries capture GUI.
@@ -36,113 +38,125 @@
 
         self._sg = sg
 
         config = ConfigurationLoader().load_config()
         sg.theme(config.simple_gui_theme)
         font_size = config.simple_gui_font_size
 
-        content_input = sg.Input(
-            key="content",
-            default_text=default_content,
-            expand_x=True,
-            expand_y=True,
-        )
         entry_type = sg.Combo(
             [
                 "Snippet",
                 "Cmd",
                 "Url",
                 "File",
                 "Anonymous",
             ],
             key="type",
             default_value=default_type,
         )
 
         tags_chucks = self._chunks_of_tags(self._tags, 4)
+
+        if not default_key:
+            default_key = self.genearte_key_from_content(default_content)
+
+        key_name_input = sg.Input(
+            key="key", default_text=default_key, expand_x=True, expand_y=True,
+            size=(15, 1),
+        )
+
+
+        content_input = sg.Multiline(
+            key="content",
+            default_text=default_content,
+            expand_x=True,
+            expand_y=True,
+            no_scrollbar=False,
+            size=(15, 7),
+        )
         layout = [
-            [sg.Text("Entry content")],
-            [content_input],
-            [sg.Text("Descriptive key name")],
+            [sg.Text("Key name")],
             [
-                sg.Input(
-                    key="key", default_text=default_key, expand_x=True, expand_y=True
-                )
+                key_name_input
             ],
+            [sg.Text("Entry content")],
+            [content_input],
+            [sg.Text("Generator"), sg.Button("Content", key="-generate-body-"), sg.Button("Title", key="-generate-title-")],
             [sg.Text("Type")],
-            [entry_type],
+            [entry_type, sg.Button("Try it", key="-try-entry-")],
             [sg.Text("Tags")],
             [self._checkbox_list(i) for i in tags_chucks],
             [sg.Button("Write", key="write")],
         ]
 
         window = sg.Window(
             title,
             layout,
             font=("Helvetica", font_size),
             finalize=True,
         )
 
         # workaround for mac bug
 
-        content_input.update(select=True)
 
         window["key"].bind("<Return>", "_Enter")
         window["content"].bind("<Return>", "_Enter")
         window["type"].bind("<Return>", "_Enter")
         window["key"].bind("<Escape>", "_Esc")
         window["content"].bind("<Escape>", "_Esc")
         window["type"].bind("<Escape>", "_Esc")
 
         threading.Thread(
             target=self._predict_entry_type, args=(window, default_content), daemon=True
         ).start()
 
-        if not default_key:
-            threading.Thread(
-                target=self._generate_description,
-                args=(window, default_content),
-                daemon=True,
-            ).start()
-
         while True:
             event, values = window.read()
+            if event and (event == "-generate-body-"):
+                window['content'].update(ChatGPT().answer(values['key']))
+
+            if event and (event == "-generate-title-"):
+                window['key'].update(self.genearte_key_from_content(values['content']))
+
             if event and (event == "write" or event.endswith("_Enter")):
                 break
 
             if event == "-type-inference-ready-":
                 window["type"].update(values[event])
                 continue
 
-            if event == "-generated-key-ready-":
-                window["key"].update(values[event])
-                continue
+            if event == "-try-entry-":
+               InterpreterMatcher.build_instance(self._configuration).get_interpreter_from_type(values['type'])(values['content']).default()
 
             if event == sg.WINDOW_CLOSED or event.endswith("_Esc"):
                 raise Exception("Quitting window")
 
+        window.hide()
         window.close()
         logging.info("values", values)
 
         selected_tags = []
         for key, value in values.items():
             if key in self._tags and value == True:
                 selected_tags.append(key)
 
         result = GuiEntryData(
             values["key"], values["content"], values["type"], selected_tags
         )
 
-        self._report_actual(result)
+        #self._report_actual(result)
 
         if serialize_output:
             result = result.__dict__
 
         return result
 
+    def genearte_key_from_content(self, content: str) -> str:
+        return ChatGPT().answer("generate a description in the imperative form with most 5 words of the follwing text: " + content)
+
     def _report_actual(self, data: GuiEntryData):
         if not self._prediction_uuid:
             print("No prediction uuid, skipping report")
             return
 
         if not Arize.is_installed():
             return
```

### Comparing `python_search-0.9.8/python_search/entry_capture/filesystem_entry_inserter.py` & `python_search-0.9.9/python_search/entry_capture/filesystem_entry_inserter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import shutil
 from datetime import datetime
 
-from python_search.config import PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
 from python_search.events.run_performed import RunPerformed
 
 
 class FilesystemEntryInserter:
     """
     Class responsible to the actual writing of the new entry in the filesystem
     """
```

### Comparing `python_search-0.9.8/python_search/entry_capture/register_new.py` & `python_search-0.9.9/python_search/entry_capture/register_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import datetime
 import time
+from typing import Optional
 
 from python_search.apps.clipboard import Clipboard
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.entry_capture.filesystem_entry_inserter import (
     FilesystemEntryInserter,
 )
 from python_search.entry_capture.entry_inserter_gui import EntryCaptureGUI, GuiEntryData
 from python_search.entry_type.entity import infer_default_type
 from python_search.exceptions import RegisterNewException
 from python_search.interpreter.base import BaseInterpreter
@@ -26,15 +27,15 @@
         if not configuration:
             configuration = ConfigurationLoader().load_config()
 
         self.configuration = configuration
         self.entry_inserter = FilesystemEntryInserter(configuration)
 
     @notify_exception()
-    def register(self, *, key: str, value: str, tag: str = None):
+    def register(self, *, key: str, value: str, tag: Optional[str] = None):
         """
         The non ui driven registering api
         Args:
             key:
             value:
             tag:
 
@@ -66,15 +67,15 @@
             default_content = Clipboard().get_content()
 
         # @todo reenable this once in the dockerfile
         if not default_type:
             default_type = infer_default_type(default_content)
 
         entry_data: GuiEntryData = EntryCaptureGUI().launch(
-            "New Entry Details",
+            "New Entry",
             default_content=default_content,
             default_key=default_key,
             default_type=default_type,
         )
         key = self._sanitize_key(entry_data.key)
         interpreter: BaseInterpreter = InterpreterMatcher.build_instance(
             self.configuration
```

### Comparing `python_search-0.9.8/python_search/entry_capture/ui.py` & `python_search-0.9.9/python_search/entry_capture/ui.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/entry_description_generator/description_geneartor.py` & `python_search-0.9.9/python_search/entry_description_generator/description_geneartor.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/entry_description_generator/pipeline.py` & `python_search-0.9.9/python_search/entry_description_generator/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Tuple
 import random
 import sys
 import numpy as np
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from keras import layers
 import keras
-from python_search.search.next_item_predictor.mlflow_logger import configure_mlflow
+from python_search.next_item_predictor import configure_mlflow
 
 
 def extract_string_from_entries(entries) -> List[str]:
     X = []
     for key, entry in entries.items():
         if "url" in entry:
             item = str(entry["url"])
```

### Comparing `python_search-0.9.8/python_search/entry_runner.py` & `python_search-0.9.9/python_search/entry_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import re
+import os
 from typing import List
 
 from python_search.apps.notification_ui import send_notification
-from python_search.config import PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
 from python_search.context import Context
+from python_search.core_entities import Key
 from python_search.events.run_performed import RunPerformed
 from python_search.events.run_performed.writer import LogRunPerformedClient
 from python_search.interpreter.cmd import CmdInterpreter
 from python_search.interpreter.interpreter_matcher import InterpreterMatcher
-from python_search.logger import setup_run_key_logger, StreamToLogger
+from python_search.logger import setup_run_key_logger
 from python_search.exceptions import notify_exception
 from python_search.search_ui.serialized_entry import (
     decode_serialized_data_from_entry_text,
 )
 
 logger = setup_run_key_logger()
 
@@ -31,24 +33,26 @@
     def run(
         self,
         entry_text: str,
         query_used: str = "",
         force_gui_mode=False,
         gui_mode=False,
         from_shortcut=False,
+        fzf_pid_to_kill = None
     ):
         """
         Runs an entry given its name or its partial name.
 
         Parameters:
             key: As it comes from FZF they is a str pair of key_name : {metadata}
             entry_rank_position: accounts for where the entry was when it was executed, if passed it will be used for
             from_shortcut means that the key execution was triggered by a desktop shortcut
         """
-        key = entry_text.split(":")[0] if ":" in entry_text else entry_text
+
+        key = str(Key.from_fzf(entry_text))
 
         logger.info("Arrived at run key")
         # if there are : in the line just take all before it as it is
         # usually the key from fzf, and our keys do not accept :
 
         if from_shortcut:
             send_notification(f"{key}")
@@ -75,34 +79,41 @@
             Rank Position: {rank_position}
         """
         )
 
         if force_gui_mode or gui_mode:
             Context.get_instance().enable_gui_mode()
 
-        real_key: str = matches[0]
+
 
         if len(matches) > 1:
-            real_key = min(matches, key=len)
+            key = min(matches, key=len)
             send_notification(
                 f"Multiple matches for this key {matches} using the smaller"
             )
 
-        result = InterpreterMatcher.build_instance(self.configuration).default(real_key)
+        result = InterpreterMatcher.build_instance(self.configuration).default(key)
+
 
         logger.info("Passed interpreter")
         run_performed = RunPerformed(
             key=key,
             query_input=query_used,
             shortcut=from_shortcut,
             rank_uuid=metadata.get("uuid"),
             rank_position=metadata.get("position"),
         )
         logger.info(f"Run performed = {run_performed}")
         LogRunPerformedClient().send(run_performed)
+
+        # this needs to be last as it will kill the process
+        if fzf_pid_to_kill:
+            print("Killing fzf")
+            os.system(f"kill -9 {fzf_pid_to_kill}")
+
         return result
 
     def _matching_keys(self, key: str) -> List[str]:
         """
         give a key it will give suggestions that matches
         """
```

### Comparing `python_search-0.9.8/python_search/entry_type/classifier_inference.py` & `python_search-0.9.9/python_search/entry_type/classifier_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ) -> Tuple[EntryType, PredictionUuid]:
 
         from python_search.search.models import PythonSearchMLFlow
 
         model = PythonSearchMLFlow().get_entry_type_classifier(
             run_id=PredictEntryTypeInference.PRODUCTION_RUN_ID
         )
-        from python_search.search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
+        from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
             create_embeddings_from_strings,
         )
 
         data = create_embeddings_from_strings([entry_data.content])
 
         from python_search.entry_type.entry_type_pipeline import Pipeline
```

### Comparing `python_search-0.9.8/python_search/entry_type/entity.py` & `python_search-0.9.9/python_search/entry_type/entity.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/entry_type/entry_type_pipeline.py` & `python_search-0.9.9/python_search/entry_type/entry_type_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import uuid
 
 
 from python_search.entry_type.classifier_inference import get_value_and_label
 from python_search.entry_type.entity import EntryType
-from python_search.config import ConfigurationLoader, DataConfig
+from python_search.config import DataConfig
+from python_search.configuration.loader import ConfigurationLoader
 import pandas as pd
 import matplotlib.pyplot as plt
 
 from python_search.infrastructure.arize import Arize
-from python_search.search.next_item_predictor.mlflow_logger import configure_mlflow
-from python_search.search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
+from python_search.next_item_predictor import configure_mlflow
+from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
     create_embeddings_from_strings,
 )
 import os
 import numpy as np
 from keras import models
 from keras import layers
 from keras.utils.np_utils import to_categorical
```

### Comparing `python_search-0.9.8/python_search/events/latest_used_entries.py` & `python_search-0.9.9/python_search/events/latest_used_entries.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/events/ranking_generated/__init__.py` & `python_search-0.9.9/python_search/events/ranking_generated/__init__.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/events/run_performed/clean.py` & `python_search-0.9.9/python_search/events/run_performed/clean.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/events/run_performed/dataset.py` & `python_search-0.9.9/python_search/events/run_performed/dataset.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/events/run_performed/entity.py` & `python_search-0.9.9/python_search/events/run_performed/entity.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/events/run_performed/writer.py` & `python_search-0.9.9/python_search/events/run_performed/writer.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/exceptions.py` & `python_search-0.9.9/python_search/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/feature_toggle.py` & `python_search-0.9.9/python_search/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/features.py` & `python_search-0.9.9/python_search/features.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/infrastructure/arize.py` & `python_search-0.9.9/python_search/infrastructure/arize.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/infrastructure/infrastructure.py` & `python_search-0.9.9/python_search/infrastructure/infrastructure.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/infrastructure/performance.py` & `python_search-0.9.9/python_search/infrastructure/performance.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/init/entries_main.py` & `python_search-0.9.9/python_search/init/entries_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,11 +45,10 @@
     "help python search manual": {"cli_cmd": "python_search --help"},
     **{
         f"get pods for {env}": {"cli_cmd": f"kubectl --context {env} get pods"}
         for env in ["production", "testing", "development"]
     },
 }
 
-
-from python_search.config import PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
 
 config = PythonSearchConfiguration(entries=entries)
```

### Comparing `python_search-0.9.8/python_search/init/install_dependencies.py` & `python_search-0.9.9/python_search/init/install_dependencies.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/init/project.py` & `python_search-0.9.9/python_search/init/project.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/base.py` & `python_search-0.9.9/python_search/interpreter/base.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/cmd.py` & `python_search-0.9.9/python_search/interpreter/cmd.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/file.py` & `python_search-0.9.9/python_search/interpreter/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from python_search.interpreter.base import BaseInterpreter
 from python_search.interpreter.cmd import CmdInterpreter
 
 
 class FileInterpreter(BaseInterpreter):
     def __init__(self, cmd: Any, context: Context = None):
         self.context = context
-        self.cmd = {}
+        self.cmd = cmd
 
         if type(cmd) == str:
             self.cmd = {"file": cmd}
-            return
 
-        if type(cmd) is dict and "file" in cmd:
-            self.cmd = cmd
-            return
+        if type(cmd) == dict and "file" not in cmd:
+            raise CommandDoNotMatchException(
+                f"Not Valid {self.__class__.__name__} command {cmd}"
+            )
 
-        if type(cmd) is str and FileInterpreter.file_exists(cmd):
-            self.cmd["file"] = cmd
+        print(cmd)
+        if FileInterpreter.file_exists(self.cmd['file']):
             return
 
         raise CommandDoNotMatchException(
             f"Not Valid {self.__class__.__name__} command {cmd}"
         )
 
     def get_executable(self):
```

### Comparing `python_search-0.9.8/python_search/interpreter/group.py` & `python_search-0.9.9/python_search/interpreter/group.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/interpreter_matcher.py` & `python_search-0.9.9/python_search/interpreter/interpreter_matcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-import logging
 import re
 
 from python_search.context import Context
 from python_search.exceptions import CommandDoNotMatchException
 from python_search.interpreter.base import BaseInterpreter
 from python_search.interpreter.cmd import CmdInterpreter
 from python_search.interpreter.file import FileInterpreter
 from python_search.interpreter.group import GroupInterpreter
 from python_search.interpreter.python import PythonInterpreter
 from python_search.interpreter.snippet import SnippetInterpreter
 from python_search.interpreter.url import UrlInterpreter
+from python_search.logger import interpreter_logger
 
 INTERPRETERS_IN_ORDER = [
     UrlInterpreter,
     FileInterpreter,
     GroupInterpreter,
     SnippetInterpreter,
     PythonInterpreter,
     CmdInterpreter,
 ]
 
-
 class InterpreterMatcher:
     """
     Matches a query with an entry interpreter
     """
 
     _instance = None
 
     @staticmethod
-    def build_instance(configuration):
+    def build_instance(configuration) -> 'InterpreterMatcher':
         """
         Singleton. Initializes a _configuration a context and a interpreter
 
         :return:
         """
         if not InterpreterMatcher._instance:
             context = Context.get_instance()
@@ -42,32 +41,34 @@
         return InterpreterMatcher._instance
 
     def __init__(self, configuration, context: Context):
         self._configuration = configuration
         self.context = context
         self.context.set_interpreter(self)
         self._interpreters = INTERPRETERS_IN_ORDER
+        self.logger = interpreter_logger()
 
-    def get_interpreter(self, given_input: str) -> BaseInterpreter:
+    def get_interpreter(self, given_input: str, skip_key_matching=False) -> BaseInterpreter:
         """
         Given the string content, returns the best matched interpreter.
         Returns the instance of the matched interpreter given an text input
         """
         self.context.set_input(given_input)
 
-        try:
-            # tries to get the real key if it exists
-            key = self._get_key(given_input)
-            given_input = self._configuration.get_command(key)
-        except Exception as e:
-            logging.error(e)
+        if not skip_key_matching:
+            try:
+                # tries to get the real key if it exists
+                key = self._get_key(given_input)
+                given_input = self._configuration.get_command(key)
+            except Exception as e:
+                self.logger.error(e)
 
         return self._match_interpreter(given_input)
 
-    def get_interpreter_from_type(self, type: str):
+    def get_interpreter_from_type(self, type: str) -> BaseInterpreter:
         """
         From a type given in the ui via string returns the matching interpreter type
 
         """
 
         if type == "Snippet":
             return SnippetInterpreter
@@ -93,19 +94,21 @@
         return specific_interpreter.default()
 
     def clipboard(self, given_input: str):
         specific_interpreter: BaseInterpreter = self.get_interpreter(given_input)
         return specific_interpreter.interpret_clipboard()
 
     def _match_interpreter(self, cmd) -> BaseInterpreter:
+        self.logger.info("Matching interpreter for command: %s", cmd)
+        print("Matching interpreter for command: %s", cmd)
         for interpreter in self._interpreters:
             try:
-                logging.info(f"Trying to construct {interpreter}")
+                print(f"Trying to construct {interpreter}")
                 command_instance = interpreter(cmd, self.context)
-                logging.info(f"Matched command instance {command_instance}")
+                print(f"Matched command instance {command_instance}")
                 return command_instance
             except CommandDoNotMatchException as e:
                 pass
 
         raise Exception("Received a dict but did not match any type")
 
     def _get_key(self, given_input) -> str:
```

### Comparing `python_search-0.9.8/python_search/interpreter/python.py` & `python_search-0.9.9/python_search/interpreter/python.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/snippet.py` & `python_search-0.9.9/python_search/interpreter/snippet.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/interpreter/url.py` & `python_search-0.9.9/python_search/interpreter/url.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/logger.py` & `python_search-0.9.9/python_search/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     logger = logging.getLogger("inference")
     logger.setLevel(logging.DEBUG)
 
     # fh = logging.FileHandler("/tmp/inference.txt")
     # fh.setLevel(logging.DEBUG)
     # logger.addHandler(fh)
 
-    ch = logging.StreamHandler()
+    ch = logging.StreamHandler(sys.stdout)
     ch.setLevel(logging.INFO)
     logger.addHandler(ch)
 
     return logger
 
 
 def setup_preview_logger():
@@ -33,24 +33,34 @@
     logger = logging.getLogger("run-key")
     fh = logging.FileHandler("/tmp/run_key.txt")
     fh.setLevel(logging.DEBUG)
     logger.addHandler(fh)
 
     return logger
 
+def interpreter_logger():
+    logger = logging.getLogger("interpeter_logger")
+    ch = logging.StreamHandler(sys.stdout)
+    ch.setLevel(logging.INFO)
+    logger.addHandler(ch)
+    fh = logging.FileHandler(f"/tmp/debug_interpreter")
+    fh.setLevel(logging.INFO)
+    logger.addHandler(fh)
+    return logger
+
 
 def setup_data_writter_logger(event_name):
     logger = logging.getLogger(f"data-writer_{event_name}")
     logger.setLevel(logging.DEBUG)
     fh = logging.FileHandler(f"/tmp/data-writer_event_{event_name}")
     fh.setLevel(logging.DEBUG)
-    ch = logging.StreamHandler()
-    ch.setLevel(logging.INFO)
+    #ch = logging.StreamHandler()
+    #ch.setLevel(logging.INFO)
     logger.addHandler(fh)
-    logger.addHandler(ch)
+    #logger.addHandler(ch)
 
     return logger
 
 
 class StreamToLogger(object):
     """
     Fake file-like stream object that redirects writes to a logger instance.
```

### Comparing `python_search-0.9.8/python_search/plugins/reminders.py` & `python_search-0.9.9/python_search/plugins/reminders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import time
 
 
 from python_search.apps.notification_ui import send_notification
-from python_search.config import ConfigurationLoader, PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
+from python_search.configuration.loader import ConfigurationLoader
 
 
 def get_random():
     config: PythonSearchConfiguration = ConfigurationLoader().load_config()
     print("Running reminder job")
 
     all_entries = config.commands
```

### Comparing `python_search-0.9.8/python_search/sdk/web_api_sdk.py` & `python_search-0.9.9/python_search/sdk/web_api_sdk.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/models.py` & `python_search-0.9.9/python_search/search/models.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/evaluator.py` & `python_search-0.9.9/python_search/next_item_predictor/evaluator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import logging
 import sys
 
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.search.entries_loader import EntriesLoader
-from python_search.search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
+from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
     RedisEmbeddingsReader,
 )
-from python_search.search.next_item_predictor.inference.inference import Inference
+from python_search.next_item_predictor.inference.inference import Inference
 
 
 class Evaluate:
     """
     Central place to evaluate the quality of the _model
     """
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/features/entry_embeddings/__init__.py` & `python_search-0.9.9/python_search/next_item_predictor/features/entry_embeddings/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import copy
 
 from python_search.events.latest_used_entries import RecentKeys
-from python_search.search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
+from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
     EmbeddingSerialization,
     RedisEmbeddingsReader,
     RedisEmbeddingsWriter,
 )
 
 
 class InferenceEmbeddingsLoader:
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/features/entry_embeddings/entry_embeddings.py` & `python_search-0.9.9/python_search/next_item_predictor/features/entry_embeddings/entry_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 from typing import List, Tuple
 
 import msgpack_numpy as m
 import numpy as np
 from numpy import ndarray
 
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.infrastructure.performance import timeit
 from python_search.infrastructure.redis import PythonSearchRedis
 from python_search.search.entries_loader import EntriesLoader
 
 
 class RedisEmbeddingsReader:
     """
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/features/times_used.py` & `python_search-0.9.9/python_search/next_item_predictor/features/times_used.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/inference/inference.py` & `python_search-0.9.9/python_search/next_item_predictor/inference/inference.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,81 @@
 from __future__ import annotations
 
 import os
 from typing import Any, List, Optional
 
-from python_search.config import ConfigurationLoader, PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.infrastructure.performance import timeit
 from python_search.logger import setup_inference_logger
-from python_search.search.models import PythonSearchMLFlow
-from python_search.search.next_item_predictor.inference.input import ModelInput
-from python_search.search.next_item_predictor.transform import ModelTransform
+from python_search.next_item_predictor.inference.input import ModelInput
 
 logger = setup_inference_logger()
 
 
 class Inference:
     """
     Performs the search inference on all existing keys in the moment
     """
 
-    PRODUCTION_RUN_ID = "db6d108526b5438dbc0d9eaf2b765729"
-
     def __init__(
         self,
         configuration: Optional[PythonSearchConfiguration] = None,
         run_id: Optional[str] = None,
         model: Optional[Any] = None,
     ):
 
         self.debug = os.getenv("DEBUG", False)
-        self.run_id = run_id if run_id else self.PRODUCTION_RUN_ID
-        if "FORCE_RUN_ID" in os.environ:
-            self.run_id = os.environ["FORCE_RUN_ID"]
 
-        if model:
-            logger.info("Using custom passed _model")
-        else:
-            logger.info("Next item predictor using run id: " + self.run_id)
+
         configuration = (
             configuration if configuration else ConfigurationLoader().load_config()
         )
-        # previous key should be setted in runtime
-        self.previous_key = None
         self.all_keys = configuration.commands.keys()
-        self._transform = ModelTransform()
+        self._model = configuration.get_next_item_predictor_model()
+
+        self.run_id = run_id if run_id else self._model.get_run_id()
+
+        if model:
+            logger.info("Using custom passed model")
+        else:
+            logger.info("Next item predictor using run id: " + self.run_id)
 
         try:
-            self.model = model if model else self._load_mlflow_model(run_id=self.run_id)
+            self._mlflow_model = model if model else self._model.load_mlflow_model(run_id=self.run_id)
         except Exception as e:
             print("Failed to load mlflow model")
-            self.model = None
+            self._mlflow_model = None
             raise e
 
     @timeit
     def get_ranking(self, predefined_input: Optional[ModelInput] = None) -> List[str]:
         """
         Gets the search from the next item _model
         """
         logger.info("Number of existing keys for inference: " + str(len(self.all_keys)))
         inference_input = (
             predefined_input
             if predefined_input
             else ModelInput.with_given_keys(
-                self._transform.inference_embeddings.get_recent_key_with_embedding(),
-                self._transform.inference_embeddings.get_recent_key_with_embedding(
+                self._model.inference_embeddings.get_recent_key_with_embedding(),
+                self._model.inference_embeddings.get_recent_key_with_embedding(
                     second_recent=True
                 ),
             )
         )
         logger.info("Inference input: " + str(inference_input.__dict__))
 
-        X = self._transform.transform_single(inference_input, self.all_keys)
+        X = self._model.transform_single({'inference_input': inference_input, 'all_keys': self.all_keys})
         Y = self._predict(X)
         result = list(zip(self.all_keys, Y))
         result.sort(key=lambda x: x[1], reverse=True)
 
         only_keys = [entry[0] for entry in result]
         logger.info("Ranking inference succeeded")
 
         # logger.debug("Only keys: ", only_keys)
         return only_keys
 
     @timeit
     def _predict(self, X):
-        return self.model.predict(X)
-
-    @timeit
-    def _load_mlflow_model(self, run_id=None):
-        model = PythonSearchMLFlow().get_next_predictor_model(run_id=run_id)
-        return model
+        return self._mlflow_model.predict(X)
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/inference/input.py` & `python_search-0.9.9/python_search/next_item_predictor/inference/input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import os
 from typing import Optional
 
-from python_search.search.next_item_predictor.features.times_used import TimesUsed
+from python_search.next_item_predictor.features.times_used import TimesUsed
 
 
 class ModelInput:
     hour: int
     month: int
     previous_key: str
     previous_previous_key: str
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/mlflow_logger.py` & `python_search-0.9.9/python_search/next_item_predictor/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/next_item_pipeline.py` & `python_search-0.9.9/python_search/next_item_predictor/next_item_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,71 @@
 #!/usr/bin/env python
 
 import os
 from typing import List, Literal, Optional
 
 import numpy as np
-from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql import SparkSession
 from sklearn.model_selection import train_test_split
 
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.events.run_performed.clean import RunPerformedCleaning
-from python_search.search.next_item_predictor.mlflow_logger import configure_mlflow
-from python_search.search.next_item_predictor.offline_evaluation import (
+from python_search.next_item_predictor.mlflow_logger import configure_mlflow
+from python_search.next_item_predictor.offline_evaluation import (
     OfflineEvaluation,
 )
-from python_search.search.next_item_predictor.train_xgboost import TrainXGBoost
-from python_search.search.next_item_predictor.training_dataset import TrainingDataset
-
+from python_search.next_item_predictor.train_xgboost import TrainXGBoost
 
 class NextItemPredictorPipeline:
     """
     Exposes the whole ML pipeline, the runs everything
     """
 
     model_types: Literal["xgboost", "keras"] = "xgboost"
 
     def __init__(self):
-        os.environ["TIME_IT"] = "1"
-        print('Overriding pyspark python executable')
+        self._fix_python_interpreter_pyspark()
 
-        from subprocess import PIPE, Popen
-        command = "whereis python"
-        with Popen(command, stdout=PIPE, stderr=None, shell=True) as process:
-            output = process.communicate()[0].decode("utf-8")
-        print(f"Where is ouptut: {output}")
-        # get only the path and remove new line in the end
-        path = output.split(' ')[1].split("\n")[0]
-        print(f"Using the following path: {path}")
-        os.environ['PYSPARK_PYTHON'] = path
-        os.environ['PYSPARK_DRIVER_PYTHON'] = path
+        configuration = ConfigurationLoader().load_config()
+        self._model = configuration.get_next_item_predictor_model()
 
     def run(
         self,
         train_only: Optional[List[model_types]] = ['xgboost'],
         use_cache=False,
-        clean_first=True,
+        clean_events_first=False,
         skip_offline_evaluation=False,
     ):
         """
         Trains both xgboost and keras models
 
         Args:
             train_only:
             use_cache:
-            clean_first:
+            clean_events_first:
 
         Returns:
 
         """
         print("Starting pipeline, use --help for understaning the options")
 
         print("Using cache is:", use_cache)
 
         if not train_only:
             train_only = ["xgboost", "keras"]
         else:
             print("Training only: ", train_only)
 
-        if clean_first:
+        if clean_events_first:
             RunPerformedCleaning().clean()
 
-        dataset: DataFrame = TrainingDataset().build(use_cache)
-        from python_search.search.next_item_predictor.transform import ModelTransform
+        dataset = self._model.build_dataset()
 
-        X, Y = ModelTransform().transform_collection(dataset, use_cache=use_cache)
-        from python_search.search.next_item_predictor.train_keras import TrainKeras
+        X, Y = self._model.transform_collection(dataset)
+        from python_search.next_item_predictor.train_keras import TrainKeras
 
         X_train, X_test, Y_train, Y_test = train_test_split(
             X, Y, test_size=TrainKeras.TEST_SPLIT_SIZE, random_state=42
         )
 
         X_test_p = X_test
         X_test = np.delete(X_test, 0, axis=1)
@@ -92,29 +81,43 @@
                         model, dataset, X_test_p
                     )
                     mlflow.log_params(offline_evaluation)
 
         if "keras" in train_only:
             mlflow = configure_mlflow()
             with mlflow.start_run():
-                from python_search.search.next_item_predictor.train_keras import (
+                from python_search.next_item_predictor.train_keras import (
                     TrainKeras,
                 )
 
                 model = TrainKeras().train(X_train, X_test, Y_train, Y_test)
                 mlflow.keras.log_model(model, "model", keras_module="keras")
                 if not skip_offline_evaluation:
                     offline_evaluation = OfflineEvaluation().run(
                         model, dataset, X_test_p
                     )
                     mlflow.log_params(offline_evaluation)
 
     def _spark(self):
         return SparkSession.builder.getOrCreate()
 
+    def _fix_python_interpreter_pyspark(self):
+        print('Overriding pyspark python executable')
+
+        from subprocess import PIPE, Popen
+        command = "whereis python"
+        with Popen(command, stdout=PIPE, stderr=None, shell=True) as process:
+            output = process.communicate()[0].decode("utf-8")
+        print(f"Where is ouptut: {output}")
+        # get only the path and remove new line in the end
+        path = output.split(' ')[1].split("\n")[0]
+        print(f"Using the following path: {path}")
+        os.environ['PYSPARK_PYTHON'] = path
+        os.environ['PYSPARK_DRIVER_PYTHON'] = path
+
 
 def main():
     import fire
 
     fire.Fire(NextItemPredictorPipeline)
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/offline_evaluation.py` & `python_search-0.9.9/python_search/next_item_predictor/offline_evaluation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyspark.sql import DataFrame
 
-from python_search.config import ConfigurationLoader
-from python_search.search.next_item_predictor.inference.inference import Inference
-from python_search.search.next_item_predictor.inference.input import ModelInput
+from python_search.configuration.loader import ConfigurationLoader
+from python_search.next_item_predictor.inference.inference import Inference
+from python_search.next_item_predictor.inference.input import ModelInput
 
 
 class OfflineEvaluation:
     """
     Evaluate the _model with a part of the training _entries
     """
 
@@ -26,34 +26,37 @@
         inference = Inference(model=model)
 
         total_found = 0
         avg_position = 0
         number_of_existing_keys = len(self._configuration.commands.keys())
         for index, row in test_df.iterrows():
 
+            key = row['key']
+            previous_key = row.get('previous_key')
+            previous_previous_key = row.get('previous_previous_key')
+
             if (
                 not self._key_exists(row["key"])
-                or not self._key_exists(row["previous_key"])
-                or not self._key_exists(row["previous_previous_key"])
+                or ('previous_key' in row and not self._key_exists(row["previous_key"]))
+                or ('previous_previous_key' in row and not self._key_exists(row["previous_previous_key"]))
             ):
                 print(
-                    f"Key pair does not exist any longer ({row['previous_key']}, {row['key']})"
+                    f"Members of entry do not existly any longer ({key}, {previous_key}, {previous_previous_key})"
                 )
                 continue
 
             input = ModelInput(
-                hour=row["hour"],
-                month=row["month"],
-                previous_key=row["previous_key"],
-                previous_previous_key=row["previous_previous_key"],
+                hour=row.get("hour"),
+                month=row.get("month"),
+                previous_key=previous_key,
+                previous_previous_key=previous_previous_key,
             )
             result = inference.get_ranking(predefined_input=input)
 
             metadata = {
-                "pair": row["previous_key"] + " -> " + row["key"],
                 "position_target": result.index(row["key"]),
                 "Len": len(result),
                 "type of result": type(result),
             }
             print(metadata)
 
             avg_position += metadata["position_target"]
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/train_keras.py` & `python_search-0.9.9/python_search/next_item_predictor/train_keras.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/train_xgboost.py` & `python_search-0.9.9/python_search/next_item_predictor/train_xgboost.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/training_dataset.py` & `python_search-0.9.9/python_search/next_item_predictor/training_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.functions import struct, udf
 from pyspark.sql.types import FloatType
 from pyspark.sql.window import Window
 
 from python_search.events.run_performed.dataset import EntryExecutedDataset
 from python_search.infrastructure.performance import timeit
-from python_search.search.next_item_predictor.features.times_used import TimesUsed
-from python_search.search.next_item_predictor.inference.label import label_formula
+from python_search.next_item_predictor.features.times_used import TimesUsed
+from python_search.next_item_predictor.inference.label import label_formula
 
 
 class TrainingDataset:
     """
     Builds the dataset ready for training
     """
```

### Comparing `python_search-0.9.8/python_search/search/next_item_predictor/transform.py` & `python_search-0.9.9/python_search/next_item_predictor/next_item_model_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import logging
 import os
 from typing import Dict, List, Tuple
 
 import numpy as np
 from pyspark.sql import DataFrame
 
-from python_search.config import ConfigurationLoader
-from python_search.search.next_item_predictor.features.entry_embeddings import (
+from python_search.configuration.loader import ConfigurationLoader
+from python_search.search.models import PythonSearchMLFlow
+from python_search.next_item_predictor.features.entry_embeddings import (
     InferenceEmbeddingsLoader,
 )
-from python_search.search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
+from python_search.next_item_predictor.features.entry_embeddings.entry_embeddings import (
     create_key_indexed_embedding,
 )
-from python_search.search.next_item_predictor.inference.input import ModelInput
-from python_search.search.next_item_predictor.training_dataset import TrainingDataset
+from python_search.next_item_predictor.training_dataset import TrainingDataset
+from python_search.next_item_predictor.model_interface import ModelInterface
 
 
-class ModelTransform:
+class NextItemModelV1(ModelInterface):
     """
     Transform takes an input and make it ready for inference
 
     From training dataset to -> _model input
     And from inference dataset -> _model input
     """
 
@@ -29,78 +30,46 @@
     # 2 embeddings of 384 dimensions
     # + 1 is for the month number
     # + 1 for entry number
     # + 1 for global popularity of previous key
     # + 1 for global popularity of previous_previous key
     DIMENSIONS = _EMBEDDINGS_ENTRIES * 384 + 1 + 1 + 1 + 1
 
+    PRODUCTION_RUN_ID = "db6d108526b5438dbc0d9eaf2b765729"
+
     def __init__(self):
         configuration = ConfigurationLoader().load_config()
         self._all_keys = configuration.commands.keys()
         self.inference_embeddings = InferenceEmbeddingsLoader(self._all_keys)
 
-    def transform_single(self, inference_input: ModelInput, all_keys) -> np.ndarray:
-        """
-        Transform the inference input into something that can be inferred.
-        This is an element wise search.
-        """
-
-        previous_key_embedding = self.inference_embeddings.get_embedding_from_key(
-            inference_input.previous_key
-        )
-        previous_previous_key_embedding = (
-            self.inference_embeddings.get_embedding_from_key(
-                inference_input.previous_previous_key
-            )
-        )
-
-        # create an inference array for all keys
-        X = np.zeros([len(self._all_keys), ModelTransform.DIMENSIONS])
-        for i, key in enumerate(all_keys):
-            key_embedding = self.inference_embeddings.get_embedding_from_key(key)
-            if key_embedding is None:
-                logging.warning(f"No content for key ({key})")
-                continue
-
-            X[i] = np.concatenate(
-                (
-                    key_embedding,
-                    previous_key_embedding,
-                    previous_previous_key_embedding,
-                    np.asarray([inference_input.month]),
-                    np.asarray([inference_input.hour]),
-                    np.asarray([inference_input.times_used_previous]),
-                    np.asarray([inference_input.times_used_previous_previous]),
-                )
-            )
-
-        return X
+    def build_dataset(self):
+        return TrainingDataset().build()
 
     def transform_collection(
         self, dataset: DataFrame, use_cache=True
     ) -> Tuple[np.ndarray, np.ndarray]:
         """
         Transform the dataset into X and Y
         Returns a pair with X, Y
         """
         print("Number of rows in the dataset: ", dataset.count())
-        print(f"Dimensions of dataset = {ModelTransform.DIMENSIONS}")
+        print(f"Dimensions of dataset = {NextItemModelV1.DIMENSIONS}")
 
         if use_cache:
             if not os.path.exists("/tmp/X.npy") or not os.path.exists("/tmp/Y.npy"):
                 raise Exception("Cache not found")
             print("Using transformed data from cache")
             X = np.load("/tmp/X.npy", allow_pickle=True)
             Y = np.load("/tmp/Y.npy", allow_pickle=True)
 
             return X, Y
 
         embeddings_keys = self._create_embeddings_training_dataset(dataset)
         # one extra for the row number
-        X = np.zeros([dataset.count(), ModelTransform.DIMENSIONS + 1])
+        X = np.zeros([dataset.count(), NextItemModelV1.DIMENSIONS + 1])
         Y = np.empty(dataset.count())
 
         print("X shape:", X.shape)
 
         # transform the spark dataframe into a python iterable
         collected_rows = dataset.select(*TrainingDataset.COLUMNS).collect()
 
@@ -126,14 +95,54 @@
         Y = np.where(np.isnan(Y), 0.5, Y)
 
         np.save("/tmp/X.npy", X)
         np.save("/tmp/Y.npy", Y)
 
         return X, Y
 
+    def transform_single(self, inference_input: dict) -> np.ndarray:
+        """
+        Transform the inference input into something that can be inferred.
+        This is an element wise search.
+        """
+
+        inference_input_obj = inference_input['inference_input']
+        all_keys = inference_input['all_keys']
+
+        previous_key_embedding = self.inference_embeddings.get_embedding_from_key(
+            inference_input_obj.previous_key
+        )
+        previous_previous_key_embedding = (
+            self.inference_embeddings.get_embedding_from_key(
+                inference_input_obj.previous_previous_key
+            )
+        )
+
+        # create an inference array for all keys
+        X = np.zeros([len(all_keys), NextItemModelV1.DIMENSIONS])
+        for i, key in enumerate(all_keys):
+            key_embedding = self.inference_embeddings.get_embedding_from_key(key)
+            if key_embedding is None:
+                logging.warning(f"No content for key ({key})")
+                continue
+
+            X[i] = np.concatenate(
+                (
+                    key_embedding,
+                    previous_key_embedding,
+                    previous_previous_key_embedding,
+                    np.asarray([inference_input_obj.month]),
+                    np.asarray([inference_input_obj.hour]),
+                    np.asarray([inference_input_obj.times_used_previous]),
+                    np.asarray([inference_input_obj.times_used_previous_previous]),
+                )
+            )
+
+        return X
+
     def _create_embeddings_training_dataset(
         self, dataset: TrainingDataset
     ) -> Dict[str, np.ndarray]:
         """
         create embeddings with all training keys and keep them in memory
         """
         print("Creating embeddings of training dataset")
@@ -148,7 +157,14 @@
 
         keys = []
         for collected_keys in collected_keys:
             keys.append(collected_keys.key)
             keys.append(collected_keys.previous_key)
 
         return keys
+
+    def load_mlflow_model(self, run_id=None):
+        model = PythonSearchMLFlow().get_next_predictor_model(run_id=run_id)
+        return model
+
+    def get_run_id(self):
+        return NextItemModelV1.PRODUCTION_RUN_ID
```

### Comparing `python_search-0.9.8/python_search/search/results.py` & `python_search-0.9.9/python_search/search/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,29 @@
 
 
 class FzfOptimizedSearchResults:
     """
     Builds the list of results ready to be consumed by fzf
     """
 
+    degraded_message = ""
+
     def __init__(self):
         self._today = datetime.datetime.now()
 
+
     @timeit
     def build_entries_result(
         self, entries: RankedEntries.type, ranking_uuid: str
     ) -> str:
         """Print results"""
         position = 1
         result = ""
+        if self.degraded_message:
+            result = f"Degraded: {self.degraded_message}\n"
         for name, content in entries:
             try:
                 if "snippet" in content:
                     content["snippet"] = sanitize(content["snippet"])
                 if "cmd" in content:
                     content["cmd"] = sanitize(content["cmd"])
 
@@ -65,15 +70,15 @@
                 content_str = json.dumps(content, default=tuple, ensure_ascii=True)
             except BaseException as e:
                 logging.info(e)
                 content_str = str(content)
 
             position = position + 1
 
-            content_str = f"{name}:" + content_str
+            content_str = f"{name}                                                      :" + content_str
             #  replaces all single quotes for double ones
             #  otherwise the json does not get rendered
             content_str = content_str.replace("'", '"')
             if os.getenv("ENABLE_TIME_IT"):
                 # do not print if enable timeit is on
                 continue
             result += content_str + "\n"
```

### Comparing `python_search-0.9.8/python_search/search/search.py` & `python_search-0.9.9/python_search/search/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 from collections import namedtuple
 from typing import List, Literal, Optional
 
-from python_search.config import PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
 from python_search.events.latest_used_entries import RecentKeys
 from python_search.events.ranking_generated import (
     RankingGenerated,
     RankingGeneratedWriter,
 )
 from python_search.feature_toggle import FeatureToggle
 from python_search.infrastructure.performance import timeit
@@ -29,53 +29,51 @@
     _inference = None
 
     def __init__(self, configuration: Optional[PythonSearchConfiguration] = None):
         self._configuration = configuration
         self._feature_toggle = FeatureToggle()
         self._model = None
         self._entries_result = FzfOptimizedSearchResults()
-        self._entries = None
+        self._entries: Optional[dict] = None
         self._ranking_generator_writer = RankingGeneratedWriter()
         self._ranking_method_used: Literal[
             "RankingNextModel", "BaselineRank"
         ] = "BaselineRank"
 
         if self._feature_toggle.is_enabled("ranking_next"):
-            from python_search.search.next_item_predictor.inference.inference import (
-                Inference,
-            )
+            from python_search.next_item_predictor.inference.inference import Inference
 
             try:
                 self._inference = Inference(self._configuration)
             except Exception as e:
                 print(
                     f"Could not initialize the inference component. Proceeding without inference, details: {e}"
                 )
+                self._entries_result.degraded_message = f"{e}"
 
     @timeit
     def search(self) -> str:
         """
         Recomputes the rank and saves the results on the file to be read
         """
 
         self._entries: dict = self._configuration.commands
         # by default the rank is just in the order they are persisted in the file
         self._ranked_keys: List[str] = list(self._entries.keys())
 
-        if self._feature_toggle.is_enabled("ranking_next") and self._inference:
-            self._rerank_via_model()
+        self._rerank_via_model()
+
 
         """Populate the variable used_entries  with the results from redis"""
         result = self._merge_with_latest_used()
 
         ranknig_generated_event = RankingGenerated(
             ranking=[i[0] for i in result[0:100]]
         )
         self._ranking_generator_writer.write(ranknig_generated_event)
-        print(f"Ranking generated UUID {ranknig_generated_event.uuid}")
         result_str = self._entries_result.build_entries_result(
             result, ranknig_generated_event.uuid
         )
 
         return result_str
 
     def _rerank_via_model(self):
```

### Comparing `python_search-0.9.8/python_search/search_ui/fzf_kitty.py` & `python_search-0.9.9/python_search/search_ui/fzf_kitty.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import os
 
 from python_search.apps.terminal import Terminal
-from python_search.config import PythonSearchConfiguration
+from python_search.configuration.configuration import PythonSearchConfiguration
 from python_search.environment import is_mac
 
 
 class FzfInKitty:
     """
     Renders the search ui using fzf + termite terminal
     """
 
-    FONT_SIZE = 15
+    FONT_SIZE : int = 15
     PREVIEW_PERCENTAGE_SIZE = 50
-    HEIGHT = 127
-    WIDTH = 950
-    RANK_TIE_BREAK = "begin,index"
+    _default_window_size = (800, 400)
+    RANK_TIE_BREAK : str = "begin,index"
 
     configuration: PythonSearchConfiguration
 
     def __init__(self, configuration: PythonSearchConfiguration):
-        self.height = FzfInKitty.HEIGHT
-        self.width = FzfInKitty.WIDTH
+        custom_window_size = configuration.get_window_size()
+        self.width = custom_window_size[0] if custom_window_size else self._default_window_size[0]
+        self.height = custom_window_size[1] if custom_window_size else self._default_window_size[1]
 
         self.preview_cmd = f"python_search _preview_entry {{}} "
         self.title = configuration.APPLICATION_TITLE
         self.configuration = configuration
 
         import logging
         import sys
@@ -35,24 +35,28 @@
 
         self._logger = logger
 
     def run(self) -> None:
         self._launch_terminal(self._fzf_cmd())
 
     def _fzf_cmd(self):
-        FZF_LIGHT_THEME = "fg:#4d4d4c,bg:#ffffff,hl:#d7005f,info:#4271ae,prompt:#8959a8,pointer:#d7005f,marker:#4271ae,spinner:#4271ae,header:#4271ae,fg+:#4d4d4c,bg+:#ffffff,hl+:#d7005f"
-        THEME = f"--color={FZF_LIGHT_THEME}"  # for more fzf options see: https://www.mankier.com/1/fzf#
+        THEME = ""
+        if self.configuration.get_fzf_theme() == "light":
+            FZF_LIGHT_THEME = "fg:#4d4d4c,bg:#ffffff,hl:#d7005f,info:#4271ae,prompt:#8959a8,pointer:#d7005f,marker:#4271ae,spinner:#4271ae,header:#4271ae,fg+:#4d4d4c,bg+:#ffffff,hl+:#d7005f"
+            THEME = f"--color={FZF_LIGHT_THEME}"  # for more fzf options see: https://www.mankier.com/1/fzf#
         cmd = f"""bash -c ' export SHELL=bash ; {self._get_rankging_generate_cmd()} | \
         fzf \
         --tiebreak={FzfInKitty.RANK_TIE_BREAK} \
         --extended \
         --reverse \
+        --no-separator \
         --info=inline \
         --cycle \
         --no-hscroll \
+        --ellipsis='' \
         --hscroll-off=0 \
         --preview "{self.preview_cmd}" \
         --preview-window=right,{FzfInKitty.PREVIEW_PERCENTAGE_SIZE}%,wrap,border-left \
         -i \
         --border=none \
         --margin=0% \
         --padding=0% \
@@ -77,39 +81,28 @@
         '
         """
 
         self._logger.info("Cmd: ", cmd)
         return cmd
 
     def _run_key(self, shortcut) -> str:
-        return f"""--bind "{shortcut}:execute-silent:(LOG_FILE=/tmp/log_run_key_fzf nohup python_search run_key {{}} --query_used {{q}} && kill -9 $PPID)"  """
+        return f"""--bind "{shortcut}:execute-silent:(run_key {{}} --query_used {{q}} --fzf_pid_to_kill $PPID {{}} &)"  """
 
     def _edit_key(self, shortcut) -> str:
-        return f"""--bind "{shortcut}:execute-silent:(nohup python_search edit_key {{}} & disown && kill -9 $PPID ) "  """
+        return f"""--bind "{shortcut}:execute-silent:(nohup python_search edit_key --fzf_pid_to_kill $PPID {{}}  & disown)" """
 
     def _get_rankging_generate_cmd(self, reload=False):
-        # @todo move this part to a binary sdk
+        # in mac we need tensorflow to be installed via conda
         if self.configuration.supported_features.is_dynamic_ranking_supported():
             if reload:
                 return f"curl -s localhost:8000/ranking/reload_and_generate"
 
             return f"curl -s localhost:8000/ranking/generate"
 
-        from python_search.cli import PythonSearchCli
-        from python_search.search.search import Search
-        return f"python_search " + PythonSearchCli._ranking.__name__ +  ' ' + Search.search.__name__
-
-    def _docker_running(self) -> bool:
-        result = os.system("docker info")
-
-        if result != 0:
-            print("Docker is not running")
-            return False
-
-        return True
+        return f"python_search _ranking search"
 
     def _launch_terminal(self, internal_cmd: str) -> None:
 
         font = "FontAwesome"
         if is_mac():
             font = "Pragmata Pro"
```

### Comparing `python_search-0.9.8/python_search/search_ui/preview.py` & `python_search-0.9.9/python_search/search_ui/preview.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from datetime import datetime
 
 from colorama import Fore
 from dateutil import parser
 
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.logger import setup_preview_logger
 from python_search.search_ui.serialized_entry import (
     decode_serialized_data_from_entry_text,
 )
 
 
 class Preview:
     """
     Preview the entry in the search ui
     """
 
     def __init__(self):
         self.configuration = ConfigurationLoader()
         self.logger = setup_preview_logger()
+        self.entries = self.configuration.load_entries()
         # do not send the errors to stderr, in the future we should send to kibana or a file
 
     def display(self, entry_text: str):
         """
         Prints the entry in the preview window
 
         """
+        key = self._extract_key(entry_text)
+        if not self._key_exists(key):
+            print(f"Not found as key {entry_text}")
+            return
 
         data = self._build_values_to_print(entry_text)
         self._print_values(data)
 
     def _print_values(self, data):
         print("")
         print(
@@ -57,17 +62,23 @@
             return Fore.RED
 
         if type in ["Url", "File"]:
             return Fore.GREEN
 
         return Fore.BLUE
 
-    def _build_values_to_print(self, entry_text) -> dict:
+    def _extract_key(self, entry_text):
         key = entry_text.split(":")[0]
+        # remove the last 2 spaces from the key as they are used for formatting the string in fzf
+        key = key.strip()
+        return key
+
+    def _build_values_to_print(self, entry_text) -> dict:
         # the entry content is after the key + a ":" character
+        key = self._extract_key(entry_text)
 
         result = {}
         result["type"] = "Unknown"
         result["key"] = key
         entry_data = self._load_key_data(key)
         if "url" in entry_data:
             result["value"] = entry_data.get("url")
@@ -119,21 +130,22 @@
             result["uuid"] = str(decoded_content["uuid"])
 
         return result
 
     def _color_str(self, a_string, a_color) -> str:
         return f"{a_color}{a_string}{Fore.RESET}"
 
+    def _key_exists(self, key):
+        return key in self.entries
+
     def _load_key_data(self, key):
-        entries = self.configuration.load_entries()
-        if not key in entries:
-            print()
+        if not self._key_exists(key):
             print(
                 (
                     f'Key "{self._color_str(key, Fore.RED)}" not found in python search data'
                 )
             )
             import sys
 
             sys.exit(0)
 
-        return entries[key]
+        return self.entries[key]
```

### Comparing `python_search-0.9.8/python_search/search_ui/serialized_entry.py` & `python_search-0.9.9/python_search/search_ui/serialized_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,12 @@
     serialized_content = entry_text[len(key) + 1 :]
     try:
         result = json.loads(serialized_content)
         logger.info(f"Decoded serialized content worked {result}")
 
         return result
     except Exception as e:
-        message = f"Failed with error {e} wile decoding the followingthe entry_text '{entry_text}' "
+        message = f"Failed with error {e} wile decoding the following entry_text '{entry_text}' "
         if logger:
             logger.info(message)
 
         return {}
```

### Comparing `python_search-0.9.8/python_search/shortcut/generator.py` & `python_search-0.9.9/python_search/shortcut/generator.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/shortcut/gnome.py` & `python_search-0.9.9/python_search/shortcut/gnome.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/shortcut/i3.py` & `python_search-0.9.9/python_search/shortcut/i3.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/shortcut/mac.py` & `python_search-0.9.9/python_search/shortcut/mac.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/shortcuts.py` & `python_search-0.9.9/python_search/shortcuts.py`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/python_search/web_api.py` & `python_search-0.9.9/python_search/web_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from python_search.entry_type.classifier_inference import (
     EntryData,
     PredictEntryTypeInference,
 )
 from python_search.events.latest_used_entries import RecentKeys
 from python_search.events.run_performed import RunPerformed
 from python_search.events.run_performed.writer import RunPerformedWriter
-from python_search.config import ConfigurationLoader
+from python_search.configuration.loader import ConfigurationLoader
 from python_search.search.search import Search
 
 import pyroscope
 
 pyroscope.configure(
     application_name="my.python.app",  # replace this with some name for your application
     server_address="http://host.docker.internal:4040",  # replace this with the address of your pyroscope server
@@ -48,32 +48,28 @@
 
 @app.get("/ranking/reload", response_class=PlainTextResponse)
 def reload():
     reload_ranking()
 
 
 @app.get("/ranking/reload_and_generate", response_class=PlainTextResponse)
-def reload():
+def reload_and_generate():
     return reload_ranking()
 
 
 @app.get("/_health")
 def health():
     global generator
 
     from python_search.events.latest_used_entries import RecentKeys
 
     entries = RecentKeys().get_latest_used_keys()
-    run_id = None
-    if generator._inference is not None:
-        run_id = generator._inference.PRODUCTION_RUN_ID
 
     return {
         "keys_count": len(ConfigurationLoader().load_config().commands.keys()),
-        "run_id": run_id,
         "latest_used_entries": entries,
         "initialization_time": ConfigurationLoader().load_config()._initialization_time,
     }
 
 
 @app.post("/log_run")
 def log_run(event: RunPerformed):
```

### Comparing `python_search-0.9.8/wrap_log_command.sh` & `python_search-0.9.9/wrap_log_command.sh`

 * *Files identical despite different names*

### Comparing `python_search-0.9.8/setup.py` & `python_search-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['python_search',
  'python_search.apps',
+ 'python_search.configuration',
  'python_search.data_ui',
  'python_search.entry_capture',
  'python_search.entry_description_generator',
  'python_search.entry_type',
  'python_search.events',
  'python_search.events.ranking_generated',
  'python_search.events.run_performed',
  'python_search.infrastructure',
  'python_search.init',
  'python_search.interpreter',
+ 'python_search.next_item_predictor',
+ 'python_search.next_item_predictor.features',
+ 'python_search.next_item_predictor.features.entry_embeddings',
+ 'python_search.next_item_predictor.inference',
  'python_search.plugins',
  'python_search.sdk',
  'python_search.search',
- 'python_search.search.next_item_predictor',
- 'python_search.search.next_item_predictor.features',
- 'python_search.search.next_item_predictor.features.entry_embeddings',
- 'python_search.search.next_item_predictor.inference',
  'python_search.search_ui',
  'python_search.shortcut']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
@@ -60,16 +61,18 @@
                      'browser = python_search.apps.browser:main',
                      'clipboard = python_search.apps.clipboard:main',
                      'collect_input = python_search.apps.collect_input:main',
                      'feature_toggle = '
                      'python_search.feature_toggle:FeatureToggle.main',
                      'generic_data_collector = '
                      'python_search.data_collector:GenericDataCollector.initialize',
+                     'next_item = '
+                     'python_search.next_item_predictor.next_item_pipeline:main',
                      'next_item_pipeline = '
-                     'python_search.search.next_item_predictor.next_item_pipeline:main',
+                     'python_search.next_item_predictor.next_item_pipeline:main',
                      'notify_send = python_search.apps.notification_ui:main',
                      'ps_container = python_search.container:start',
                      'ps_webapi = python_search.sdk.web_api_sdk:main',
                      'python_search = python_search.cli:main',
                      'python_search_infra = '
                      'python_search.infrastructure.infrastructure:main',
                      'python_search_webapi = python_search.web_api:main',
@@ -78,15 +81,15 @@
                      'run_key = python_search.cli:_run_key_bin']}
 
 scripts = \
 ['wrap_log_command.sh']
 
 setup_kwargs = {
     'name': 'python-search',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Build your knowledge database in python and retrieve it efficiently',
     'long_description': 'None',
     'author': 'Jean Carlo Machado',
     'author_email': 'machado.c.jean@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `python_search-0.9.8/PKG-INFO` & `python_search-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-search
-Version: 0.9.8
+Version: 0.9.9
 Summary: Build your knowledge database in python and retrieve it efficiently
 Author: Jean Carlo Machado
 Author-email: machado.c.jean@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

