# Comparing `tmp/hawthorn-0.0.3.tar.gz` & `tmp/hawthorn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hawthorn-0.0.3.tar", last modified: Tue Jan  3 09:53:25 2023, max compression
+gzip compressed data, was "hawthorn-0.0.4.tar", last modified: Sat Jul 15 17:24:47 2023, max compression
```

## Comparing `hawthorn-0.0.3.tar` & `hawthorn-0.0.4.tar`

### file list

```diff
@@ -1,62 +1,66 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.320898 hawthorn-0.0.3/
--rw-r--r--   0 kevin      (501) staff       (20)    35149 2022-11-20 07:26:03.000000 hawthorn-0.0.3/LICENSE
--rw-r--r--   0 kevin      (501) staff       (20)       30 2022-12-13 02:14:16.000000 hawthorn-0.0.3/MANIFEST.in
--rw-r--r--   0 kevin      (501) staff       (20)      494 2023-01-03 09:53:25.320534 hawthorn-0.0.3/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)       58 2022-11-20 07:26:03.000000 hawthorn-0.0.3/README.md
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.254837 hawthorn-0.0.3/hawthorn/
--rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-15 01:36:07.000000 hawthorn-0.0.3/hawthorn/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)    48320 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/amqplib.py
--rw-r--r--   0 kevin      (501) staff       (20)     7686 2022-12-13 07:27:18.000000 hawthorn-0.0.3/hawthorn/asynchttphandler.py
--rw-r--r--   0 kevin      (501) staff       (20)    15575 2022-12-17 16:46:49.000000 hawthorn-0.0.3/hawthorn/asyncrequest.py
--rw-r--r--   0 kevin      (501) staff       (20)    12464 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/cacheproxy.py
--rw-r--r--   0 kevin      (501) staff       (20)    77847 2022-12-17 16:40:06.000000 hawthorn-0.0.3/hawthorn/dbproxy.py
--rw-r--r--   0 kevin      (501) staff       (20)     6816 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/elasticsearchsaver.py
--rw-r--r--   0 kevin      (501) staff       (20)     4782 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/exceptionreporter.py
--rw-r--r--   0 kevin      (501) staff       (20)     1437 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/guniapp.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.271521 hawthorn-0.0.3/hawthorn/modelutils/
--rw-r--r--   0 kevin      (501) staff       (20)     4008 2022-12-28 01:30:49.000000 hawthorn-0.0.3/hawthorn/modelutils/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1853 2022-12-15 01:39:44.000000 hawthorn-0.0.3/hawthorn/modelutils/behaviors.py
--rw-r--r--   0 kevin      (501) staff       (20)     1226 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/registerroute.py
--rw-r--r--   0 kevin      (501) staff       (20)     1911 2022-11-20 09:40:23.000000 hawthorn-0.0.3/hawthorn/session.py
--rw-r--r--   0 kevin      (501) staff       (20)      302 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/singleton.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.272533 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/
--rw-r--r--   0 kevin      (501) staff       (20)       27 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.274044 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/asyncpg_migrate/
--rw-r--r--   0 kevin      (501) staff       (20)     4400 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/asyncpg_migrate/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.282533 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/
--rw-r--r--   0 kevin      (501) staff       (20)       82 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     3274 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/asyncio.py
--rw-r--r--   0 kevin      (501) staff       (20)    22769 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/base.py
--rw-r--r--   0 kevin      (501) staff       (20)      777 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/exc.py
--rw-r--r--   0 kevin      (501) staff       (20)      542 2022-11-20 07:43:33.000000 hawthorn-0.0.3/hawthorn/supports.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.286561 hawthorn-0.0.3/hawthorn/tornadoadapts/
--rw-r--r--   0 kevin      (501) staff       (20)       46 2022-11-20 14:54:20.000000 hawthorn-0.0.3/hawthorn/tornadoadapts/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      147 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/tornadoadapts/stack_context.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.290670 hawthorn-0.0.3/hawthorn/tornadozeep/
--rw-r--r--   0 kevin      (501) staff       (20)       65 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/tornadozeep/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      755 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/tornadozeep/bindings.py
--rw-r--r--   0 kevin      (501) staff       (20)     4601 2022-11-20 07:43:32.000000 hawthorn-0.0.3/hawthorn/tornadozeep/transport.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.319487 hawthorn-0.0.3/hawthorn/utilities/
--rw-r--r--   0 kevin      (501) staff       (20)     5210 2023-01-03 09:50:44.000000 hawthorn-0.0.3/hawthorn/utilities/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1237 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/aescoder.py
--rw-r--r--   0 kevin      (501) staff       (20)     1126 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/descoder.py
--rw-r--r--   0 kevin      (501) staff       (20)      288 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/fileutil.py
--rw-r--r--   0 kevin      (501) staff       (20)     4640 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/htmldocutils.py
--rw-r--r--   0 kevin      (501) staff       (20)     1000 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/img_utils.py
--rw-r--r--   0 kevin      (501) staff       (20)      638 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/iplist.py
--rw-r--r--   0 kevin      (501) staff       (20)      400 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/orderutil.py
--rw-r--r--   0 kevin      (501) staff       (20)     1236 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/restful_api.py
--rw-r--r--   0 kevin      (501) staff       (20)      610 2022-11-20 09:12:09.000000 hawthorn-0.0.3/hawthorn/utilities/rsacoder.py
--rw-r--r--   0 kevin      (501) staff       (20)     4428 2022-12-12 17:21:39.000000 hawthorn-0.0.3/hawthorn/utilities/signatureutils.py
--rw-r--r--   0 kevin      (501) staff       (20)      638 2022-11-20 09:12:10.000000 hawthorn-0.0.3/hawthorn/utilities/timeutil.py
--rw-r--r--   0 kevin      (501) staff       (20)     2721 2022-11-20 09:12:10.000000 hawthorn-0.0.3/hawthorn/utilities/work.py
--rw-r--r--   0 kevin      (501) staff       (20)     2844 2022-12-12 17:21:32.000000 hawthorn-0.0.3/hawthorn/utilities/xmlutil.py
--rw-r--r--   0 kevin      (501) staff       (20)      434 2022-12-15 01:36:46.000000 hawthorn-0.0.3/hawthorn/webapplication.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-01-03 09:53:25.268620 hawthorn-0.0.3/hawthorn.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)      494 2023-01-03 09:53:24.000000 hawthorn-0.0.3/hawthorn.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     1526 2023-01-03 09:53:24.000000 hawthorn-0.0.3/hawthorn.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2023-01-03 09:53:24.000000 hawthorn-0.0.3/hawthorn.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)      260 2023-01-03 09:53:24.000000 hawthorn-0.0.3/hawthorn.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)        9 2023-01-03 09:53:24.000000 hawthorn-0.0.3/hawthorn.egg-info/top_level.txt
--rw-r--r--   0 kevin      (501) staff       (20)       38 2023-01-03 09:53:25.321009 hawthorn-0.0.3/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)     1413 2023-01-03 09:52:51.000000 hawthorn-0.0.3/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.786264 hawthorn-0.0.4/
+-rw-r--r--   0 kevin      (501) staff       (20)    35149 2022-11-20 07:26:03.000000 hawthorn-0.0.4/LICENSE
+-rw-r--r--   0 kevin      (501) staff       (20)       30 2022-12-13 02:14:16.000000 hawthorn-0.0.4/MANIFEST.in
+-rw-r--r--   0 kevin      (501) staff       (20)      494 2023-07-15 17:24:47.785835 hawthorn-0.0.4/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)       58 2022-11-20 07:26:03.000000 hawthorn-0.0.4/README.md
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.597655 hawthorn-0.0.4/hawthorn/
+-rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-15 01:36:07.000000 hawthorn-0.0.4/hawthorn/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)    48320 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/amqplib.py
+-rw-r--r--   0 kevin      (501) staff       (20)     7686 2022-12-13 07:27:18.000000 hawthorn-0.0.4/hawthorn/asynchttphandler.py
+-rw-r--r--   0 kevin      (501) staff       (20)    15575 2022-12-17 16:46:49.000000 hawthorn-0.0.4/hawthorn/asyncrequest.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10089 2023-07-06 15:21:26.000000 hawthorn-0.0.4/hawthorn/cacheproxy.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.678323 hawthorn-0.0.4/hawthorn/cacher/
+-rw-r--r--   0 kevin      (501) staff       (20)       46 2023-07-06 13:09:33.000000 hawthorn-0.0.4/hawthorn/cacher/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5758 2023-07-06 15:28:47.000000 hawthorn-0.0.4/hawthorn/cacher/filecache.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3027 2023-07-06 13:36:53.000000 hawthorn-0.0.4/hawthorn/db2cachehelper.py
+-rw-r--r--   0 kevin      (501) staff       (20)    77847 2022-12-17 16:40:06.000000 hawthorn-0.0.4/hawthorn/dbproxy.py
+-rw-r--r--   0 kevin      (501) staff       (20)     6816 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/elasticsearchsaver.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4782 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/exceptionreporter.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1437 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/guniapp.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.680427 hawthorn-0.0.4/hawthorn/modelutils/
+-rw-r--r--   0 kevin      (501) staff       (20)     4008 2022-12-28 01:30:49.000000 hawthorn-0.0.4/hawthorn/modelutils/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1853 2022-12-15 01:39:44.000000 hawthorn-0.0.4/hawthorn/modelutils/behaviors.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1226 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/registerroute.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4228 2023-07-06 15:52:08.000000 hawthorn-0.0.4/hawthorn/session.py
+-rw-r--r--   0 kevin      (501) staff       (20)      302 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/singleton.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.681629 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/
+-rw-r--r--   0 kevin      (501) staff       (20)       27 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.682597 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/asyncpg_migrate/
+-rw-r--r--   0 kevin      (501) staff       (20)     4400 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/asyncpg_migrate/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.694173 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/
+-rw-r--r--   0 kevin      (501) staff       (20)       82 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     3274 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/asyncio.py
+-rw-r--r--   0 kevin      (501) staff       (20)    22769 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/base.py
+-rw-r--r--   0 kevin      (501) staff       (20)      777 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/exc.py
+-rw-r--r--   0 kevin      (501) staff       (20)      542 2022-11-20 07:43:33.000000 hawthorn-0.0.4/hawthorn/supports.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.758119 hawthorn-0.0.4/hawthorn/tornadoadapts/
+-rw-r--r--   0 kevin      (501) staff       (20)       46 2022-11-20 14:54:20.000000 hawthorn-0.0.4/hawthorn/tornadoadapts/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      147 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/tornadoadapts/stack_context.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.765348 hawthorn-0.0.4/hawthorn/tornadozeep/
+-rw-r--r--   0 kevin      (501) staff       (20)       65 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/tornadozeep/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      755 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/tornadozeep/bindings.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4601 2022-11-20 07:43:32.000000 hawthorn-0.0.4/hawthorn/tornadozeep/transport.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.784860 hawthorn-0.0.4/hawthorn/utilities/
+-rw-r--r--   0 kevin      (501) staff       (20)     5210 2023-01-03 09:50:44.000000 hawthorn-0.0.4/hawthorn/utilities/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1237 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/aescoder.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1126 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/descoder.py
+-rw-r--r--   0 kevin      (501) staff       (20)      288 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/fileutil.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4640 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/htmldocutils.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1000 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/img_utils.py
+-rw-r--r--   0 kevin      (501) staff       (20)      638 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/iplist.py
+-rw-r--r--   0 kevin      (501) staff       (20)      400 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/orderutil.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1236 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/restful_api.py
+-rw-r--r--   0 kevin      (501) staff       (20)      610 2022-11-20 09:12:09.000000 hawthorn-0.0.4/hawthorn/utilities/rsacoder.py
+-rw-r--r--   0 kevin      (501) staff       (20)     4428 2022-12-12 17:21:39.000000 hawthorn-0.0.4/hawthorn/utilities/signatureutils.py
+-rw-r--r--   0 kevin      (501) staff       (20)      638 2022-11-20 09:12:10.000000 hawthorn-0.0.4/hawthorn/utilities/timeutil.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2721 2022-11-20 09:12:10.000000 hawthorn-0.0.4/hawthorn/utilities/work.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2844 2022-12-12 17:21:32.000000 hawthorn-0.0.4/hawthorn/utilities/xmlutil.py
+-rw-r--r--   0 kevin      (501) staff       (20)      434 2022-12-15 01:36:46.000000 hawthorn-0.0.4/hawthorn/webapplication.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:24:47.674766 hawthorn-0.0.4/hawthorn.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)      494 2023-07-15 17:24:47.000000 hawthorn-0.0.4/hawthorn.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     1610 2023-07-15 17:24:47.000000 hawthorn-0.0.4/hawthorn.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-07-15 17:24:47.000000 hawthorn-0.0.4/hawthorn.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)      260 2023-07-15 17:24:47.000000 hawthorn-0.0.4/hawthorn.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        9 2023-07-15 17:24:47.000000 hawthorn-0.0.4/hawthorn.egg-info/top_level.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-07-15 17:24:47.786382 hawthorn-0.0.4/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     1413 2023-07-15 17:24:32.000000 hawthorn-0.0.4/setup.py
```

### Comparing `hawthorn-0.0.3/LICENSE` & `hawthorn-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/amqplib.py` & `hawthorn-0.0.4/hawthorn/amqplib.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/asynchttphandler.py` & `hawthorn-0.0.4/hawthorn/asynchttphandler.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/asyncrequest.py` & `hawthorn-0.0.4/hawthorn/asyncrequest.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/cacheproxy.py` & `hawthorn-0.0.4/hawthorn/cacheproxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 #!/usr/bin/env python
-#! -*- coding: utf-8 -*-
+# -*- coding: utf-8 -*-
 
-import redis
 import logging
 import datetime
 import tornado.gen
 import aredis
 
 from .supports import singleton
-from .modelutils import model_columns, format_mongo_value, DEFAULT_SKIP_FIELDS
-from .dbproxy import DbProxy
+from .modelutils import model_columns, DEFAULT_SKIP_FIELDS
+from .cacher.filecache import FileCache
 
 LOG = logging.getLogger('components.cacheproxy')
 
 @singleton
 class CacheProxy(object):
     """
     Cacher agent component
     """
 
     def __init__(self):
-        self.dbproxy = DbProxy()
-        self.async_redis_conn = None
+        self.cache_inst = None
     
-    def configure(self, redis_conf: dict) -> bool:
-        self.async_redis_conn = aredis.StrictRedis(host=redis_conf['host'], port=redis_conf['port'], 
-            db=redis_conf['db'], password=redis_conf['password'], retry_on_timeout=True)
+    def configure(self, conf: dict):
+        if conf.get('type', None) == 'redis':
+            self.configure_redis(conf)
+        elif conf.get('type', None) == 'file':
+            self.configure_filecache(conf.get('path', 'data/file-caching.db'))
+        else:
+            LOG.error('configure cacheproxy with configure:%s failed with unknown cache type', str(conf))
+    
+    def configure_redis(self, redis_conf: dict):
+        self.cache_inst = aredis.StrictRedis(host=redis_conf.get('host', 'localhost'), port=redis_conf.get('port', 6379), 
+            db=redis_conf.get('db', 0), password=redis_conf.get('password', None), retry_on_timeout=True)
         return True
+    
+    def configure_filecache(self, cache_path: str):
+        self.cache_inst = FileCache(cache_path)
 
     def prepare(self):
-        pass
+        if self.cache_inst == None:
+            self.configure_filecache('data/file-caching.db')
 
     @tornado.gen.coroutine
-    def getObject(self, key, keys):
+    def get_object(self, key, keys):
         self.prepare()
-        res = yield self.async_redis_conn.hmget(key, keys)
+        res = yield self.cache_inst.hmget(key, keys)
         if not res:
             return False
         result = {}
-        isAllNone = True
+        is_all_none = True
         i = 0
         for k in keys:
             v = res[i].decode() if isinstance(res[i], bytes) else res[i]
             result[k] = v
             i += 1
-            if isAllNone and v is not None:
-                isAllNone = False
-        if isAllNone:
+            if is_all_none and v is not None:
+                is_all_none = False
+        if is_all_none:
             result = False
         return result
     
     @tornado.gen.coroutine
-    def getObjects(self, key, keys):
+    def get_objects(self, key, keys):
         self.prepare()
         results = []
-        idxes = yield self.getSetsValues(key)
+        idxes = yield self.get_sets_values(key)
         for idx in idxes:
-            row = yield self.getObject(key+':'+idx, keys)
+            row = yield self.get_object(key+':'+idx, keys)
             if row is not False:
                 results.append(row)
         return results
 
     @tornado.gen.coroutine
-    def saveObject(self, key, mapping, expire=None):
+    def set_object(self, key, mapping, expire=None):
         if not mapping:
             return False
         for k,v in mapping.items():
             if v is None:
                 mapping[k] = ''
-        yield self.async_redis_conn.hmset(key, mapping)
-        if expire is not None:
-            yield self.async_redis_conn.expire(key, expire)
+        yield self.cache_inst.hmset(key, mapping, expire=expire)
         return True
 
     @tornado.gen.coroutine
-    def getSetsValues(self, key):
+    def get_sets_values(self, key):
         results = []
-        vals = yield self.async_redis_conn.smembers(key)
+        vals = yield self.cache_inst.smembers(key)
         if not vals:
             return results
         for val in vals:
             val = val.decode() if isinstance(val, bytes) else str(val)
             results.append(val)
         return results
 
     @tornado.gen.coroutine
-    def addSetsValue(self, key, value):
-        yield self.async_redis_conn.sadd(key, value)
+    def add_sets_values(self, key, value):
+        yield self.cache_inst.sadd(key, value)
         
     @tornado.gen.coroutine
-    def getSetsValuesExtend(self, key, keys):
-        vals = yield self.getSetsValues(key)
-        return self.parseImplodedValues(vals, keys)
+    def get_sets_values_extend(self, key, keys):
+        vals = yield self.get_sets_values(key)
+        return self.parse_imploded_values(vals, keys)
 
-    def parseImplodedValues(self, rows, keys):
+    def parse_imploded_values(self, rows, keys):
         results = []
         if not rows:
             return results
         l = len(keys)
         for val in rows:
             one = {k:'' for k in keys}
             i = 0
@@ -110,93 +118,93 @@
             if l > 0 and l2 > l:
                 for j in range(l2-l):
                     one[keys[l-1]] += '-' + eles[l+j]
             results.append(one)
         return results
         
     @tornado.gen.coroutine
-    def getSortedSetsValues(self, key):
+    def get_sorted_sets_values(self, key):
         results = []
         vals = yield self.zrange(key, 0, -1, withscores=True)
         if not vals:
             return results
         for ele in vals:
             val = ele[0]
             val = val.decode() if isinstance(val, bytes) else val
             results.append(val)
         return results
     
     @tornado.gen.coroutine
-    def getSortedSetsValuesExtend(self, key, keys):
-        vals = yield self.getSortedSetsValues(key)
-        return self.parseImplodedValues(vals, keys)
+    def get_sorted_sets_value_extend(self, key, keys):
+        vals = yield self.get_sorted_sets_values(key)
+        return self.parse_imploded_values(vals, keys)
 
     @tornado.gen.coroutine
-    def getCacheValue(self, key):
-        val = yield self.async_redis_conn.get(key)
+    def get_cache_value(self, key):
+        val = yield self.cache_inst.get(key)
         return val
 
     @tornado.gen.coroutine
-    def scanHashKeys(self, hashKey, keyMatch, count=1000, cursor=0):
-        res = yield self.async_redis_conn.hscan(hashKey, cursor, match=keyMatch, count=count)
+    def scan_hash_keys(self, hash_key, key_match, count=1000, cursor=0):
+        res = yield self.cache_inst.hscan(hash_key, cursor, match=key_match, count=count)
         keys = []
-        nextCursor = 0
+        next_cursor = 0
         if res:
-            nextCursor = res[0]
+            next_cursor = res[0]
             for k in res[1]:
                 keys.append(k.decode() if isinstance(k, bytes) else str(k))
-        return keys, nextCursor
+        return keys, next_cursor
     
     @tornado.gen.coroutine
-    def findHashKeys(self, hashKey, keyMatch, matchKeys = {}):
+    def find_hash_keys(self, hash_key, key_match, match_keys = {}):
         keys = []
-        if not hashKey or not keyMatch or not matchKeys:
+        if not hash_key or not key_match or not match_keys:
             return keys
-        nextCursor = -1
-        while nextCursor != 0:
-            if nextCursor == -1:
-                nextCursor = 0
-            scanedKeys, nextCursor = yield self.scanHashKeys(hashKey, keyMatch, cursor=nextCursor)
+        next_cursor = -1
+        while next_cursor != 0:
+            if next_cursor == -1:
+                next_cursor = 0
+            scanedKeys, next_cursor = yield self.scan_hash_keys(hash_key, key_match, cursor=next_cursor)
             for k in scanedKeys:
-                if k in matchKeys:
+                if k in match_keys:
                     keys.append(k)
         return keys
 
     @tornado.gen.coroutine
-    def getAllHashKeys(self, hashKeyPrefix, matchKeys = {}):
-        res = yield self.async_redis_conn.hgetall(hashKeyPrefix)
+    def get_all_hash_keys(self, hash_key_prefix, match_keys = {}):
+        res = yield self.cache_inst.hgetall(hash_key_prefix)
         result = []
         for row in res:
             a = row
         return result
         
     @tornado.gen.coroutine
-    def clearByKeyPrefix(self, keyPrefix):
-        keys = yield self.async_redis_conn.keys(keyPrefix+'*')
+    def clear_by_key_prefix(self, key_prefix):
+        keys = yield self.cache_inst.keys(key_prefix+'*')
         del_keys = [[]]
         i = 0
         for k in keys:
             del_keys[i].append(k.decode() if isinstance(k, bytes) else str(k))
             if len(del_keys[i]) > 50:
                 i += 1
                 del_keys.append([])
 
             if i > 10:
-                yield [self.async_redis_conn.delete(*dkeys) for dkeys in del_keys]
+                yield [self.cache_inst.delete(*dkeys) for dkeys in del_keys]
                 del_keys = [[]]
                 i = 0
         
         if del_keys[0]:
-            yield [self.async_redis_conn.delete(*dkeys) for dkeys in del_keys]
+            yield [self.cache_inst.delete(*dkeys) for dkeys in del_keys]
 
     @tornado.gen.coroutine
     def incr(self, key, expire = None):
-        yield self.async_redis_conn.incr(key)
+        yield self.cache_inst.incr(key)
         if expire:
-            yield self.async_redis_conn.expire(key, expire)
+            yield self.cache_inst.expire(key, expire)
 
     @tornado.gen.coroutine
     def set(self, key, value, expire = None, px=None, nx=False, xx=False):
         """
         Set the value at key ``name`` to ``value``
 
         ``expire`` sets an expire flag on key ``name`` for ``expire`` seconds.
@@ -205,24 +213,24 @@
 
         ``nx`` if set to True, set the value at key ``name`` to ``value`` only
             if it does not exist.
 
         ``xx`` if set to True, set the value at key ``name`` to ``value`` only
             if it already exists.
         """
-        yield self.async_redis_conn.set(key, value, ex=expire, px=px, nx=nx, xx=xx)
+        yield self.cache_inst.set(key, value, ex=expire, px=px, nx=nx, xx=xx)
 
     @tornado.gen.coroutine
     def get(self, key):
-        val = yield self.async_redis_conn.get(key)
+        val = yield self.cache_inst.get(key)
         return val
 
     @tornado.gen.coroutine
     def delete(self, key):
-        val = yield self.async_redis_conn.delete(key)
+        val = yield self.cache_inst.delete(key)
         return val
 
     @tornado.gen.coroutine
     def zrange(self, name, start, end, desc=False, withscores=False,
                score_cast_func=float):
         """
         Return a range of values from sorted set ``name`` between
@@ -233,126 +241,56 @@
         ``desc`` a boolean indicating whether to sort the results descendingly
 
         ``withscores`` indicates to return the scores along with the values.
         The return type is a list of (value, score) pairs
 
         ``score_cast_func`` a callable used to cast the score return value
         """
-        val = yield self.async_redis_conn.zrange(name, start, end, desc=desc, withscores=withscores, score_cast_func=score_cast_func)
+        val = yield self.cache_inst.zrange(name, start, end, desc=desc, withscores=withscores, score_cast_func=score_cast_func)
         return val
 
     @tornado.gen.coroutine
-    def isExistsInSets(self, key, value):
-        val = yield self.async_redis_conn.sismember(key, value)
+    def is_exists_in_sets(self, key, value):
+        val = yield self.cache_inst.sismember(key, value)
         return val
 
     @tornado.gen.coroutine
-    def loadMongoDataToCache(self, model, keyPrefix, pk, filters=None, excachecb=None, clearcache=True):
-        checkUniques = {}
-        @tornado.gen.coroutine
-        def _load_cache_pk(item):
-            cache_key = keyPrefix + self._getIndexKeyValue(item, pk)
-            if cache_key in checkUniques:
-                LOG.warning('loadToCache by key:%s that already exists.', cache_key)
-            checkUniques[cache_key] = 1
-            yield self.saveObject(cache_key, item)
-            if callable(excachecb):
-                yield excachecb(item, self.async_redis_conn)
-
-        if clearcache:
-            yield self.clearByKeyPrefix(keyPrefix)
-        yield self._loadDataFromMongoDb(model, _load_cache_pk, filters=filters)
-
-    @tornado.gen.coroutine
-    def loadMongoDataToCacheIndexedToMany(self, model, keyPrefix, indexKey, pk, filters=None, orderby=None, clearcache=True):
-        @tornado.gen.coroutine
-        def _load_cache_index(item):
-            yield self.addToCacheIndexedToMany(item, keyPrefix, indexKey, pk)
-        if clearcache:
-            yield self.clearByKeyPrefix(keyPrefix)
-        yield self._loadDataFromMongoDb(model, _load_cache_index, filters=filters, orderby=orderby)
-
-    @tornado.gen.coroutine
-    def addToCacheIndexedToMany(self, item, keyPrefix, indexKey, pk):
+    def add_to_cache_indexed_to_many(self, item, key_prefix, index_key, pk):
         if not isinstance(item, dict):
             item2 = item
             item = {}
             columns,_ = model_columns(item2)
             for k in columns:
                 if k not in DEFAULT_SKIP_FIELDS:
                     item[k] = getattr(item2, k)
-        pkValue = self._getIndexKeyValue(item, pk)
-        idxValue = self._getIndexKeyValue(item, indexKey)
-        cache_key = keyPrefix + idxValue
-        yield self.async_redis_conn.sadd(cache_key, pkValue)
-        cache_key += ':' + pkValue
-        yield self.saveObject(cache_key, item)
-
-    @tornado.gen.coroutine
-    def delFromCacheIndexedToMany(self, item, keyPrefix, indexKey, pk):
-        pkValue = self._getIndexKeyValue(item, pk)
-        idxValue = self._getIndexKeyValue(item, indexKey)
-        cache_key = keyPrefix + idxValue
-        yield self.async_redis_conn.srem(cache_key, pkValue)
-        cache_key += ':' + pkValue
-        yield self.async_redis_conn.delete(cache_key)
-
-    def _getIndexKeyValue(self, item, indexKey):
-        idxValue = ''
-        if isinstance(indexKey, list):
+        pk_value = self.get_index_key_value(item, pk)
+        idx_value = self.get_index_key_value(item, index_key)
+        cache_key = key_prefix + idx_value
+        yield self.cache_inst.sadd(cache_key, pk_value)
+        cache_key += ':' + pk_value
+        yield self.set_object(cache_key, item)
+
+    @tornado.gen.coroutine
+    def del_from_cache_indexed_to_many(self, item, key_prefix, index_key, pk):
+        pk_value = self.get_index_key_value(item, pk)
+        idx_value = self.get_index_key_value(item, index_key)
+        cache_key = key_prefix + idx_value
+        yield self.cache_inst.srem(cache_key, pk_value)
+        cache_key += ':' + pk_value
+        yield self.cache_inst.delete(cache_key)
+
+    def get_index_key_value(self, item, index_key):
+        idx_value = ''
+        if isinstance(index_key, list):
             vals = []
-            for k in indexKey:
+            for k in index_key:
                 if isinstance(item, dict):
                     vals.append(str(item[k]) if item[k] is not None else '')
                 else:
                     vals.append(str(getattr(item, k, '')))
-            idxValue = ':'.join(vals)
+            idx_value = ':'.join(vals)
         else:
             if isinstance(item, dict):
-                idxValue = str(item[indexKey] if item[indexKey] is not None else '')
+                idx_value = str(item[index_key] if item[index_key] is not None else '')
             else:
-                idxValue = str(getattr(item, indexKey, ''))
-        return idxValue
-
-    @tornado.gen.coroutine
-    def _loadDataFromMongoDb(self, model, cb, filters=None, orderby=None):
-        limit = 5000
-        offset = 0
-        nrows = limit
-        modelName = str(model.__name__)
-        LOG.info("loading %s from db begining", modelName)
-        qfilters = []
-        kwfilters = {}
-        curId = None
-        if isinstance(filters, tuple):
-            for f in filters:
-                if isinstance(f, dict):
-                    for k,v in f.items():
-                        kwfilters[k] = v
-                elif isinstance(f, list):
-                    for v in f:
-                        qfilters.append(v)
-        elif isinstance(filters, dict):
-            kwfilters = filters
-        elif isinstance(filters, list):
-            qfilters = filters
-        while nrows >= limit:
-            if curId:
-                kwfilters['id__gt'] = curId
-            rows = yield self.dbproxy.query_all_mongo(model, (qfilters, kwfilters), limit)
-            nrows = 0
-            for row in rows:
-                nrows += 1
-                curId = row.get('id')
-                item = {}
-                for k in row:
-                    if k in DEFAULT_SKIP_FIELDS:
-                        continue
-                    item[k] = format_mongo_value(row.get(k))
-                if tornado.gen.is_coroutine_function(cb):
-                    yield cb(item)
-                else:
-                    cb(item)
-            offset += nrows
-            LOG.info("loading %s from db offset:%d rows:%d", modelName, offset, nrows)
-        
-        LOG.info("loading %s from db finished", modelName)
+                idx_value = str(getattr(item, index_key, ''))
+        return idx_value
```

### Comparing `hawthorn-0.0.3/hawthorn/dbproxy.py` & `hawthorn-0.0.4/hawthorn/dbproxy.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/elasticsearchsaver.py` & `hawthorn-0.0.4/hawthorn/elasticsearchsaver.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/exceptionreporter.py` & `hawthorn-0.0.4/hawthorn/exceptionreporter.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/guniapp.py` & `hawthorn-0.0.4/hawthorn/guniapp.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/modelutils/__init__.py` & `hawthorn-0.0.4/hawthorn/modelutils/__init__.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/modelutils/behaviors.py` & `hawthorn-0.0.4/hawthorn/modelutils/behaviors.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/registerroute.py` & `hawthorn-0.0.4/hawthorn/registerroute.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/asyncpg_migrate/__init__.py` & `hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/asyncpg_migrate/__init__.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/asyncio.py` & `hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/asyncio.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/base.py` & `hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/base.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/sqlalchemy_dialects/sync_threading/exc.py` & `hawthorn-0.0.4/hawthorn/sqlalchemy_dialects/sync_threading/exc.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/supports.py` & `hawthorn-0.0.4/hawthorn/supports.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/tornadozeep/bindings.py` & `hawthorn-0.0.4/hawthorn/tornadozeep/bindings.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/tornadozeep/transport.py` & `hawthorn-0.0.4/hawthorn/tornadozeep/transport.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/__init__.py` & `hawthorn-0.0.4/hawthorn/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/aescoder.py` & `hawthorn-0.0.4/hawthorn/utilities/aescoder.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/descoder.py` & `hawthorn-0.0.4/hawthorn/utilities/descoder.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/htmldocutils.py` & `hawthorn-0.0.4/hawthorn/utilities/htmldocutils.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/img_utils.py` & `hawthorn-0.0.4/hawthorn/utilities/img_utils.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/iplist.py` & `hawthorn-0.0.4/hawthorn/utilities/iplist.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/restful_api.py` & `hawthorn-0.0.4/hawthorn/utilities/restful_api.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/rsacoder.py` & `hawthorn-0.0.4/hawthorn/utilities/rsacoder.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/signatureutils.py` & `hawthorn-0.0.4/hawthorn/utilities/signatureutils.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/timeutil.py` & `hawthorn-0.0.4/hawthorn/utilities/timeutil.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/work.py` & `hawthorn-0.0.4/hawthorn/utilities/work.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn/utilities/xmlutil.py` & `hawthorn-0.0.4/hawthorn/utilities/xmlutil.py`

 * *Files identical despite different names*

### Comparing `hawthorn-0.0.3/hawthorn.egg-info/SOURCES.txt` & `hawthorn-0.0.4/hawthorn.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,28 +3,31 @@
 README.md
 setup.py
 hawthorn/__init__.py
 hawthorn/amqplib.py
 hawthorn/asynchttphandler.py
 hawthorn/asyncrequest.py
 hawthorn/cacheproxy.py
+hawthorn/db2cachehelper.py
 hawthorn/dbproxy.py
 hawthorn/elasticsearchsaver.py
 hawthorn/exceptionreporter.py
 hawthorn/guniapp.py
 hawthorn/registerroute.py
 hawthorn/session.py
 hawthorn/singleton.py
 hawthorn/supports.py
 hawthorn/webapplication.py
 hawthorn.egg-info/PKG-INFO
 hawthorn.egg-info/SOURCES.txt
 hawthorn.egg-info/dependency_links.txt
 hawthorn.egg-info/requires.txt
 hawthorn.egg-info/top_level.txt
+hawthorn/cacher/__init__.py
+hawthorn/cacher/filecache.py
 hawthorn/modelutils/__init__.py
 hawthorn/modelutils/behaviors.py
 hawthorn/sqlalchemy_dialects/__init__.py
 hawthorn/sqlalchemy_dialects/asyncpg_migrate/__init__.py
 hawthorn/sqlalchemy_dialects/sync_threading/__init__.py
 hawthorn/sqlalchemy_dialects/sync_threading/asyncio.py
 hawthorn/sqlalchemy_dialects/sync_threading/base.py
```

### Comparing `hawthorn-0.0.3/setup.py` & `hawthorn-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="hawthorn",
-    version="0.0.3",
+    version="0.0.4",
     author="kevinyjn",
     author_email="kevinyjn@gmail.com",
     description="common python programing encapsulation library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/libpub/hawthorn",
     packages=setuptools.find_packages(exclude=[".tests", ".tests.", "tests.*", "tests"]),
```

