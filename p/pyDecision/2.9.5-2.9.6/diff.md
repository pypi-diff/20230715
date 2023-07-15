# Comparing `tmp/pyDecision-2.9.5.tar.gz` & `tmp/pyDecision-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-2.9.5.tar", last modified: Sat Jul 15 00:22:30 2023, max compression
+gzip compressed data, was "dist\pyDecision-2.9.6.tar", last modified: Sat Jul 15 00:28:12 2023, max compression
```

## Comparing `pyDecision-2.9.5.tar` & `pyDecision-2.9.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 00:22:30.000000 pyDecision-2.9.5/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-2.9.5/LICENSE
--rw-rw-rw-   0        0        0    12492 2023-07-15 00:22:30.000000 pyDecision-2.9.5/PKG-INFO
--rw-rw-rw-   0        0        0    12099 2023-07-14 22:31:57.000000 pyDecision-2.9.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-2.9.5/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     1835 2023-07-14 22:26:21.000000 pyDecision-2.9.5/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-2.9.5/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-2.9.5/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-2.9.5/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-2.9.5/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-2.9.5/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-2.9.5/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-2.9.5/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-2.9.5/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-2.9.5/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-2.9.5/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-2.9.5/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-2.9.5/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-2.9.5/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-2.9.5/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-2.9.5/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-2.9.5/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-2.9.5/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-2.9.5/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-2.9.5/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-2.9.5/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-2.9.5/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-2.9.5/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-2.9.5/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-2.9.5/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-2.9.5/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2915 2023-07-15 00:21:11.000000 pyDecision-2.9.5/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-2.9.5/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-2.9.5/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-2.9.5/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-2.9.5/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2372 2023-07-15 00:22:05.000000 pyDecision-2.9.5/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-2.9.5/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-2.9.5/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-2.9.5/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-2.9.5/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-2.9.5/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-2.9.5/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-2.9.5/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-2.9.5/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-2.9.5/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-2.9.5/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-2.9.5/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-2.9.5/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-2.9.5/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-2.9.5/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision/util/
--rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-2.9.5/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-2.9.5/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-2.9.5/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    12492 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 00:22:30.000000 pyDecision-2.9.5/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 00:22:30.000000 pyDecision-2.9.5/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-15 00:22:17.000000 pyDecision-2.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:28:12.000000 pyDecision-2.9.6/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-2.9.6/LICENSE
+-rw-rw-rw-   0        0        0    12492 2023-07-15 00:28:12.000000 pyDecision-2.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0    12099 2023-07-14 22:31:57.000000 pyDecision-2.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 00:28:12.000000 pyDecision-2.9.6/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-2.9.6/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:28:12.000000 pyDecision-2.9.6/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     1835 2023-07-14 22:26:21.000000 pyDecision-2.9.6/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-2.9.6/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-2.9.6/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-2.9.6/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-2.9.6/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-2.9.6/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-2.9.6/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-2.9.6/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-2.9.6/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-2.9.6/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-2.9.6/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-2.9.6/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-2.9.6/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-2.9.6/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-2.9.6/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-2.9.6/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-2.9.6/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-2.9.6/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-2.9.6/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-2.9.6/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-2.9.6/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-2.9.6/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-2.9.6/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-2.9.6/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-2.9.6/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-2.9.6/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2935 2023-07-15 00:27:34.000000 pyDecision-2.9.6/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-2.9.6/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-2.9.6/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-2.9.6/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-2.9.6/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2408 2023-07-15 00:27:34.000000 pyDecision-2.9.6/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-2.9.6/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-2.9.6/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-2.9.6/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-2.9.6/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-2.9.6/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-2.9.6/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-2.9.6/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-2.9.6/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-2.9.6/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-2.9.6/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-2.9.6/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-2.9.6/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-2.9.6/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-2.9.6/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:28:12.000000 pyDecision-2.9.6/pyDecision/util/
+-rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-2.9.6/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-2.9.6/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-2.9.6/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:28:12.000000 pyDecision-2.9.6/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    12492 2023-07-15 00:28:11.000000 pyDecision-2.9.6/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2023-07-15 00:28:12.000000 pyDecision-2.9.6/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 00:28:11.000000 pyDecision-2.9.6/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-15 00:28:11.000000 pyDecision-2.9.6/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 00:28:11.000000 pyDecision-2.9.6/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 00:28:12.000000 pyDecision-2.9.6/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-07-15 00:27:54.000000 pyDecision-2.9.6/setup.py
```

### Comparing `pyDecision-2.9.5/LICENSE` & `pyDecision-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/PKG-INFO` & `pyDecision-2.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.5
+Version: 2.9.6
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-2.9.5/README.md` & `pyDecision-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/__init__.py` & `pyDecision-2.9.6/pyDecision/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/ahp.py` & `pyDecision-2.9.6/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/aras.py` & `pyDecision-2.9.6/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/borda.py` & `pyDecision-2.9.6/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/bwm.py` & `pyDecision-2.9.6/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/cocoso.py` & `pyDecision-2.9.6/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/codas.py` & `pyDecision-2.9.6/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/copras.py` & `pyDecision-2.9.6/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/critic.py` & `pyDecision-2.9.6/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/dematel.py` & `pyDecision-2.9.6/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_i.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_i_s.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_i_v.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_ii.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_iii.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_iv.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/e_tri_b.py` & `pyDecision-2.9.6/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/edas.py` & `pyDecision-2.9.6/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-2.9.6/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-2.9.6/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-2.9.6/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-2.9.6/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-2.9.6/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/gra.py` & `pyDecision-2.9.6/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/idocriw.py` & `pyDecision-2.9.6/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/mabac.py` & `pyDecision-2.9.6/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/marcos.py` & `pyDecision-2.9.6/pyDecision/algorithm/marcos.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             worst[j] = worst[j] / best[j]
             best[j]  = best[j]  / best[j]
         else:
             X[:,j]   =  best[j] / X[:,j]
             worst[j] = best[j]  / worst[j]
             best[j]  = best[j]  / best[j]
     for i in range(0, X.shape[1]):
-        best[i]  = best[i]  * weights[i]
-        worst[i] = worst[i] * weights[i]
+        best[i]  = best[i]  * np.array(weights[i])
+        worst[i] = worst[i] * np.array(weights[i])
     V     = X * np.array(weights)
     S     = V.sum(axis = 1)
     k_n   = S / np.sum(worst)
     k_p   = S / np.sum(best)
     f_k_n = k_p / (k_p + k_n)
     f_k_p = k_n / (k_p + k_n)
     f_k   = (k_p + k_n) / (1 + ((1 - f_k_p) / f_k_p) + ((1 - f_k_n) / f_k_n))
```

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/maut.py` & `pyDecision-2.9.6/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/moora.py` & `pyDecision-2.9.6/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/moosra.py` & `pyDecision-2.9.6/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/multimoora.py` & `pyDecision-2.9.6/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/ocra.py` & `pyDecision-2.9.6/pyDecision/algorithm/ocra.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     n, m  = dataset.shape
     I     = np.zeros(n)
     O     = np.zeros(n)    
     for j in range(0, m):
         if (criterion_type[j] == 'max'):
             A = (X[:,j] - np.min(X[:,j])) / np.min(X[:,j])
             for k in range(0, A.shape[0]):
-                A = A*weights[k]
+                A[k] = A[k] * np.array(weights[k])
             O = O + A
         else:
             B = (np.max(X[:,j]) - X[:,j]) / np.min(X[:,j])
             for k in range(0, B.shape[0]):
-                B = B*weights[k]
+                B[k] = B[k] * np.array(weights[k])
             I = I + B
     O = O - np.min(O)
     I = I - np.min(I)
     r = (I + O) - np.min(I + O)
     for i in range(0, r.shape[0]):
         print('a' + str(i+1) + ': ' + str(round(r[i], 2)))
     if ( graph == True):
```

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_i.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_ii.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_iii.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_iv.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_v.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_vi.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/p_xgaia.py` & `pyDecision-2.9.6/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/saw.py` & `pyDecision-2.9.6/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/smart.py` & `pyDecision-2.9.6/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/todim.py` & `pyDecision-2.9.6/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/topsis.py` & `pyDecision-2.9.6/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/vikor.py` & `pyDecision-2.9.6/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/waspas.py` & `pyDecision-2.9.6/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/algorithm/wings.py` & `pyDecision-2.9.6/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/util/ga.py` & `pyDecision-2.9.6/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision/util/gwo.py` & `pyDecision-2.9.6/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/pyDecision.egg-info/PKG-INFO` & `pyDecision-2.9.6/pyDecision.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.5
+Version: 2.9.6
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyDecision-2.9.5/pyDecision.egg-info/SOURCES.txt` & `pyDecision-2.9.6/pyDecision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.5/setup.py` & `pyDecision-2.9.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='2.9.5',
+    version='2.9.6',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

