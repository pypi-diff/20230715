# Comparing `tmp/granny-pliers-0.0.18.tar.gz` & `tmp/granny-pliers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "granny-pliers-0.0.18.tar", last modified: Sat Jul 15 13:42:33 2023, max compression
+gzip compressed data, was "granny-pliers-0.0.9.tar", last modified: Wed Jun 14 21:02:38 2023, max compression
```

## Comparing `granny-pliers-0.0.18.tar` & `granny-pliers-0.0.9.tar`

### file list

```diff
@@ -1,75 +1,70 @@
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.199671 granny-pliers-0.0.18/
--rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.18/LICENSE
--rw-r--r--   0 pd         (501) staff       (20)    13843 2023-07-15 13:42:33.199203 granny-pliers-0.0.18/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.18/README.md
--rw-r--r--   0 pd         (501) staff       (20)     2362 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/pyproject.toml
--rw-r--r--   0 pd         (501) staff       (20)       38 2023-07-15 13:42:33.199799 granny-pliers-0.0.18/setup.cfg
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.159500 granny-pliers-0.0.18/src/
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.167194 granny-pliers-0.0.18/src/granny_pliers/
--rw-r--r--   0 pd         (501) staff       (20)     1116 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.174980 granny-pliers-0.0.18/src/granny_pliers/auth/
--rw-r--r--   0 pd         (501) staff       (20)     1028 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.18/src/granny_pliers/auth/auth_config.py
--rw-r--r--   0 pd         (501) staff       (20)      987 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/auth/auth_error.py
--rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.18/src/granny_pliers/auth/auth_request.py
--rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.18/src/granny_pliers/auth/auth_response.py
--rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.18/src/granny_pliers/auth/jwt.py
--rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.18/src/granny_pliers/auth/permissions.py
--rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.18/src/granny_pliers/auth/roles.py
--rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.18/src/granny_pliers/auth/rsa_codec.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.177403 granny-pliers-0.0.18/src/granny_pliers/config/
--rw-r--r--   0 pd         (501) staff       (20)      865 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/config/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     3186 2023-07-07 22:22:41.000000 granny-pliers-0.0.18/src/granny_pliers/config/abstract_config.py
--rw-r--r--   0 pd         (501) staff       (20)     1749 2023-07-06 20:08:56.000000 granny-pliers-0.0.18/src/granny_pliers/config/autowired_config.py
--rw-r--r--   0 pd         (501) staff       (20)     7048 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/config/logger_config.py
--rw-r--r--   0 pd         (501) staff       (20)      861 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/config/project_environment.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.178744 granny-pliers-0.0.18/src/granny_pliers/logger/
--rw-r--r--   0 pd         (501) staff       (20)      859 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/logger/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.18/src/granny_pliers/logger/abstract_logger.py
--rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.18/src/granny_pliers/logger/log_processors.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.179176 granny-pliers-0.0.18/src/granny_pliers/models/
--rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.18/src/granny_pliers/models/__init__.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.180126 granny-pliers-0.0.18/src/granny_pliers/models/auth/
--rw-r--r--   0 pd         (501) staff       (20)      663 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/models/auth/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2061 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/models/auth/user.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.181243 granny-pliers-0.0.18/src/granny_pliers/models/metrics/
--rw-r--r--   0 pd         (501) staff       (20)      690 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/models/metrics/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.18/src/granny_pliers/models/metrics/confusion_matrix.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.182731 granny-pliers-0.0.18/src/granny_pliers/models/web/
--rw-r--r--   0 pd         (501) staff       (20)      704 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/models/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1669 2023-07-09 09:54:16.000000 granny-pliers-0.0.18/src/granny_pliers/models/web/web_service_health_status.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.188933 granny-pliers-0.0.18/src/granny_pliers/orm/
--rw-r--r--   0 pd         (501) staff       (20)     1072 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/orm/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.18/src/granny_pliers/orm/abstract_http_client.py
--rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.18/src/granny_pliers/orm/abstract_http_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     3296 2023-07-01 23:04:28.000000 granny-pliers-0.0.18/src/granny_pliers/orm/abstract_model.py
--rw-r--r--   0 pd         (501) staff       (20)    20067 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/orm/abstract_mongo_repository.py
--rw-r--r--   0 pd         (501) staff       (20)     7827 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/orm/abstract_repository.py
--rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.18/src/granny_pliers/orm/restful_http_client.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.191204 granny-pliers-0.0.18/src/granny_pliers/scheduler/
--rw-r--r--   0 pd         (501) staff       (20)      217 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/scheduler/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1154 2023-06-25 17:47:45.000000 granny-pliers-0.0.18/src/granny_pliers/scheduler/abstract_schedule_object.py
--rw-r--r--   0 pd         (501) staff       (20)     7068 2023-06-25 17:47:10.000000 granny-pliers-0.0.18/src/granny_pliers/scheduler/abstract_scheduler.py
--rw-r--r--   0 pd         (501) staff       (20)     4916 2023-06-25 17:44:42.000000 granny-pliers-0.0.18/src/granny_pliers/scheduler/time_table.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.193018 granny-pliers-0.0.18/src/granny_pliers/testing/
--rw-r--r--   0 pd         (501) staff       (20)      781 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/testing/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.18/src/granny_pliers/testing/abstract_test_case.py
--rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.18/src/granny_pliers/testing/async_abstract_test_case.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.194200 granny-pliers-0.0.18/src/granny_pliers/tools/
--rw-r--r--   0 pd         (501) staff       (20)      686 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/tools/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.18/src/granny_pliers/tools/datetime_helper.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.197255 granny-pliers-0.0.18/src/granny_pliers/web/
--rw-r--r--   0 pd         (501) staff       (20)      941 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/web/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     2194 2023-07-09 09:54:22.000000 granny-pliers-0.0.18/src/granny_pliers/web/abstract_status_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.18/src/granny_pliers/web/abstract_web_application.py
--rw-r--r--   0 pd         (501) staff       (20)    12099 2023-07-07 22:39:35.000000 granny-pliers-0.0.18/src/granny_pliers/web/abstract_web_service.py
--rw-r--r--   0 pd         (501) staff       (20)     1575 2023-06-15 19:06:25.000000 granny-pliers-0.0.18/src/granny_pliers/web/web_application_config.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.198521 granny-pliers-0.0.18/src/granny_pliers/worker/
--rw-r--r--   0 pd         (501) staff       (20)      688 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/worker/__init__.py
--rw-r--r--   0 pd         (501) staff       (20)     5471 2023-07-15 13:42:07.000000 granny-pliers-0.0.18/src/granny_pliers/worker/abstract_worker.py
-drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-07-15 13:42:33.170128 granny-pliers-0.0.18/src/granny_pliers.egg-info/
--rw-r--r--   0 pd         (501) staff       (20)    13843 2023-07-15 13:42:33.000000 granny-pliers-0.0.18/src/granny_pliers.egg-info/PKG-INFO
--rw-r--r--   0 pd         (501) staff       (20)     2275 2023-07-15 13:42:33.000000 granny-pliers-0.0.18/src/granny_pliers.egg-info/SOURCES.txt
--rw-r--r--   0 pd         (501) staff       (20)        1 2023-07-15 13:42:33.000000 granny-pliers-0.0.18/src/granny_pliers.egg-info/dependency_links.txt
--rw-r--r--   0 pd         (501) staff       (20)      262 2023-07-15 13:42:33.000000 granny-pliers-0.0.18/src/granny_pliers.egg-info/requires.txt
--rw-r--r--   0 pd         (501) staff       (20)       14 2023-07-15 13:42:33.000000 granny-pliers-0.0.18/src/granny_pliers.egg-info/top_level.txt
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.471133 granny-pliers-0.0.9/
+-rw-r--r--   0 pd         (501) staff       (20)    11357 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/LICENSE
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.470754 granny-pliers-0.0.9/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)       16 2023-06-10 17:39:54.000000 granny-pliers-0.0.9/README.md
+-rw-r--r--   0 pd         (501) staff       (20)     1619 2023-06-14 20:50:52.000000 granny-pliers-0.0.9/pyproject.toml
+-rw-r--r--   0 pd         (501) staff       (20)       38 2023-06-14 21:02:38.471227 granny-pliers-0.0.9/setup.cfg
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.437214 granny-pliers-0.0.9/src/
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.440162 granny-pliers-0.0.9/src/granny_pliers/
+-rw-r--r--   0 pd         (501) staff       (20)      987 2023-06-14 20:51:00.000000 granny-pliers-0.0.9/src/granny_pliers/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.448122 granny-pliers-0.0.9/src/granny_pliers/auth/
+-rw-r--r--   0 pd         (501) staff       (20)     1228 2023-06-10 13:12:31.000000 granny-pliers-0.0.9/src/granny_pliers/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1683 2023-06-10 11:50:56.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      986 2023-06-10 13:13:15.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py
+-rw-r--r--   0 pd         (501) staff       (20)     1308 2023-06-10 13:13:08.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py
+-rw-r--r--   0 pd         (501) staff       (20)     1016 2023-06-10 13:11:55.000000 granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py
+-rw-r--r--   0 pd         (501) staff       (20)     6158 2023-06-10 13:18:46.000000 granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py
+-rw-r--r--   0 pd         (501) staff       (20)      882 2023-06-10 11:26:21.000000 granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py
+-rw-r--r--   0 pd         (501) staff       (20)      828 2023-06-10 11:26:59.000000 granny-pliers-0.0.9/src/granny_pliers/auth/roles.py
+-rw-r--r--   0 pd         (501) staff       (20)     9678 2023-06-10 13:14:07.000000 granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.450537 granny-pliers-0.0.9/src/granny_pliers/config/
+-rw-r--r--   0 pd         (501) staff       (20)      985 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/config/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     3198 2023-06-09 21:43:11.000000 granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     1614 2023-06-03 23:39:30.000000 granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py
+-rw-r--r--   0 pd         (501) staff       (20)     6694 2023-06-14 20:55:52.000000 granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py
+-rw-r--r--   0 pd         (501) staff       (20)      860 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.452701 granny-pliers-0.0.9/src/granny_pliers/logger/
+-rw-r--r--   0 pd         (501) staff       (20)      884 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1292 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py
+-rw-r--r--   0 pd         (501) staff       (20)     1253 2023-06-03 18:43:25.000000 granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.453438 granny-pliers-0.0.9/src/granny_pliers/models/
+-rw-r--r--   0 pd         (501) staff       (20)      620 2023-06-10 11:58:05.000000 granny-pliers-0.0.9/src/granny_pliers/models/__init__.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.454935 granny-pliers-0.0.9/src/granny_pliers/models/auth/
+-rw-r--r--   0 pd         (501) staff       (20)      688 2023-06-10 13:33:22.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2061 2023-06-10 13:36:39.000000 granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.456903 granny-pliers-0.0.9/src/granny_pliers/models/metrics/
+-rw-r--r--   0 pd         (501) staff       (20)      715 2023-06-10 13:32:44.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2766 2023-06-10 13:33:13.000000 granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.458526 granny-pliers-0.0.9/src/granny_pliers/models/web/
+-rw-r--r--   0 pd         (501) staff       (20)      729 2023-06-10 13:36:51.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1645 2023-06-10 11:59:08.000000 granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.462837 granny-pliers-0.0.9/src/granny_pliers/orm/
+-rw-r--r--   0 pd         (501) staff       (20)     1222 2023-06-10 13:29:12.000000 granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5494 2023-06-10 13:26:46.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py
+-rw-r--r--   0 pd         (501) staff       (20)     5956 2023-06-10 13:25:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     2990 2023-06-10 13:38:35.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py
+-rw-r--r--   0 pd         (501) staff       (20)    19833 2023-06-10 13:36:11.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)     7523 2023-06-09 21:46:56.000000 granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py
+-rw-r--r--   0 pd         (501) staff       (20)    14519 2023-06-10 17:09:48.000000 granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.464681 granny-pliers-0.0.9/src/granny_pliers/testing/
+-rw-r--r--   0 pd         (501) staff       (20)      806 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     1998 2023-06-10 12:35:19.000000 granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py
+-rw-r--r--   0 pd         (501) staff       (20)      914 2023-06-10 12:35:55.000000 granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.466108 granny-pliers-0.0.9/src/granny_pliers/tools/
+-rw-r--r--   0 pd         (501) staff       (20)      711 2023-06-10 13:15:39.000000 granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2271 2023-06-10 17:09:40.000000 granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.468181 granny-pliers-0.0.9/src/granny_pliers/web/
+-rw-r--r--   0 pd         (501) staff       (20)     1041 2023-06-10 13:18:21.000000 granny-pliers-0.0.9/src/granny_pliers/web/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     2135 2023-06-10 17:09:00.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     4235 2023-06-10 13:21:16.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py
+-rw-r--r--   0 pd         (501) staff       (20)    11869 2023-06-10 13:32:23.000000 granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py
+-rw-r--r--   0 pd         (501) staff       (20)     1499 2023-06-10 12:04:19.000000 granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.469771 granny-pliers-0.0.9/src/granny_pliers/worker/
+-rw-r--r--   0 pd         (501) staff       (20)      713 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py
+-rw-r--r--   0 pd         (501) staff       (20)     5086 2023-06-04 16:29:44.000000 granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py
+drwxr-xr-x   0 pd         (501) staff       (20)        0 2023-06-14 21:02:38.441760 granny-pliers-0.0.9/src/granny_pliers.egg-info/
+-rw-r--r--   0 pd         (501) staff       (20)    13700 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO
+-rw-r--r--   0 pd         (501) staff       (20)     2087 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt
+-rw-r--r--   0 pd         (501) staff       (20)        1 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/dependency_links.txt
+-rw-r--r--   0 pd         (501) staff       (20)      230 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/requires.txt
+-rw-r--r--   0 pd         (501) staff       (20)       14 2023-06-14 21:02:38.000000 granny-pliers-0.0.9/src/granny_pliers.egg-info/top_level.txt
```

### Comparing `granny-pliers-0.0.18/LICENSE` & `granny-pliers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/PKG-INFO` & `granny-pliers-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.18
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,22 +202,20 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://gitlab.com/stepanenko-family/shared/granny-pliers.git
-Project-URL: Documentation, https://gitlab.com/stepanenko-family/shared/granny-pliers.git
 Keywords: logging,configuration,tools,tool-belt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10.12
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Granny Pliers
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,13 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Granny Pliers is a Python library that contains a collection of useful
 and helpful tools, designed to simplify developers' lives."""
 
-__version__ = "0.0.18"
+__version__ = "0.0.9"
 __author__ = "Dmytro Stepanenko"
 __copyright__ = "Copyright 2022, Dmytro Stepanenko, Granny Pliers"
 __credits__ = ["Dmytro Stepanenko"]
 __license__ = "Apache License Version 2.0"
 __email__ = "dmitrijstepanenko@gmail.com"
-
-
-from .config import *
-from .logger import *
-from .worker import *
-
-__all__ = logger.__all__ + config.__all__ + worker.__all__
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/auth_config.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_config.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/auth_error.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 __all__ = ["AuthError"]
 
 
 @dataclass(repr=False, eq=False)
 class AuthError:
     """AuthError"""
-
     error: str
 
 
 @jsonplus.encoder("AuthError", predicate=lambda obj: isinstance(obj, AuthError), exact=False, priority=100)
 def auth_error_encoder(obj):
     """auth_error_encoder"""
     return asdict(obj)
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/auth_request.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_request.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/auth_response.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/auth_response.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/jwt.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/permissions.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/roles.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/roles.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/auth/rsa_codec.py` & `granny-pliers-0.0.9/src/granny_pliers/auth/rsa_codec.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/config/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/web/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""Configs"""
+"""WEB"""
 
-from .abstract_config import *
-from .autowired_config import *
-from .logger_config import *
-from .project_environment import *
+from .abstract_status_web_service import *
+from .abstract_web_application import *
+from .abstract_web_service import *
+from .web_application_config import *
 
-__all__ = abstract_config.__all__ + autowired_config.__all__ + logger_config.__all__ + project_environment.__all__
+__all__ = (
+    abstract_status_web_service.__all__  # pylint: disable=E0602
+    + abstract_web_application.__all__  # pylint: disable=E0602
+    + abstract_web_service.__all__  # pylint: disable=E0602
+    + web_application_config.__all__  # pylint: disable=E0602
+)
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/config/abstract_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/abstract_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """AbstractConfig"""
 import inspect
 import os
 import pathlib
 from abc import ABC
 from dataclasses import dataclass, fields
+from typing import Self
 
 import structlog
 import yaml
 
 __all__ = ["AbstractConfig", "ConfigError"]
 
 
@@ -52,15 +53,15 @@
 
             if (value := os.getenv(env_var_name, None)) is None:
                 continue
 
             setattr(self, field.name, field_meta_type(value))
 
     @classmethod
-    def load(cls, config_file: pathlib.Path) -> "AbstractConfig":
+    def load(cls, config_file: pathlib.Path) -> Self:
         """Load config"""
         log = structlog.get_logger(cls.__name__)
         log.info("Loading config from: %s", config_file)
         if not config_file.exists():
             msg = f"Can not load config from {str(config_file)}, file not found"
             log.error(msg)
             raise ConfigError(msg)
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/config/autowired_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/autowired_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,19 +37,14 @@
     )
 
     commit_branch: str = field(
         default=None,
         metadata={"env_var_name": "COMMIT_BRANCH", "type": str},
     )
 
-    commit_message: str = field(
-        default=None,
-        metadata={"env_var_name": "COMMIT_BRANCH_MESSAGE", "type": str},
-    )
-
     def __post_init__(self):
         super().__post_init__()
         self.environment = self.environment.lower()
         if self.commit_short_sha is not None:
             self.commit_short_sha = self.commit_short_sha.lower()
         if self.commit_branch is not None:
             self.commit_branch = self.commit_branch.lower()
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/config/logger_config.py` & `granny-pliers-0.0.9/src/granny_pliers/config/logger_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """LoggerConfig"""
-import logging
+
+import logging.config
 import sys
 from dataclasses import dataclass, field
-from logging import config
 
 import structlog
 
 from granny_pliers.logger import add_proc_name, add_logger_name
 from .abstract_config import AbstractConfig
 from .autowired_config import AutoWiredConfig
 from .project_environment import ProjectEnvironment
@@ -74,29 +74,19 @@
         super().__post_init__()
         if self.auto_wired is None:
             self.auto_wired = AutoWiredConfig()
 
         if self.log_level is None:
             self.log_level = self.get_log_level_from_env()
         elif isinstance(self.log_level, str):
-            self.log_level = {
-                "CRITICAL": logging.CRITICAL,
-                "FATAL": logging.FATAL,
-                "ERROR": logging.ERROR,
-                "WARN": logging.WARNING,
-                "WARNING": logging.WARNING,
-                "INFO": logging.INFO,
-                "DEBUG": logging.DEBUG,
-                "NOTSET": logging.NOTSET,
-            }.get(self.log_level.upper(), logging.INFO)
+            self.log_level = logging.getLevelNamesMapping()[self.log_level]
 
     def setup(self):
         """Initialize and setup logger"""
-
-        config.dictConfig(
+        logging.config.dictConfig(
             {
                 "version": 1,
                 "disable_existing_loggers": False,
                 "loggers": {
                     "": {
                         "level": self.log_level,
                         "handlers": [self.auto_wired.environment],
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/config/project_environment.py` & `granny-pliers-0.0.9/src/granny_pliers/config/project_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,13 +18,12 @@
 
 __all__ = ["ProjectEnvironment"]
 
 
 @unique
 class ProjectEnvironment(Enum):
     """ProjectEnvironment"""
-
     LOCAL = "local"
     DEV = "dev"
     STAGE = "stage"
     PROD = "prod"
     TEST = "test"
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/logger/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 """Logger - based on the structlog in addition colorized, includes extra
 meta info and can be printed in PLAIN or JSON formats"""
 
 from .abstract_logger import *
 from .log_processors import *
 
-__all__ = abstract_logger.__all__ + log_processors.__all__
+__all__ = abstract_logger.__all__ + log_processors.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/logger/abstract_logger.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/abstract_logger.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/logger/log_processors.py` & `granny-pliers-0.0.9/src/granny_pliers/logger/log_processors.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/auth/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """AUTH"""
 
 from .user import *
 
-__all__ = user.__all__
+__all__ = user.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/auth/user.py` & `granny-pliers-0.0.9/src/granny_pliers/models/auth/user.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import hashlib
 from dataclasses import dataclass
 from typing import Type, TypeVar
 
 from granny_pliers.orm import AbstractModel, AbstractMongoRepository, MongoConfig, BaseModel
 
 __all__ = ["User", "Users", "UserActivationRequest", "UserResetPasswordRequest", "UserSetPasswordRequest"]
-ModelT = TypeVar("ModelT")
+TModel = TypeVar("TModel")
 
 
 @dataclass(repr=False, eq=False)
 class User(AbstractModel):
     """User"""
 
     login: str = None
@@ -59,15 +59,15 @@
     secret: str = None
     token: str = None
 
 
 class Users(AbstractMongoRepository[User]):
     """Users"""
 
-    def __init__(self, config: MongoConfig, model_class: Type[ModelT] = None):
+    def __init__(self, config: MongoConfig, model_class: Type[TModel] = None):
         super().__init__(config, User if model_class is None else model_class)
 
     @property
     def collection_name(self) -> str:
         return "_users"
 
     @property
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/metrics/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""METRICS"""
+"""Tools"""
 
-from .confusion_matrix import *
+from .datetime_helper import *
 
-__all__ = confusion_matrix.__all__
+__all__ = datetime_helper.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/metrics/confusion_matrix.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/web/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/config/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,12 +8,20 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""WEB"""
+"""Configs"""
 
-from .web_service_health_status import *
+from .abstract_config import *
+from .autowired_config import *
+from .logger_config import *
+from .project_environment import *
 
-__all__ = web_service_health_status.__all__
+__all__ = (
+    abstract_config.__all__  # pylint: disable=E0602
+    + autowired_config.__all__  # pylint: disable=E0602
+    + logger_config.__all__  # pylint: disable=E0602
+    + project_environment.__all__  # pylint: disable=E0602
+)
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/models/web/web_service_health_status.py` & `granny-pliers-0.0.9/src/granny_pliers/models/web/web_service_health_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 class WebServiceHealthStatus(BaseModel):
     """WebServiceHealthStatus"""
 
     created_at: datetime = None
 
     environment: str = None
 
-    commit_short_sha: str = None
-    commit_branch: str = None
-    commit_message: str = None
+    ci_commit_short_sha: str = None
+
+    ci_commit_branch: str = None
 
     status: str = "Unknown"
 
     data: dict = field(default_factory=dict)
 
     system_name: str = None
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 from .abstract_http_repository import *
 from .abstract_model import *
 from .abstract_mongo_repository import *
 from .abstract_repository import *
 from .restful_http_client import *
 
 __all__ = (
-    abstract_model.__all__
-    + abstract_repository.__all__
-    + abstract_http_client.__all__
-    + abstract_mongo_repository.__all__
-    + restful_http_client.__all__
-    + abstract_http_repository.__all__
+    abstract_model.__all__  # pylint: disable=E0602
+    + abstract_repository.__all__  # pylint: disable=E0602
+    + abstract_http_client.__all__  # pylint: disable=E0602
+    + abstract_mongo_repository.__all__  # pylint: disable=E0602
+    + restful_http_client.__all__  # pylint: disable=E0602
+    + abstract_http_repository.__all__  # pylint: disable=E0602
 )
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/abstract_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/abstract_http_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_http_repository.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/abstract_model.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """BaseModel"""
 
 from dataclasses import dataclass, fields, field
 from datetime import datetime
-from enum import Enum
 from typing import TypeVar, Generic
 
 import jsonplus
 
 __all__ = ["BaseModel", "base_model_encoder", "AbstractModel", "ModelsPage", "ModelsCount"]
 
 from bson import ObjectId
@@ -51,15 +50,15 @@
 
     @id.setter
     def id(self, value: None | str | ObjectId):  # pylint: disable=C0103
         """id"""
         match value:
             case ObjectId():
                 self._id = value
-            case None | "None":
+            case None:
                 self._id = ObjectId()
             case str():
                 self._id = ObjectId() if value == "" else ObjectId(value)
 
     @property
     def created_at(self) -> datetime:
         """ObjectID"""
@@ -105,19 +104,13 @@
 
     :param obj:
     :return: dict
     """
     obj_dict = {}
     for cls_field in fields(obj):
         if cls_field.type is ObjectId:
-            value = str(getattr(obj, cls_field.name))
-            if value is None:
-                obj_dict[cls_field.name] = None
-            else:
-                obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
+            obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
         elif cls_field.type is tuple:
             obj_dict[cls_field.name] = str(getattr(obj, cls_field.name))
-        elif issubclass(cls_field.type, Enum):
-            obj_dict[cls_field.name] = getattr(obj, cls_field.name).value
         else:
             obj_dict[cls_field.name] = getattr(obj, cls_field.name)
     return obj_dict
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/abstract_mongo_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_mongo_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,20 +138,20 @@
         if self.__client is not None:
             self.__client.close()
             self.__client = None
 
     def _fallback_encoder(self, value):
         try:
             if isinstance(value, Enum):
-                return value.value
-            # Python datetime to BSON DateTime encoder
-            return setup_datetime(value)
+                return asdict(value.value)
+            else:
+                # Python datetime to BSON DateTime encoder
+                return setup_datetime(value)
         except TypeError as error:
             self.log.error("_fallback_encoder", error=error)
-        return None
 
     @staticmethod
     def parse_object_id(obj_id: Any):
         """parse ObjectId from any type"""
         if obj_id is None:
             return ObjectId()
 
@@ -179,22 +179,22 @@
         try:
             insert_result: InsertOneResult = await self.collection.insert_one(document=asdict(obj))
 
             if insert_result.acknowledged is None:
                 self.log.error("Can not save %s", self.model_class_name)
                 return None
 
-            result = await self.collection.find_one(filter=insert_result.inserted_id)
+            resource = await self.collection.find_one(filter=insert_result.inserted_id)
 
-            if result is None:
+            if resource is None:
                 self.log.error("Saved %s not found", self.model_class_name)
                 return None
             if verbose:
-                self.log.info("Saved %s: %s", self.model_class_name, result.get("_id", None))
-            return self.model_class(**self.filter_model_class_fields(result))
+                self.log.info("Saved %s: %s", self.model_class_name, resource.get("_id"))
+            return self.model_class(**resource)
 
         except (DuplicateKeyError, OperationFailure, TypeError) as error:
             self.log.error("Can not save %s", self.model_class_name, error=error)
             return None
 
     async def save_if_not_exists(self, obj: ModelT, conditions: dict = None) -> Optional[ModelT]:
         """save_if_not_exists"""
@@ -238,15 +238,15 @@
                 return_document=ReturnDocument.AFTER,
             )
 
             if result is None:
                 self.log.error("Can not update %s: %s", self.model_class_name, obj.id)
                 return None
             self.log.info("Updated %s: %s", self.model_class_name, obj.id)
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not update %s: %s", self.model_class_name, obj.id, error=error)
             return None
 
     async def update_many(self, objects: list[ModelT]) -> int:
         if len(objects) == 0:
             self.log.info("Updated 0 %ss", self.model_class_name)
@@ -293,15 +293,15 @@
                 return_document=ReturnDocument.AFTER,
             )
 
             if result is None:
                 self.log.error("Can not patch %s: %s", self.model_class_name, obj_id)
                 return None
             self.log.info("Patched %s: %s", self.model_class_name, obj_id)
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not patch %s", self.model_class_name, obj_id=obj_id, error=error)
             return None
 
     async def patch_many_by_id(self, obj_ids: list[Any], resources: dict) -> int:
         if len(obj_ids) == 0:
             self.log.info("Patched 0 %ss", self.model_class_name)
@@ -343,18 +343,18 @@
             return 0
 
         try:
             if soft:
                 result = await self.patch_many(objects, dict(is_deleted=True))
                 self.log.info("Soft Deleted %d %ss", result, self.model_class_name)
                 return result
-
-            result = await self.collection.bulk_write(list(map(lambda o: DeleteOne(dict(_id=o.id)), objects)))
-            self.log.info("Hard Deleted %d %ss", result.deleted_count, self.model_class_name)
-            return result.deleted_count
+            else:
+                result = await self.collection.bulk_write(list(map(lambda o: DeleteOne(dict(_id=o.id)), objects)))
+                self.log.info("Hard Deleted %d %ss", result.deleted_count, self.model_class_name)
+                return result.deleted_count
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not delete objects", self.model_class_name, error=error)
             return 0
 
     async def delete_by_id(self, obj_id: Any, soft: bool = True) -> Optional[ModelT]:
         try:
             mongo_obj_id = self.parse_object_id(obj_id)
@@ -365,19 +365,15 @@
                 result = await self.collection.find_one_and_delete(dict(_id=mongo_obj_id))
                 self.log.info("Hard deleted %s: %s", self.model_class_name, mongo_obj_id)
 
             if result is None:
                 self.log.error("Can not delete %s", self.model_class_name, obj_id=mongo_obj_id)
                 return None
 
-            return (
-                result
-                if isinstance(result, self._model_class)
-                else self.model_class(**self.filter_model_class_fields(result))
-            )
+            return result if isinstance(result, self._model_class) else self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not delete %s", self.model_class_name, obj_id=obj_id, error=error)
             return None
 
     async def delete_all(self, soft: bool = True) -> int:
         try:
             if soft:
@@ -389,38 +385,38 @@
 
                 if not result.acknowledged:
                     self.log.error("Cant soft delete %s", self.model_class_name)
                     return 0
 
                 self.log.info("Soft Deleted %d %ss", result.modified_count, self.model_class_name)
                 return result.modified_count
+            else:
+                result: DeleteResult = await self.collection.delete_many({})
 
-            result: DeleteResult = await self.collection.delete_many({})
-
-            if not result.acknowledged:
-                self.log.error("Cant delete %s", self.model_class_name)
-                return 0
-            self.log.info("Hard Deleted %d %ss", result.deleted_count, self.model_class_name)
+                if not result.acknowledged:
+                    self.log.error("Cant delete %s", self.model_class_name)
+                    return 0
+                self.log.info("Hard Deleted %d %ss", result.deleted_count, self.model_class_name)
 
-            return result.deleted_count
+                return result.deleted_count
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not delete many %s", self.model_class_name, error=error)
             return 0
 
     async def find(self, conditions: dict, verbose: bool = True) -> Optional[ModelT]:
         try:
             result = await self.collection.find_one(filter=conditions)
 
             if result is None:
                 return None
 
             if verbose:
                 self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
 
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error(
                 "Can not execute find for %s",
                 self.model_class_name,
                 conditions=conditions,
                 error=error,
             )
@@ -432,15 +428,15 @@
 
             result = await self.collection.find_one(filter=mongo_obj_id)
             if result is None:
                 self.log.info("Not found %s: %s", self.model_class_name, mongo_obj_id)
                 return None
 
             self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error(
                 "Can not execute find_by_id %s",
                 self.model_class_name,
                 obj_id=obj_id,
                 error=error,
             )
@@ -451,15 +447,15 @@
             result = await self.collection.find_one(filter=conditions, limit=1, sort=[("_id", -1)])
 
             if result is None:
                 self.log.info("Last not found %s, collection is empty", self.model_class_name)
                 return None
 
             self.log.info("Found %s: %s", self.model_class_name, result.get("_id"))
-            return self.model_class(**self.filter_model_class_fields(result))
+            return self.model_class(**result)
         except (OperationFailure, TypeError) as error:
             self.log.error("Can not find %s", self.model_class_name, error=error)
             return None
 
     async def count(self, conditions: dict = None) -> int:
         """
         Calculate number of objects
@@ -493,15 +489,15 @@
         limit = page_size
         try:
             cursor = self.collection.find(filter=conditions, skip=skip, limit=limit, sort=sort, projection=projection)
 
             result = await cursor.to_list(None)
             if verbose:
                 self.log.info("Found %d %ss", len(result), self.model_class_name)
-            return list(map(lambda t: self.model_class(**self.filter_model_class_fields(t)), result))
+            return list(map(lambda t: self.model_class(**t), result))
         except (OperationFailure, TypeError, Exception) as error:
             self.log.error("Can not find %s", self.model_class_name, error=error)
             return []
 
     @staticmethod
     def helper_symbol_date_condition(symbol: str, date: datetime) -> dict:
         """helper_symbol_date_condition"""
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/abstract_repository.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/abstract_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """Abstract Repository"""
 
 import abc
-from dataclasses import fields
 from types import TracebackType
 from typing import TypeVar, Generic, Optional, Any, Type
 
 from granny_pliers.logger import AbstractLogger
 
 __all__ = ["AbstractRepository"]
 ModelT = TypeVar("ModelT")
@@ -27,19 +26,14 @@
 
 class AbstractRepository(Generic[ModelT], AbstractLogger):
     """AbstractRepository"""
 
     def __init__(self, model_class: Type[ModelT]):
         super().__init__()
         self._model_class = model_class
-        self.model_class_fields_names = [f.name for f in fields(model_class)]
-
-    def filter_model_class_fields(self, resource: dict) -> dict:
-        """filter_model_class_fields"""
-        return {k: v for k, v in resource.items() if k in self.model_class_fields_names}
 
     async def __aenter__(self):
         """__aenter__"""
         return self
 
     async def __aexit__(
         self,
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/orm/restful_http_client.py` & `granny-pliers-0.0.9/src/granny_pliers/orm/restful_http_client.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/testing/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 #  limitations under the License.
 
 """Testing boilerplate"""
 
 from .abstract_test_case import *
 from .async_abstract_test_case import *
 
-__all__ = abstract_test_case.__all__ + async_abstract_test_case.__all__
+__all__ = abstract_test_case.__all__ + async_abstract_test_case.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/testing/abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/testing/async_abstract_test_case.py` & `granny-pliers-0.0.9/src/granny_pliers/testing/async_abstract_test_case.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/tools/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""Tools"""
+"""Workers"""
 
-from .datetime_helper import *
+from .abstract_worker import *
 
-__all__ = datetime_helper.__all__
+__all__ = abstract_worker.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/tools/datetime_helper.py` & `granny-pliers-0.0.9/src/granny_pliers/tools/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/web/abstract_status_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_status_web_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,17 +50,16 @@
         """routes"""
         return [web.get(self.path, self.get)]
 
     async def generate_status(self) -> WebServiceHealthStatus:
         """generate_status"""
         return WebServiceHealthStatus(
             environment=self.autowired_config.environment,
-            commit_branch=self.autowired_config.commit_branch,
-            commit_short_sha=self.autowired_config.commit_short_sha,
-            commit_message=self.autowired_config.commit_message,
+            ci_commit_branch=self.autowired_config.commit_branch,
+            ci_commit_short_sha=self.autowired_config.commit_short_sha,
             status="ok",
         )
 
     async def get(self, _) -> web.Response:
         """Get Service status
 
         :return: JSON - SSServiceHealthStatus
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/web/abstract_web_application.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_application.py`

 * *Files identical despite different names*

### Comparing `granny-pliers-0.0.18/src/granny_pliers/web/abstract_web_service.py` & `granny-pliers-0.0.9/src/granny_pliers/web/abstract_web_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,22 +115,18 @@
     @property
     def routes(self):
         """Defines default API endpoints"""
         return [
             web.get(self.path, self.get),
             web.post(self.path, self.post),
             web.get(self.path + "/count", self.count),
-            # web.put(self.path + r"/{id:[0-9a-f]{24}+}", self.put),
-            # web.get(self.path + r"/{id:[0-9a-f]{24}+}", self.get_one),
-            # web.patch(self.path + r"/{id:[0-9a-f]{24}+}", self.patch),
-            # web.delete(self.path + r"/{id:[0-9a-f]{24}+}", self.delete),
-            web.put(self.path + "/{id}", self.put),
-            web.get(self.path + "/{id}", self.get_one),
-            web.patch(self.path + "/{id}", self.patch),
-            web.delete(self.path + "/{id}", self.delete),
+            web.put(self.path + r"/{id:[0-9a-f]{24}+}", self.put),
+            web.get(self.path + r"/{id:[0-9a-f]{24}+}", self.get_one),
+            web.patch(self.path + r"/{id:[0-9a-f]{24}+}", self.patch),
+            web.delete(self.path + r"/{id:[0-9a-f]{24}+}", self.delete),
         ]
 
     @staticmethod
     def get_authenticated_user_id(request: web.Request) -> Optional[ObjectId]:
         """get_authenticated_user_id"""
         jwt_token: JwtToken = request.get("jwt_token_name", None)
         if jwt_token is None:
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/web/web_application_config.py` & `granny-pliers-0.0.9/src/granny_pliers/web/web_application_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 __all__ = ["WebApplicationConfig"]
 
 
 @dataclass()
 class WebApplicationConfig(AbstractConfig):
     """WebApplicationConfig"""
 
-    auth: AuthConfig = field(
-        default="localhost",
-        metadata={"type": AuthConfig},
-    )
+    auth: AuthConfig = None
 
     host: str = field(
         default="localhost",
         metadata={"env_var_name": "WEB_HOST", "type": str},
     )
     port: int = field(
         default=8080,
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/worker/__init__.py` & `granny-pliers-0.0.9/src/granny_pliers/models/metrics/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-"""Workers"""
+"""METRICS"""
 
-from .abstract_worker import *
+from .confusion_matrix import *
 
-__all__ = abstract_worker.__all__
+__all__ = confusion_matrix.__all__  # pylint: disable=E0602
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers/worker/abstract_worker.py` & `granny-pliers-0.0.9/src/granny_pliers/worker/abstract_worker.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,37 +36,27 @@
 
 class AbstractWorker(AbstractLogger, ABC):
     """AbstractWorker"""
 
     def __init__(self):
         super().__init__()
         self._loop = None
-        self._exit_code = 0
-
-    @property
-    def exit_code(self) -> int:
-        """Worker exit code"""
-        return self._exit_code
-
-    @exit_code.setter
-    def exit_code(self, value: int):
-        self._exit_code = value
 
     @property
     def loop(self):
         """event loop"""
         if self._loop is None:
             self._loop = asyncio.get_event_loop()
         return self._loop
 
     @abstractmethod
     async def _process(self):
         """Process body"""
 
-    def run(self) -> int:
+    def run(self) -> None:
         """main run loop"""
         name = multiprocessing.current_process().name
 
         if platform.system() == "Windows":
             signal.signal(signal.SIGINT, self.windows_graceful_shutdown)
             signal.signal(signal.SIGTERM, self.windows_graceful_shutdown)
         else:
@@ -75,24 +65,19 @@
 
         try:
             self.log.info("Initializing process %s...", name)
             self.loop.create_task(self._process())
             self.log.info("Process %s is started", name)
 
             self.loop.run_forever()
-        except Exception as error:
-            self.log.error("Unexpected error", error=error)
-            self.exit_code = 1
         finally:
             self.shutdown()
             self.log.info("Process %s is finished", name)
             self.loop.close()
 
-        return self.exit_code
-
     def shutdown(self):
         """Graceful process shutdown"""
         name = multiprocessing.current_process().name
         self.log.info("Shutting down %s ...", name)
         tasks = [task for task in asyncio.all_tasks(self.loop) if task is not asyncio.current_task(self.loop)]
         for task in tasks:
             task.cancel()
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers.egg-info/PKG-INFO` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: granny-pliers
-Version: 0.0.18
+Version: 0.0.9
 Summary: Set of tools
 Author-email: Dmytro Stepanenko <dmitrijstepanenko@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -202,22 +202,20 @@
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://gitlab.com/stepanenko-family/shared/granny-pliers.git
-Project-URL: Documentation, https://gitlab.com/stepanenko-family/shared/granny-pliers.git
 Keywords: logging,configuration,tools,tool-belt
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10.12
+Requires-Python: >=3.11.4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Granny Pliers
```

### Comparing `granny-pliers-0.0.18/src/granny_pliers.egg-info/SOURCES.txt` & `granny-pliers-0.0.9/src/granny_pliers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,14 @@
 src/granny_pliers/orm/__init__.py
 src/granny_pliers/orm/abstract_http_client.py
 src/granny_pliers/orm/abstract_http_repository.py
 src/granny_pliers/orm/abstract_model.py
 src/granny_pliers/orm/abstract_mongo_repository.py
 src/granny_pliers/orm/abstract_repository.py
 src/granny_pliers/orm/restful_http_client.py
-src/granny_pliers/scheduler/__init__.py
-src/granny_pliers/scheduler/abstract_schedule_object.py
-src/granny_pliers/scheduler/abstract_scheduler.py
-src/granny_pliers/scheduler/time_table.py
 src/granny_pliers/testing/__init__.py
 src/granny_pliers/testing/abstract_test_case.py
 src/granny_pliers/testing/async_abstract_test_case.py
 src/granny_pliers/tools/__init__.py
 src/granny_pliers/tools/datetime_helper.py
 src/granny_pliers/web/__init__.py
 src/granny_pliers/web/abstract_status_web_service.py
```

