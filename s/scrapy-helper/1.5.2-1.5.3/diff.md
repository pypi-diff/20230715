# Comparing `tmp/scrapy-helper-1.5.2.tar.gz` & `tmp/scrapy-helper-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-helper-1.5.2.tar", last modified: Thu Sep  8 05:41:24 2022, max compression
+gzip compressed data, was "scrapy-helper-1.5.3.tar", last modified: Sat Jul 15 13:46:26 2023, max compression
```

## Comparing `scrapy-helper-1.5.2.tar` & `scrapy-helper-1.5.3.tar`

### file list

```diff
@@ -1,30 +1,141 @@
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.807939 scrapy-helper-1.5.2/
--rw-r--r--   0 zhouping   (501) admin       (80)    11343 2022-09-08 01:14:06.000000 scrapy-helper-1.5.2/LICENSE
--rw-r--r--   0 zhouping   (501) admin       (80)       53 2022-09-08 03:55:43.000000 scrapy-helper-1.5.2/MANIFEST.in
--rw-r--r--   0 zhouping   (501) admin       (80)     1239 2022-09-08 05:41:24.807612 scrapy-helper-1.5.2/PKG-INFO
--rw-r--r--   0 zhouping   (501) admin       (80)       81 2022-09-08 03:13:02.000000 scrapy-helper-1.5.2/README.md
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.801830 scrapy-helper-1.5.2/scrapy_helper/
--rw-r--r--   0 zhouping   (501) admin       (80)       21 2022-09-08 03:29:44.000000 scrapy-helper-1.5.2/scrapy_helper/__init__.py
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.803851 scrapy-helper-1.5.2/scrapy_helper/__pycache__/
--rw-r--r--   0 zhouping   (501) admin       (80)      190 2022-09-08 05:39:20.000000 scrapy-helper-1.5.2/scrapy_helper/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.804641 scrapy-helper-1.5.2/scrapy_helper/core/
--rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-08 05:23:32.000000 scrapy-helper-1.5.2/scrapy_helper/core/__init__.py
--rwxr-xr-x   0 zhouping   (501) admin       (80)      748 2022-09-08 05:36:13.000000 scrapy-helper-1.5.2/scrapy_helper/core/utils.py
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.805112 scrapy-helper-1.5.2/scrapy_helper/middlewares/
--rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-08 03:57:34.000000 scrapy-helper-1.5.2/scrapy_helper/middlewares/__init__.py
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.806263 scrapy-helper-1.5.2/scrapy_helper/pipelines/
--rw-r--r--   0 zhouping   (501) admin       (80)       70 2022-09-08 05:20:10.000000 scrapy-helper-1.5.2/scrapy_helper/pipelines/__init__.py
--rwxr-xr-x   0 zhouping   (501) admin       (80)     1159 2022-09-06 01:02:25.000000 scrapy-helper-1.5.2/scrapy_helper/pipelines/mongodb.py
--rwxr-xr-x   0 zhouping   (501) admin       (80)     1656 2022-09-08 05:20:10.000000 scrapy-helper-1.5.2/scrapy_helper/pipelines/mysql.py
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.807193 scrapy-helper-1.5.2/scrapy_helper/spiders/
--rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-08 03:58:21.000000 scrapy-helper-1.5.2/scrapy_helper/spiders/__init__.py
--rwxr-xr-x   0 zhouping   (501) admin       (80)     4913 2022-09-08 05:36:13.000000 scrapy-helper-1.5.2/scrapy_helper/spiders/crawl.py
-drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2022-09-08 05:41:24.803589 scrapy-helper-1.5.2/scrapy_helper.egg-info/
--rw-r--r--   0 zhouping   (501) admin       (80)     1239 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/PKG-INFO
--rw-r--r--   0 zhouping   (501) admin       (80)      601 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/SOURCES.txt
--rw-r--r--   0 zhouping   (501) admin       (80)        1 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/dependency_links.txt
--rw-r--r--   0 zhouping   (501) admin       (80)        1 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/not-zip-safe
--rw-r--r--   0 zhouping   (501) admin       (80)       91 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/requires.txt
--rw-r--r--   0 zhouping   (501) admin       (80)       14 2022-09-08 05:41:24.000000 scrapy-helper-1.5.2/scrapy_helper.egg-info/top_level.txt
--rw-r--r--   0 zhouping   (501) admin       (80)       38 2022-09-08 05:41:24.808019 scrapy-helper-1.5.2/setup.cfg
--rw-r--r--   0 zhouping   (501) admin       (80)     1808 2022-09-08 03:48:14.000000 scrapy-helper-1.5.2/setup.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.251264 scrapy-helper-1.5.3/
+-rw-r--r--   0 zhouping   (501) admin       (80)    11343 2022-09-08 01:14:06.000000 scrapy-helper-1.5.3/LICENSE
+-rw-r--r--   0 zhouping   (501) admin       (80)       82 2022-09-27 12:27:33.000000 scrapy-helper-1.5.3/MANIFEST.in
+-rw-r--r--   0 zhouping   (501) admin       (80)     1397 2023-07-15 13:46:26.250817 scrapy-helper-1.5.3/PKG-INFO
+-rw-r--r--   0 zhouping   (501) admin       (80)      188 2022-09-22 08:05:24.000000 scrapy-helper-1.5.3/README.md
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.159638 scrapy-helper-1.5.3/scrapy_helper/
+-rw-r--r--   0 zhouping   (501) admin       (80)       21 2023-07-15 13:44:19.000000 scrapy-helper-1.5.3/scrapy_helper/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.163815 scrapy-helper-1.5.3/scrapy_helper/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      190 2022-09-08 07:17:37.000000 scrapy-helper-1.5.3/scrapy_helper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)      205 2023-07-15 13:46:25.000000 scrapy-helper-1.5.3/scrapy_helper/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.166039 scrapy-helper-1.5.3/scrapy_helper/core/
+-rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-08 05:23:32.000000 scrapy-helper-1.5.3/scrapy_helper/core/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.172237 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      174 2022-09-08 07:17:37.000000 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     4366 2022-09-20 09:04:44.000000 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/dict_path.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     1053 2022-10-10 07:34:43.000000 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/fast_item.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     6520 2022-09-15 06:37:57.000000 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/urls.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     2264 2022-10-10 07:34:43.000000 scrapy-helper-1.5.3/scrapy_helper/core/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     4523 2022-09-19 05:21:22.000000 scrapy-helper-1.5.3/scrapy_helper/core/dict_path.py
+-rw-r--r--   0 zhouping   (501) admin       (80)      502 2022-10-03 03:01:25.000000 scrapy-helper-1.5.3/scrapy_helper/core/fast_item.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     8617 2022-09-15 04:05:56.000000 scrapy-helper-1.5.3/scrapy_helper/core/urls.py
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     2180 2022-10-03 04:03:03.000000 scrapy-helper-1.5.3/scrapy_helper/core/utils.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.173782 scrapy-helper-1.5.3/scrapy_helper/linkextractors/
+-rw-r--r--   0 zhouping   (501) admin       (80)       42 2022-09-19 07:52:11.000000 scrapy-helper-1.5.3/scrapy_helper/linkextractors/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.175167 scrapy-helper-1.5.3/scrapy_helper/linkextractors/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      184 2022-09-09 07:23:40.000000 scrapy-helper-1.5.3/scrapy_helper/linkextractors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)      728 2022-09-09 07:23:40.000000 scrapy-helper-1.5.3/scrapy_helper/linkextractors/__pycache__/article.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)      341 2022-09-09 07:21:53.000000 scrapy-helper-1.5.3/scrapy_helper/linkextractors/article.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.175912 scrapy-helper-1.5.3/scrapy_helper/middlewares/
+-rw-r--r--   0 zhouping   (501) admin       (80)      279 2022-09-20 15:02:24.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.176350 scrapy-helper-1.5.3/scrapy_helper/middlewares/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      510 2022-09-21 12:00:49.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.180205 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/
+-rw-r--r--   0 zhouping   (501) admin       (80)      180 2022-09-19 06:29:55.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.185994 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      412 2022-09-20 09:46:22.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     1465 2022-09-20 09:46:22.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/cookies.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     2344 2022-09-20 13:27:18.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/persist_filter.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     1522 2022-09-20 09:46:22.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/proxy.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     3812 2022-09-20 09:46:23.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/pyppeteer_middleware.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     1587 2022-09-21 12:00:49.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/__pycache__/user_agent.cpython-310.pyc
+-rwxr-xr-x   0 zhouping   (501) admin       (80)      966 2023-04-03 01:01:16.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/cookies.py
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     1811 2022-11-10 04:04:54.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/persist_filter.py
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     1132 2022-09-19 01:08:24.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/proxy.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     4381 2022-09-08 08:16:35.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/pyppeteer_middleware.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     1209 2022-09-21 12:00:45.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/downloader/user_agent.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.187501 scrapy-helper-1.5.3/scrapy_helper/middlewares/spider/
+-rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-09 02:33:47.000000 scrapy-helper-1.5.3/scrapy_helper/middlewares/spider/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.192809 scrapy-helper-1.5.3/scrapy_helper/newspaper/
+-rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-15 03:31:37.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.204593 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      179 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     7138 2022-09-15 08:10:34.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/article.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     7831 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/cleaners.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     2553 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/configuration.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)    28163 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/extractors.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     6154 2022-09-15 08:25:24.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/outputformatters.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     8535 2022-09-15 08:29:03.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/parsers.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)      320 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     6820 2022-09-15 08:25:24.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/text.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     3565 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     8959 2022-09-15 08:10:33.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/article.py
+-rw-r--r--   0 zhouping   (501) admin       (80)    10419 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/cleaners.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     2657 2022-09-15 07:40:03.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/configuration.py
+-rw-r--r--   0 zhouping   (501) admin       (80)    41623 2022-09-15 06:53:36.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/extractors.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     5850 2022-09-15 08:25:23.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/outputformatters.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     7854 2022-09-15 08:28:09.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/parsers.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.156969 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.240557 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/
+-rw-r--r--   0 zhouping   (501) admin       (80)     1450 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-ar.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      936 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-be.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2409 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-bg.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      484 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-da.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     5967 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-de.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)    13903 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-el.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     3585 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-en.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2185 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-es.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      189 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-et.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     7710 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-fa.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      464 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-fi.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2002 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-fr.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1836 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-he.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2790 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-hi.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      870 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-hr.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2337 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-hu.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)    10499 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-id.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1696 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-it.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1006 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-ja.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      459 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-ko.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      763 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-lt.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1504 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-mk.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      587 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-nb.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      177 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-nl.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      513 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-no.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2015 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-pl.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     3610 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-pt.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1915 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-ro.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     4958 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-ru.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     2435 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-sl.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      776 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-sr.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     3956 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-sv.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      407 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-sw.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1420 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-th.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     1368 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-tr.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)     4029 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-uk.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      724 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-vi.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      623 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/resources/text/stopwords-zh.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)      138 2022-09-15 05:32:18.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/settings.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     5850 2023-03-23 01:54:52.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/text.py
+-rw-r--r--   0 zhouping   (501) admin       (80)     2451 2022-09-15 05:32:18.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/utils.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.242091 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/
+-rw-r--r--   0 zhouping   (501) admin       (80)        0 2022-09-15 05:11:00.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.244248 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      186 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     3724 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/__pycache__/extractors.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)      589 2022-09-15 07:54:06.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/__pycache__/videos.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     3793 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/extractors.py
+-rw-r--r--   0 zhouping   (501) admin       (80)      421 2022-09-08 09:09:26.000000 scrapy-helper-1.5.3/scrapy_helper/newspaper/videos/videos.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.245716 scrapy-helper-1.5.3/scrapy_helper/pipelines/
+-rw-r--r--   0 zhouping   (501) admin       (80)       70 2022-09-08 05:20:10.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.247775 scrapy-helper-1.5.3/scrapy_helper/pipelines/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      269 2022-09-20 09:04:45.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     1855 2022-09-27 13:35:21.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/__pycache__/mongodb.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     2017 2022-09-20 09:04:45.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/__pycache__/mysql.cpython-310.pyc
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     1454 2022-09-27 13:27:36.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/mongodb.py
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     3085 2022-11-10 08:42:01.000000 scrapy-helper-1.5.3/scrapy_helper/pipelines/mysql.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.248906 scrapy-helper-1.5.3/scrapy_helper/spiders/
+-rw-r--r--   0 zhouping   (501) admin       (80)       55 2022-09-19 06:18:40.000000 scrapy-helper-1.5.3/scrapy_helper/spiders/__init__.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.249972 scrapy-helper-1.5.3/scrapy_helper/spiders/__pycache__/
+-rw-r--r--   0 zhouping   (501) admin       (80)      245 2022-09-20 09:04:44.000000 scrapy-helper-1.5.3/scrapy_helper/spiders/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 zhouping   (501) admin       (80)     6931 2022-10-10 07:34:43.000000 scrapy-helper-1.5.3/scrapy_helper/spiders/__pycache__/crawl.cpython-310.pyc
+-rwxr-xr-x   0 zhouping   (501) admin       (80)     7409 2022-10-03 02:59:33.000000 scrapy-helper-1.5.3/scrapy_helper/spiders/crawl.py
+drwxr-xr-x   0 zhouping   (501) admin       (80)        0 2023-07-15 13:46:26.162431 scrapy-helper-1.5.3/scrapy_helper.egg-info/
+-rw-r--r--   0 zhouping   (501) admin       (80)     1397 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/PKG-INFO
+-rw-r--r--   0 zhouping   (501) admin       (80)     5845 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)        1 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)        1 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/not-zip-safe
+-rw-r--r--   0 zhouping   (501) admin       (80)      340 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/requires.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)       14 2023-07-15 13:46:26.000000 scrapy-helper-1.5.3/scrapy_helper.egg-info/top_level.txt
+-rw-r--r--   0 zhouping   (501) admin       (80)       38 2023-07-15 13:46:26.251413 scrapy-helper-1.5.3/setup.cfg
+-rw-r--r--   0 zhouping   (501) admin       (80)     1858 2023-07-15 10:08:57.000000 scrapy-helper-1.5.3/setup.py
```

### Comparing `scrapy-helper-1.5.2/LICENSE` & `scrapy-helper-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-helper-1.5.2/PKG-INFO` & `scrapy-helper-1.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-helper
-Version: 1.5.2
+Version: 1.5.3
 Summary: scrapy helper
 Author: Zhou Ping
 Author-email: 231409@qq.com
 License: Apache 2.0
 Keywords: scrapy,spider,helper
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,24 +14,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scrapy helper
 
 基于scrapy 的一些扩展
 
 
+docker build -t wisdom-env .
+
+python3 setup.py install
+
+docker-compose up -d
+docker-compose up -d --build
+
 ```
 pip install scrapy-helper
 ```
```

### Comparing `scrapy-helper-1.5.2/scrapy_helper/pipelines/mongodb.py` & `scrapy-helper-1.5.3/scrapy_helper/pipelines/mongodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,32 +2,37 @@
 from twisted.internet.threads import deferToThread
 
 
 class MongoDBPipeline(object):
     def __init__(self, mongodb_uri, mongodb_database):
         self.mongodb_uri = mongodb_uri
         self.mongodb_database = mongodb_database
-    
+
     @classmethod
     def from_crawler(cls, crawler):
         return cls(
             mongodb_uri=crawler.settings.get('MONGODB_URI'),
             mongodb_database=crawler.settings.get('MONGODB_DATABASE')
         )
-    
+
     def open_spider(self, spider):
         self.client = pymongo.MongoClient(self.mongodb_uri)
         self.database = self.client[self.mongodb_database]
-    
+
     def _process_item(self, item, spider):
         allowed_spiders = item.mongodb_spiders
         allowed_collections = item.mongodb_collections
         if allowed_spiders and spider.name in allowed_spiders:
             for allowed_collection in allowed_collections:
-                self.database[allowed_collection].insert(dict(item))
+                if item.unique_key and item.unique_identity:
+                    condition = {item.unique_key: item.get(item.unique_key), 'unique_identity': item.unique_identity}
+                    self.database[allowed_collection].update_one(condition, {'$set': dict(item)}, True)
+                else:
+                    self.database[allowed_collection].insert_one(dict(item))
+
         return item
-    
+
     def close_spider(self, spider):
         self.client.close()
-    
+
     def process_item(self, item, spider):
-        return deferToThread(self._process_item, item, spider)
+        return deferToThread(self._process_item, item, spider)
```

### Comparing `scrapy-helper-1.5.2/scrapy_helper/pipelines/mysql.py` & `scrapy-helper-1.5.3/scrapy_helper/pipelines/mysql.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,84 @@
 import pymysql
 from twisted.internet.threads import deferToThread
 
 
-class MySQLPipeline():
+class MySQLPipeline:
     def __init__(self, host, database, user, password, port):
         self.host = host
         self.database = database
         self.user = user
         self.password = password
         self.port = port
-    
+
     @classmethod
     def from_crawler(cls, crawler):
         return cls(
             host=crawler.settings.get('MYSQL_HOST'),
             database=crawler.settings.get('MYSQL_DATABASE'),
             user=crawler.settings.get('MYSQL_USER'),
             password=crawler.settings.get('MYSQL_PASSWORD'),
             port=crawler.settings.get('MYSQL_PORT'),
         )
-    
+
     def open_spider(self, spider):
         self.db = pymysql.connect(self.host, self.user, self.password, self.database, charset='utf8',
                                   port=self.port)
         self.cursor = self.db.cursor()
-    
+
     def close_spider(self, spider):
         self.db.close()
-    
+
+    def _has_dict_item(self, table, item):
+        where_strs = f"`unique_identity` = %s and `{item.unique_key}` = %s"
+        where_value_list = [item.unique_identity, item.get(item.unique_key)]
+        query = 'select %s from %s where %s' % (item.unique_key, table, where_strs)
+
+        self.cursor.execute(query, tuple(where_value_list))
+        rows = self.cursor.fetchone()
+
+        if rows:
+            return True
+        else:
+            return False
+
+    def _insert_dict_item(self, table, item):
+        data = dict(item)
+        keys = ', '.join(f'`{data.keys()}`')
+        values = ', '.join(['%s'] * len(data))
+        sql = 'insert into %s (%s) values (%s)' % (table, keys, values)
+        self.cursor.execute(sql, tuple(data.values()))
+        self.db.commit()
+
+    def _update_dict_item(self, table, item):
+        data = dict(item)
+        set_strs = []
+        set_values = []
+
+        for param, value in data.items():
+            set_strs.append(f'`{param}` = %s')
+            set_values.append(value)
+
+        where_strs = f"`unique_identity` = %s and `{item.unique_key}` = %s"
+        where_value_list = [item.unique_identity, data.get(item.unique_key)]
+
+        set_str = ', '.join(set_strs)
+        sql = "update %s set %s where %s" % (table, set_str, where_strs)
+        self.cursor.execute(sql, tuple(data.values()) + tuple(where_value_list))
+        self.db.commit()
+
     def _process_item(self, item, spider):
         allowed_spiders = item.mysql_spiders
         allowed_tables = item.mysql_tables
         if allowed_spiders and spider.name in allowed_spiders:
             for allowed_table in allowed_tables:
-                data = dict(item)
-                keys = ', '.join(data.keys())
-                values = ', '.join(['%s'] * len(data))
-                sql = 'insert into %s (%s) values (%s)' % (allowed_table, keys, values)
-                self.cursor.execute(sql, tuple(data.values()))
-                self.db.commit()
+                if item.unique_key and item.unique_identity:
+                    if self._has_dict_item(allowed_table, item):
+                        self._update_dict_item(allowed_table, item)
+                    else:
+                        self._insert_dict_item(allowed_table, item)
+                else:
+                    self._insert_dict_item(allowed_table, item)
         return item
-    
+
     def process_item(self, item, spider):
         return deferToThread(self._process_item, item, spider)
```

### Comparing `scrapy-helper-1.5.2/scrapy_helper/spiders/crawl.py` & `scrapy-helper-1.5.3/scrapy_helper/spiders/crawl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,56 @@
+import time
+
 from furl import furl
-from scrapy.spiders import CrawlSpider as BaseSpider, signals
 from scrapy import Request
-
+from scrapy.http import HtmlResponse
+from scrapy.spiders import CrawlSpider as BaseSpider, signals
 from scrapy.spiders.crawl import Rule as BaseRule
+from scrapy.utils.request import request_fingerprint
+from scrapy_helper.core.fast_item import FastItem
 
-from scrapy_helper.core.utils import str2body, str2dict, str2list
+from scrapy_helper.core.urls import get_domain
+from scrapy_helper.core.utils import str2body, str2dict, str2list, convert_to_html, convert_to_text
+from scrapy_helper.newspaper.article import Article
 
 
 class Rule(BaseRule):
-    def __init__(self, link_extractor, method='GET', data=None, params=None, headers=None,
-                 callback=None, cb_kwargs=None, follow=None, priority=0, dont_filter=False,
-                 meta=None, proxy=None, render=False, dont_redirect=None, dont_retry=None,
+    def __init__(self, link_extractor, callback=None, cb_kwargs=None, follow=None, process_links=None,
+                 process_request=None, errback=None,
+                 method='GET', params=None, process_body=None, data=None, headers=None,
+                 priority=0, dont_filter=False, cookies=None,
+                 meta=None, dont_redirect=None, dont_retry=None,
                  handle_httpstatus_list=None, handle_httpstatus_all=None,
                  dont_cache=None, dont_obey_robotstxt=None,
-                 download_timeout=None, max_retry_times=None,
-                 process_links=None, process_request=lambda x: x, process_body=None):
-        self.link_extractor = link_extractor
-        self.callback = callback
+                 download_timeout=None, max_retry_times=None, proxy=None, render=False, splash=None,
+                 persist_filter=False, extract_article=False):
+        super().__init__(link_extractor, callback, cb_kwargs, follow, process_links, process_request, errback)
+
         self.method = method
-        self.data = str2body(data)
         self.params = str2dict(params)
+        self.process_body = process_body
+        self.data = str2body(data)
         self.headers = str2dict(headers)
         self.priority = priority
         self.dont_filter = dont_filter
+        self.cookies = str2body(cookies)
         self.meta = str2dict(meta)
-        self.cb_kwargs = str2dict(cb_kwargs)
-        self.proxy = proxy
-        self.render = render
         self.dont_redirect = dont_redirect
         self.dont_retry = dont_retry
         self.handle_httpstatus_list = str2list(handle_httpstatus_list, lambda x: int(x))
         self.handle_httpstatus_all = handle_httpstatus_all
         self.dont_cache = dont_cache
         self.dont_obey_robotstxt = dont_obey_robotstxt
         self.download_timeout = download_timeout
         self.max_retry_times = max_retry_times
-        self.process_links = process_links
-        self.process_request = process_request
-        self.process_body = process_body
-        if follow is None:
-            self.follow = False if callback else True
-        else:
-            self.follow = follow
+        self.proxy = proxy
+        self.render = render
+        self.splash = str2body(splash)
+        self.persist_filter = persist_filter
+        self.extract_article = extract_article
 
     def __str__(self):
         """
         object to str
         :return:
         """
         return str(self.__dict__.items())
@@ -81,18 +86,18 @@
     def make_start_urls(self):
         """
         get start urls
         :return:
         """
         return self.start_urls
 
-    def _generate_request(self, index, rule, link, response):
+    def _generate_request(self, rule_index, rule, link, response):
         """
         generate request by rule
-        :param index: rule index
+        :param rule_index: rule index
         :param rule: rule object
         :param link: link object
         :return: new request object
         """
         url = furl(link.url).add(rule.params).url if rule.params else link.url
 
         # init request body
@@ -102,39 +107,91 @@
             # if process_body defined, use its result
             if callable(rule.process_body):
                 body = rule.process_body(response)
             # if data defined in rule, use data
             if rule.data:
                 body = rule.data
 
-        r = Request(url=url, method=rule.method, body=body, headers=rule.headers,
-                    priority=rule.priority,
-                    dont_filter=rule.dont_filter, callback=self._response_downloaded)
-
-        # update meta args
-        r.meta.update(**rule.meta)
-
+        meta = dict(**rule.meta)
         meta_items = ['dont_redirect', 'dont_retry', 'handle_httpstatus_list', 'handle_httpstatus_all',
-                      'dont_cache', 'dont_obey_robotstxt', 'download_timeout', 'max_retry_times', 'proxy', 'render']
+                      'dont_cache', 'dont_obey_robotstxt', 'download_timeout', 'max_retry_times', 'proxy', 'render',
+                      'splash', 'persist_filter', 'extract_article']
         meta_args = {meta_item: getattr(rule, meta_item) for meta_item in meta_items if
                      not getattr(rule, meta_item) is None}
-        # update extra meta args
-        r.meta.update(**meta_args)
+        meta.update(**meta_args)
+        meta.update(rule=rule_index, link_text=link.text)
+
+        r = Request(
+            url=url,
+            method=rule.method,
+            body=body,
+            headers=rule.headers,
+            cookies=rule.cookies,
+            priority=rule.priority,
+            dont_filter=rule.dont_filter,
+            callback=self._callback,
+            errback=self._errback,
+            meta=meta,
+        )
+
         return r
 
+    @staticmethod
+    def _get_request_fp(request):
+        return request.meta.get('request_fp') or request_fingerprint(request)
+
+    @staticmethod
+    def convert_to_html(element):
+        return convert_to_html(element)
+
+    @staticmethod
+    def convert_to_text(element):
+        return convert_to_text(element)
+
+    @staticmethod
+    def join_to_html(texts):
+        return convert_to_html(''.join(texts))
+
+    @staticmethod
+    def join_to_text(texts):
+        return convert_to_text(''.join(texts))
+
+    @staticmethod
+    def fast_item(*args: str):
+        _item = FastItem()
+        _item.set(args)
+        return _item
+
+    def _callback(self, response):
+        request_fp = self._get_request_fp(response.request)
+        request_domain = get_domain(response.url)
+        response.meta.update(request_fp=request_fp, request_domain=request_domain,
+                             insert_time=time.strftime('%Y-%m-%d %H:%M:%S'))
+
+        if response.meta['extract_article']:
+            article = Article(url=response.url, html=response.body)
+            article.parse()
+            response.meta.update(
+                article={"title": article.title, "text": article.text, "article_html": article.article_html,
+                         "images": article.images, "movies": article.movies, "tags": article.tags,
+                         "authors": article.authors, "top_img": article.top_img,
+                         "meta_img": article.meta_img, "meta_keywords": article.meta_keywords,
+                         "meta_description": article.meta_description, "meta_lang": article.meta_lang,
+                         "publish_date": article.publish_date, "meta_favicon": article.meta_favicon,
+                         "meta_site_name": article.meta_site_name, "meta_data": article.meta_data,
+                         "canonical_link": article.canonical_link})
+
+        rule = self._rules[response.meta['rule']]
+        return self._parse_response(response, rule.callback, rule.cb_kwargs, rule.follow)
+
     def _requests_to_follow(self, response):
-        """
-        requests to follow
-        :param response:
-        :return:
-        """
+        if not isinstance(response, HtmlResponse):
+            return
         seen = set()
-        for index, rule in enumerate(self._rules):
+        for rule_index, rule in enumerate(self._rules):
             links = [lnk for lnk in rule.link_extractor.extract_links(response)
                      if lnk not in seen]
-            if links and rule.process_links:
-                links = rule.process_links(links)
-            for link in links:
+            for link in rule.process_links(links):
                 seen.add(link)
-                # change _build_request to _generate_request
-                r = self._generate_request(index, rule, link, response)
-                yield rule.process_request(r)
+                # request = self._build_request(rule_index, link)
+                request = self._generate_request(rule_index, rule, link, response)
+                yield rule.process_request(request, response)
```

### Comparing `scrapy-helper-1.5.2/scrapy_helper.egg-info/PKG-INFO` & `scrapy-helper-1.5.3/scrapy_helper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-helper
-Version: 1.5.2
+Version: 1.5.3
 Summary: scrapy helper
 Author: Zhou Ping
 Author-email: 231409@qq.com
 License: Apache 2.0
 Keywords: scrapy,spider,helper
 Classifier: Framework :: Scrapy
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,24 +14,32 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scrapy helper
 
 基于scrapy 的一些扩展
 
 
+docker build -t wisdom-env .
+
+python3 setup.py install
+
+docker-compose up -d
+docker-compose up -d --build
+
 ```
 pip install scrapy-helper
 ```
```

### Comparing `scrapy-helper-1.5.2/setup.py` & `scrapy-helper-1.5.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     python_requires='>=3.7',
```

