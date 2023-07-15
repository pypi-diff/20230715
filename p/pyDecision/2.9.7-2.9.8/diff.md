# Comparing `tmp/pyDecision-2.9.7.tar.gz` & `tmp/pyDecision-2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-2.9.7.tar", last modified: Sat Jul 15 00:39:29 2023, max compression
+gzip compressed data, was "dist\pyDecision-2.9.8.tar", last modified: Sat Jul 15 01:33:29 2023, max compression
```

## Comparing `pyDecision-2.9.7.tar` & `pyDecision-2.9.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 00:39:29.000000 pyDecision-2.9.7/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-2.9.7/LICENSE
--rw-rw-rw-   0        0        0    12492 2023-07-15 00:39:29.000000 pyDecision-2.9.7/PKG-INFO
--rw-rw-rw-   0        0        0    12099 2023-07-14 22:31:57.000000 pyDecision-2.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-2.9.7/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:39:29.000000 pyDecision-2.9.7/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     1835 2023-07-14 22:26:21.000000 pyDecision-2.9.7/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-2.9.7/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-2.9.7/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-2.9.7/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-2.9.7/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-2.9.7/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-2.9.7/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-2.9.7/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-2.9.7/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-2.9.7/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-2.9.7/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-2.9.7/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-2.9.7/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-2.9.7/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-2.9.7/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-2.9.7/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-2.9.7/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-2.9.7/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-2.9.7/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-2.9.7/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-2.9.7/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-2.9.7/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-2.9.7/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-2.9.7/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-2.9.7/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-2.9.7/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2998 2023-07-15 00:34:12.000000 pyDecision-2.9.7/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-2.9.7/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-2.9.7/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-2.9.7/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-2.9.7/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-2.9.7/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-2.9.7/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-2.9.7/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-2.9.7/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-2.9.7/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-2.9.7/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-2.9.7/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-2.9.7/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-2.9.7/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-2.9.7/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-2.9.7/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-2.9.7/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-2.9.7/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-2.9.7/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-2.9.7/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:39:29.000000 pyDecision-2.9.7/pyDecision/util/
--rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-2.9.7/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-2.9.7/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-2.9.7/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    12492 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 00:39:28.000000 pyDecision-2.9.7/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 00:39:29.000000 pyDecision-2.9.7/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-15 00:39:00.000000 pyDecision-2.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-2.9.8/LICENSE
+-rw-rw-rw-   0        0        0    12577 2023-07-15 01:33:29.000000 pyDecision-2.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0    12184 2023-07-15 01:32:45.000000 pyDecision-2.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-2.9.8/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     1835 2023-07-14 22:26:21.000000 pyDecision-2.9.8/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-2.9.8/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-2.9.8/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-2.9.8/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-2.9.8/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-2.9.8/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-2.9.8/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-2.9.8/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-2.9.8/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-2.9.8/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-2.9.8/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-2.9.8/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-2.9.8/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-2.9.8/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-2.9.8/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-2.9.8/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-2.9.8/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-2.9.8/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-2.9.8/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-2.9.8/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-2.9.8/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-2.9.8/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-2.9.8/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-2.9.8/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-2.9.8/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-2.9.8/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-2.9.8/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-2.9.8/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-2.9.8/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-2.9.8/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-2.9.8/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-2.9.8/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-2.9.8/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-2.9.8/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-2.9.8/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-2.9.8/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-2.9.8/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-2.9.8/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/util/
+-rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-2.9.8/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-2.9.8/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-2.9.8/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    12577 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1701 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 01:33:29.000000 pyDecision-2.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-07-15 01:32:55.000000 pyDecision-2.9.8/setup.py
```

### Comparing `pyDecision-2.9.7/LICENSE` & `pyDecision-2.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/PKG-INFO` & `pyDecision-2.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.7
+Version: 2.9.8
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -97,15 +97,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
-- TODIM ([ Colab Demo ]()) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
+- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-2.9.7/README.md` & `pyDecision-2.9.8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
-- TODIM ([ Colab Demo ]()) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
+- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/__init__.py` & `pyDecision-2.9.8/pyDecision/algorithm/__init__.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/ahp.py` & `pyDecision-2.9.8/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/aras.py` & `pyDecision-2.9.8/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/borda.py` & `pyDecision-2.9.8/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/bwm.py` & `pyDecision-2.9.8/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/cocoso.py` & `pyDecision-2.9.8/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/codas.py` & `pyDecision-2.9.8/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/copras.py` & `pyDecision-2.9.8/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/critic.py` & `pyDecision-2.9.8/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/dematel.py` & `pyDecision-2.9.8/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_i.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_i_s.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_i_v.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_ii.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_iii.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_iv.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/e_tri_b.py` & `pyDecision-2.9.8/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/edas.py` & `pyDecision-2.9.8/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/gra.py` & `pyDecision-2.9.8/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/idocriw.py` & `pyDecision-2.9.8/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/mabac.py` & `pyDecision-2.9.8/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/marcos.py` & `pyDecision-2.9.8/pyDecision/algorithm/marcos.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
             best[i]  = np.max(X[:, i])
             worst[i] = np.min(X[:, i])
         else:
             best[i]  = np.min(X[:, i])
             worst[i] = np.max(X[:, i])   
     for j in range(0, X.shape[1]):
         if (criterion_type[j] == 'max'):
-            X[:,j]   =  X[:,j]  / best[j]
+            X[:,j]   = X[:,j]   / best[j]
             worst[j] = worst[j] / best[j]
             best[j]  = best[j]  / best[j]
         else:
-            X[:,j]   =  best[j] / X[:,j]
+            X[:,j]   = best[j]  / X[:,j]
             worst[j] = best[j]  / worst[j]
             best[j]  = best[j]  / best[j]
     best  = np.array(best)
     worst = np.array(worst)
     for i in range(0, X.shape[1]):
         best[i]  = best[i]  * weights[i]
         worst[i] = worst[i] * weights[i]
```

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/maut.py` & `pyDecision-2.9.8/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/moora.py` & `pyDecision-2.9.8/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/moosra.py` & `pyDecision-2.9.8/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/multimoora.py` & `pyDecision-2.9.8/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/ocra.py` & `pyDecision-2.9.8/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_i.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_ii.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_iii.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_iv.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_v.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_vi.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/p_xgaia.py` & `pyDecision-2.9.8/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/saw.py` & `pyDecision-2.9.8/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/smart.py` & `pyDecision-2.9.8/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/todim.py` & `pyDecision-2.9.8/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/topsis.py` & `pyDecision-2.9.8/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/vikor.py` & `pyDecision-2.9.8/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/waspas.py` & `pyDecision-2.9.8/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/algorithm/wings.py` & `pyDecision-2.9.8/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/util/ga.py` & `pyDecision-2.9.8/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision/util/gwo.py` & `pyDecision-2.9.8/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/pyDecision.egg-info/PKG-INFO` & `pyDecision-2.9.8/pyDecision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.7
+Version: 2.9.8
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -97,15 +97,15 @@
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
-- TODIM ([ Colab Demo ]()) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
+- TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
 - WINGS ([ Colab Demo ](https://colab.research.google.com/drive/1li1_cPxwEM3NOZ4hbI8RROXyOmXeoWew?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.ejor.2013.02.007))
 - WSM, WPM, WASPAS ([ Colab Demo ](https://colab.research.google.com/drive/1HbLwXI4HkrmI-lsNzDtBOlCiwxfJltHi?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_15))
```

### Comparing `pyDecision-2.9.7/pyDecision.egg-info/SOURCES.txt` & `pyDecision-2.9.8/pyDecision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.7/setup.py` & `pyDecision-2.9.8/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='2.9.7',
+    version='2.9.8',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

