# Comparing `tmp/souJpg-comm-1.1.0.tar.gz` & `tmp/souJpg-comm-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "souJpg-comm-1.1.0.tar", last modified: Tue Jul 11 09:36:44 2023, max compression
+gzip compressed data, was "souJpg-comm-1.1.3.tar", last modified: Fri Jul 14 22:55:47 2023, max compression
```

## Comparing `souJpg-comm-1.1.0.tar` & `souJpg-comm-1.1.3.tar`

### file list

```diff
@@ -1,61 +1,60 @@
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.217567 souJpg-comm-1.1.0/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1650 2023-07-11 09:36:44.217567 souJpg-comm-1.1.0/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.1.0/README.md
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-07-11 09:36:44.217567 souJpg-comm-1.1.0/setup.cfg
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      794 2023-07-11 09:35:57.000000 souJpg-comm-1.1.0/setup.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.197567 souJpg-comm-1.1.0/souJpg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      505 2023-05-07 01:53:29.000000 souJpg-comm-1.1.0/souJpg/__init__.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2689 2023-07-11 09:35:57.000000 souJpg-comm-1.1.0/souJpg/comm/apiResponse.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/cfg/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/cfg/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/cfg/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/cfg/vcgCfg.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/contextManagers.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2010 2023-07-11 09:35:57.000000 souJpg-comm-1.1.0/souJpg/comm/cos.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1383 2023-05-01 02:47:30.000000 souJpg-comm-1.1.0/souJpg/comm/dbHelper.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.1.0/souJpg/comm/dbsCL.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/decorators/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.1.0/souJpg/comm/decorators/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.1.0/souJpg/comm/decorators/base.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.1.0/souJpg/comm/decorators/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.1.0/souJpg/comm/decorators/methodRetry.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/es/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/es/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15100 2023-06-18 13:56:37.000000 souJpg-comm-1.1.0/souJpg/comm/es/es.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/es/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/es/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.1.0/souJpg/comm/es/test/test.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/fs/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/fs/__init__.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/fs/comm.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9783 2023-07-11 09:35:57.000000 souJpg-comm-1.1.0/souJpg/comm/fs/distributeFs.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/hdfsUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16709 2023-05-01 03:02:12.000000 souJpg-comm-1.1.0/souJpg/comm/imageUtils.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 02:47:39.000000 souJpg-comm-1.1.0/souJpg/comm/kafkaOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.1.0/souJpg/comm/labelUtils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/mathUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/ops/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/ops/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7766 2023-06-18 13:56:37.000000 souJpg-comm-1.1.0/souJpg/comm/ops/ops.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.207567 souJpg-comm-1.1.0/souJpg/comm/ops/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/ops/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.1.0/souJpg/comm/ops/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.1.0/souJpg/comm/projectUitls.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.1.0/souJpg/comm/redisOps.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.1.0/souJpg/comm/sparkApp.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.1.0/souJpg/comm/sparkBase.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.217567 souJpg-comm-1.1.0/souJpg/comm/test/
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/test/__init__.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    21234 2023-05-07 01:40:18.000000 souJpg-comm-1.1.0/souJpg/comm/test/test.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/threadPools.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/utils.py
--rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.1.0/souJpg/comm/vcgUtils.py
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2024 2023-05-07 01:50:41.000000 souJpg-comm-1.1.0/souJpg/comm/videoUtils.py
-drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-11 09:36:44.217567 souJpg-comm-1.1.0/souJpg_comm.egg-info/
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1650 2023-07-11 09:36:44.000000 souJpg-comm-1.1.0/souJpg_comm.egg-info/PKG-INFO
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1252 2023-07-11 09:36:44.000000 souJpg-comm-1.1.0/souJpg_comm.egg-info/SOURCES.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-07-11 09:36:44.000000 souJpg-comm-1.1.0/souJpg_comm.egg-info/dependency_links.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      508 2023-07-11 09:36:44.000000 souJpg-comm-1.1.0/souJpg_comm.egg-info/requires.txt
--rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-07-11 09:36:44.000000 souJpg-comm-1.1.0/souJpg_comm.egg-info/top_level.txt
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      333 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1316 2023-05-01 00:43:15.000000 souJpg-comm-1.1.3/README.md
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)       38 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/setup.cfg
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      806 2023-07-14 22:55:43.000000 souJpg-comm-1.1.3/setup.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.020915 souJpg-comm-1.1.3/souJpg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      505 2023-05-07 01:53:29.000000 souJpg-comm-1.1.3/souJpg/__init__.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.020915 souJpg-comm-1.1.3/souJpg/comm/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2781 2023-07-14 22:49:31.000000 souJpg-comm-1.1.3/souJpg/comm/apiResponse.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.020915 souJpg-comm-1.1.3/souJpg/comm/cfg/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/cfg/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2127 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/cfg/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      819 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/cfg/vcgCfg.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1603 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/contextManagers.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     2010 2023-07-11 09:35:57.000000 souJpg-comm-1.1.3/souJpg/comm/cos.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1383 2023-05-01 02:47:30.000000 souJpg-comm-1.1.3/souJpg/comm/dbHelper.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3816 2023-05-01 01:03:36.000000 souJpg-comm-1.1.3/souJpg/comm/dbsCL.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.020915 souJpg-comm-1.1.3/souJpg/comm/decorators/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 02:37:52.000000 souJpg-comm-1.1.3/souJpg/comm/decorators/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      264 2023-05-01 02:37:52.000000 souJpg-comm-1.1.3/souJpg/comm/decorators/base.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1071 2023-05-01 02:37:52.000000 souJpg-comm-1.1.3/souJpg/comm/decorators/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1747 2023-05-01 02:38:58.000000 souJpg-comm-1.1.3/souJpg/comm/decorators/methodRetry.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/es/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/es/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    15100 2023-06-18 13:56:37.000000 souJpg-comm-1.1.3/souJpg/comm/es/es.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/es/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/es/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7351 2023-05-01 01:12:39.000000 souJpg-comm-1.1.3/souJpg/comm/es/test/test.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/fs/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/fs/__init__.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/fs/comm.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     9783 2023-07-11 09:35:57.000000 souJpg-comm-1.1.3/souJpg/comm/fs/distributeFs.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4676 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/hdfsUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    16709 2023-05-01 03:02:12.000000 souJpg-comm-1.1.3/souJpg/comm/imageUtils.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     3719 2023-05-01 02:47:39.000000 souJpg-comm-1.1.3/souJpg/comm/kafkaOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    10938 2023-05-01 01:12:38.000000 souJpg-comm-1.1.3/souJpg/comm/labelUtils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1543 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/mathUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/ops/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/ops/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7766 2023-06-18 13:56:37.000000 souJpg-comm-1.1.3/souJpg/comm/ops/ops.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/ops/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/ops/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     6989 2023-05-01 01:12:39.000000 souJpg-comm-1.1.3/souJpg/comm/ops/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     1072 2023-05-01 01:12:38.000000 souJpg-comm-1.1.3/souJpg/comm/projectUitls.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3728 2023-05-01 01:12:39.000000 souJpg-comm-1.1.3/souJpg/comm/redisOps.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     3539 2023-05-01 01:12:37.000000 souJpg-comm-1.1.3/souJpg/comm/sparkApp.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     4623 2023-05-01 01:12:38.000000 souJpg-comm-1.1.3/souJpg/comm/sparkBase.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg/comm/test/
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/test/__init__.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)    21234 2023-05-07 01:40:18.000000 souJpg-comm-1.1.3/souJpg/comm/test/test.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)      277 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/threadPools.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      218 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/utils.py
+-rwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)     7924 2023-05-01 00:48:52.000000 souJpg-comm-1.1.3/souJpg/comm/vcgUtils.py
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     2024 2023-05-07 01:50:41.000000 souJpg-comm-1.1.3/souJpg/comm/videoUtils.py
+drwxr-xr-x   0 zhaoyufei  (1000) zhaoyufei  (1000)        0 2023-07-14 22:55:47.030915 souJpg-comm-1.1.3/souJpg_comm.egg-info/
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)      333 2023-07-14 22:55:46.000000 souJpg-comm-1.1.3/souJpg_comm.egg-info/PKG-INFO
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)     1218 2023-07-14 22:55:46.000000 souJpg-comm-1.1.3/souJpg_comm.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        1 2023-07-14 22:55:46.000000 souJpg-comm-1.1.3/souJpg_comm.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaoyufei  (1000) zhaoyufei  (1000)        7 2023-07-14 22:55:46.000000 souJpg-comm-1.1.3/souJpg_comm.egg-info/top_level.txt
```

### Comparing `souJpg-comm-1.1.0/README.md` & `souJpg-comm-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/setup.py` & `souJpg-comm-1.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
-with open(here / "requirements.txt", "r") as f:
-    requireds = f.read().splitlines()
+# with open(here / "requirements.txt", "r") as f:
+#     requireds = f.read().splitlines()
 
-with open(here / "README.md", "r") as f:
-    long_description = f.read()
+# with open(here / "README.md", "r") as f:
+#     long_description = f.read()
 
 setup(
     name="souJpg-comm",
-    version="1.1.0",
+    version="1.1.3",
     author="zhaoyufei",
     author_email="",
     description="souJpg-comm",
-    long_description=long_description,
+    # long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
-    install_requires=requireds,
+    # install_requires=requireds,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.8.10",
 )
```

### Comparing `souJpg-comm-1.1.0/souJpg/comm/apiResponse.py` & `souJpg-comm-1.1.3/souJpg/comm/apiResponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,25 @@
     error: Optional[str] = None
     errorCode: Optional[str] = None
 
     # async request related
     asyncRequestId: Optional[str] = None
     status: Optional[int] = None
     
-    
+    # 请求参数
     params: Optional[dict] = None
+    
+    
+    # 
+    
+    
+    leftQuota: Optional[int] = None
+    
+    
+    
 
 
 class ErrorCodeType(Enum):
 
     userRegisterError01 = "userRegisterError01"
     userRegisterError02 = "userRegisterError02"
     userLoginError01 = "userLoginError01"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `souJpg-comm-1.1.0/souJpg/comm/cfg/utils.py` & `souJpg-comm-1.1.3/souJpg/comm/cfg/utils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/cfg/vcgCfg.py` & `souJpg-comm-1.1.3/souJpg/comm/cfg/vcgCfg.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/contextManagers.py` & `souJpg-comm-1.1.3/souJpg/comm/contextManagers.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/cos.py` & `souJpg-comm-1.1.3/souJpg/comm/cos.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/dbHelper.py` & `souJpg-comm-1.1.3/souJpg/comm/dbHelper.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/dbsCL.py` & `souJpg-comm-1.1.3/souJpg/comm/dbsCL.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/decorators/comm.py` & `souJpg-comm-1.1.3/souJpg/comm/decorators/comm.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/decorators/methodRetry.py` & `souJpg-comm-1.1.3/souJpg/comm/decorators/methodRetry.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/es/es.py` & `souJpg-comm-1.1.3/souJpg/comm/es/es.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/es/test/test.py` & `souJpg-comm-1.1.3/souJpg/comm/es/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/fs/distributeFs.py` & `souJpg-comm-1.1.3/souJpg/comm/fs/distributeFs.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/hdfsUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/hdfsUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/imageUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/imageUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/kafkaOps.py` & `souJpg-comm-1.1.3/souJpg/comm/kafkaOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/labelUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/labelUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/mathUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/mathUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/ops/ops.py` & `souJpg-comm-1.1.3/souJpg/comm/ops/ops.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/ops/test/test.py` & `souJpg-comm-1.1.3/souJpg/comm/ops/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/projectUitls.py` & `souJpg-comm-1.1.3/souJpg/comm/projectUitls.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/redisOps.py` & `souJpg-comm-1.1.3/souJpg/comm/redisOps.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/sparkApp.py` & `souJpg-comm-1.1.3/souJpg/comm/sparkApp.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/sparkBase.py` & `souJpg-comm-1.1.3/souJpg/comm/sparkBase.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/test/test.py` & `souJpg-comm-1.1.3/souJpg/comm/test/test.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/vcgUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/vcgUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg/comm/videoUtils.py` & `souJpg-comm-1.1.3/souJpg/comm/videoUtils.py`

 * *Files identical despite different names*

### Comparing `souJpg-comm-1.1.0/souJpg_comm.egg-info/SOURCES.txt` & `souJpg-comm-1.1.3/souJpg_comm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,8 @@
 souJpg/comm/ops/test/__init__.py
 souJpg/comm/ops/test/test.py
 souJpg/comm/test/__init__.py
 souJpg/comm/test/test.py
 souJpg_comm.egg-info/PKG-INFO
 souJpg_comm.egg-info/SOURCES.txt
 souJpg_comm.egg-info/dependency_links.txt
-souJpg_comm.egg-info/requires.txt
 souJpg_comm.egg-info/top_level.txt
```

