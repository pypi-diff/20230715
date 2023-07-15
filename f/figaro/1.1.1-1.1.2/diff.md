# Comparing `tmp/figaro-1.1.1.tar.gz` & `tmp/figaro-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.1.1.tar", last modified: Fri Jul 14 18:59:55 2023, max compression
+gzip compressed data, was "figaro-1.1.2.tar", last modified: Sat Jul 15 13:49:39 2023, max compression
```

## Comparing `figaro-1.1.1.tar` & `figaro-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,77 @@
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.692126 figaro-1.1.1/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.1/LICENSE
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      205 2023-07-14 18:25:52.000000 figaro-1.1.1/MANIFEST.in
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:59:55.691622 figaro-1.1.1/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.1/README.md
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.682100 figaro-1.1.1/figaro/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.1/figaro/__init__.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2475 2022-05-01 13:54:12.000000 figaro-1.1.1/figaro/coordinates.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000222 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro/cosmology.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-14 18:58:34.000000 figaro-1.1.1/figaro/cosmology.pxd
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.1.1/figaro/cosmology.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7637 2022-05-15 14:27:47.000000 figaro-1.1.1/figaro/credible_regions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.1/figaro/cumulative.c
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.1/figaro/cumulative.pyx
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.1/figaro/decorators.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8535 2023-07-07 12:21:05.000000 figaro-1.1.1/figaro/diagnostic.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.1/figaro/exceptions.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5301 2023-07-07 12:27:53.000000 figaro-1.1.1/figaro/likelihood.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26785 2023-07-14 18:57:48.000000 figaro-1.1.1/figaro/load.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5981 2023-07-12 07:21:45.000000 figaro-1.1.1/figaro/marginal.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41110 2023-07-14 08:28:34.000000 figaro-1.1.1/figaro/mixture.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2610 2023-01-31 15:40:41.000000 figaro-1.1.1/figaro/montecarlo.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.690972 figaro-1.1.1/figaro/pipelines/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.1/figaro/pipelines/create_glade.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/pipelines/entropy.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.1/figaro/pipelines/gen_mock_data.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.1/figaro/pipelines/hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.1/figaro/pipelines/par_hierarchical_inference.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/pipelines/par_probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.1/figaro/pipelines/ppplot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.1/figaro/pipelines/probability_density.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31946 2023-07-07 12:44:53.000000 figaro-1.1.1/figaro/plot.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.1/figaro/plot_settings.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39776 2023-07-07 12:44:53.000000 figaro-1.1.1/figaro/threeDvolume.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2236 2023-06-25 09:51:30.000000 figaro-1.1.1/figaro/transform.py
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15184 2023-07-14 08:00:31.000000 figaro-1.1.1/figaro/utils.py
-drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-14 18:59:55.685924 figaro-1.1.1/figaro.egg-info/
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/PKG-INFO
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      974 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/entry_points.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       94 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/requires.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-14 18:59:55.000000 figaro-1.1.1/figaro.egg-info/top_level.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)      110 2023-07-14 18:33:57.000000 figaro-1.1.1/pyproject.toml
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       93 2023-03-13 15:25:38.000000 figaro-1.1.1/requirements.txt
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-14 18:59:55.692290 figaro-1.1.1/setup.cfg
--rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4460 2023-07-14 18:56:51.000000 figaro-1.1.1/setup.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.822779 figaro-1.1.2/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1072 2022-02-08 13:50:37.000000 figaro-1.1.2/LICENSE
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 09:07:00.000000 figaro-1.1.2/MANIFEST.in
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-15 13:49:39.822307 figaro-1.1.2/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4255 2023-02-20 15:52:20.000000 figaro-1.1.2/README.md
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.782888 figaro-1.1.2/docs/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      142 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.coordinates.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.cosmology.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      159 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.credible_regions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.cumulative.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.decorators.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.diagnostic.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.exceptions.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.likelihood.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.load.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      133 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.marginal.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      130 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.mixture.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      139 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.montecarlo.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      177 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.create_glade.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      160 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.entropy.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      182 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.gen_mock_data.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      207 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.hierarchical_inference.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      221 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.par_hierarchical_inference.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      212 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.par_probability_density.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      157 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.ppplot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      198 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.probability_density.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      521 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.pipelines.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      121 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.plot.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      150 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.plot_settings.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      545 2023-07-14 21:26:56.000000 figaro-1.1.2/docs/figaro.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.threeDvolume.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      136 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.transform.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      124 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/figaro.utils.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      443 2023-07-15 08:11:09.000000 figaro-1.1.2/docs/index.rst
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       55 2023-07-15 08:03:40.000000 figaro-1.1.2/docs/modules.rst
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.809949 figaro-1.1.2/figaro/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        0 2022-05-05 11:31:57.000000 figaro-1.1.2/figaro/__init__.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2465 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/coordinates.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)  1000320 2023-07-15 09:07:35.000000 figaro-1.1.2/figaro/cosmology.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     3649 2023-07-15 09:06:46.000000 figaro-1.1.2/figaro/cosmology.pxd
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5030 2023-07-14 18:58:50.000000 figaro-1.1.2/figaro/cosmology.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     7604 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/credible_regions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)   297682 2023-03-13 16:06:47.000000 figaro-1.1.2/figaro/cumulative.c
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1911 2022-05-18 11:00:07.000000 figaro-1.1.2/figaro/cumulative.pyx
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1996 2023-03-08 12:59:32.000000 figaro-1.1.2/figaro/decorators.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     8492 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/diagnostic.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     1249 2023-07-07 12:34:31.000000 figaro-1.1.2/figaro/exceptions.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5262 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/likelihood.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    26737 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/load.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     5953 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/marginal.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    41154 2023-07-15 08:11:25.000000 figaro-1.1.2/figaro/mixture.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2604 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/montecarlo.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.821567 figaro-1.1.2/figaro/pipelines/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     6409 2022-05-15 14:27:47.000000 figaro-1.1.2/figaro/pipelines/create_glade.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    16259 2023-06-25 09:51:30.000000 figaro-1.1.2/figaro/pipelines/entropy.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4583 2022-11-17 16:07:28.000000 figaro-1.1.2/figaro/pipelines/gen_mock_data.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    12961 2023-06-30 08:48:22.000000 figaro-1.1.2/figaro/pipelines/hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    17678 2023-06-30 08:48:22.000000 figaro-1.1.2/figaro/pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    10389 2023-06-25 09:51:30.000000 figaro-1.1.2/figaro/pipelines/par_probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    11156 2023-03-29 08:52:28.000000 figaro-1.1.2/figaro/pipelines/ppplot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     9184 2023-07-13 15:25:45.000000 figaro-1.1.2/figaro/pipelines/probability_density.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    31875 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/plot.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      933 2023-06-27 13:05:57.000000 figaro-1.1.2/figaro/plot_settings.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    39731 2023-07-15 08:17:11.000000 figaro-1.1.2/figaro/threeDvolume.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     2230 2023-07-14 19:38:56.000000 figaro-1.1.2/figaro/transform.py
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    15174 2023-07-14 20:20:08.000000 figaro-1.1.2/figaro/utils.py
+drwxr-xr-x   0 stefanorinaldi   (501) staff       (20)        0 2023-07-15 13:49:39.815727 figaro-1.1.2/figaro.egg-info/
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4678 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)    24290 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)        1 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      483 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      103 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/requires.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      279 2023-07-15 13:49:39.000000 figaro-1.1.2/figaro.egg-info/top_level.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      145 2023-07-15 13:47:26.000000 figaro-1.1.2/pyproject.toml
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)      102 2023-07-15 13:48:02.000000 figaro-1.1.2/requirements.txt
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)       38 2023-07-15 13:49:39.822953 figaro-1.1.2/setup.cfg
+-rw-r--r--   0 stefanorinaldi   (501) staff       (20)     4092 2023-07-15 13:48:51.000000 figaro-1.1.2/setup.py
```

### Comparing `figaro-1.1.1/LICENSE` & `figaro-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/PKG-INFO` & `figaro-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.1
+Version: 1.1.2
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `figaro-1.1.1/README.md` & `figaro-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/coordinates.py` & `figaro-1.1.2/figaro/coordinates.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 def cartesian_to_celestial(vector):
     """
     Convert the Cartesian vector [x, y, z] to spherical coordinates [r, theta, phi].
     The parameter r is the radial distance, theta is the polar angle, and phi is the azimuth.
     
     Arguments:
-        :np.ndarray: cartesian vector [x, y, z]
+        np.ndarray: cartesian vector [x, y, z]
         
     Returns:
-        :np.ndarray: spherical coordinate vector [phi, theta, r]
+        np.ndarray: spherical coordinate vector [phi, theta, r]
     """
     vector = np.atleast_2d(vector)
     D = np.linalg.norm(vector, axis = -1)
     unit = np.array([v/np.linalg.norm(v) for v in vector])
     dec = np.arcsin(unit[:,2])
     ra = np.arctan2(unit[:,0], unit[:,1])
     ra[ra<0] += 2*np.pi
@@ -22,18 +22,18 @@
 
 def celestial_to_cartesian(vector):
     """
     Convert the celestial coordinate vector [phi, theta, r] to the Cartesian vector [x, y, z].
     The parameter r is the radial distance, theta is the polar angle, and phi is the azimuth
     
     Arguments:
-        :np.ndarray vector: celestial coordinate vector [ra, dec, dist]
+        np.ndarray vector: celestial coordinate vector [ra, dec, dist]
         
     Returns:
-        :np.ndarray: cartesian vector [x, y, z]
+        np.ndarray: cartesian vector [x, y, z]
     """
     vector = np.atleast_2d(vector)
     # Trig alias.
     cos_theta = np.cos(vector[:,1])
     # The vector.
     x = vector[:,2] * np.sin(vector[:,0]) * cos_theta
     y = vector[:,2] * np.cos(vector[:,0]) * cos_theta
@@ -41,40 +41,40 @@
     return np.array([x,y,z]).T
 
 def Jacobian(cartesian_vect):
     """
     Computes the jacobian of celestial transformation for a cartesian vector
     
     Arguments:
-        :np.ndarray cartesian_vect: cartesian vector [x, y, z]
+        np.ndarray cartesian_vect: cartesian vector [x, y, z]
     
     Returns:
-        :np.ndarray: Jacobian of the transformation
+        np.ndarray: Jacobian of the transformation
     """
     return Jacobian_in_celestial(cartesian_to_celestial(np.atleast_2d(cartesian_vect)))
 
 def inv_Jacobian(celestial_vect):
     """
     Computes the inverse jacobian of celestial transformation for a celestial vector
     
     Arguments:
-        :np.ndarray cartesian_vect: cartesian vector [ra, dec, D]
+        np.ndarray cartesian_vect: cartesian vector [ra, dec, D]
     
     Returns:
-        :np.ndarray: inverse Jacobian of the transformation
+        np.ndarray: inverse Jacobian of the transformation
     """
     detJ = Jacobian_in_celestial(np.atleast_2d(celestial_vect))
     return 1/detJ
     
 def Jacobian_in_celestial(celestial_vect):
     """
     Computes the jacobian of celestial transformation
     
     Arguments:
-        :np.ndarray cartesian_vect: cartesian vector [ra, dec, D]
+        np.ndarray cartesian_vect: cartesian vector [ra, dec, D]
     
     Returns:
-        :np.ndarray: Jacobian of the transformation
+        np.ndarray: Jacobian of the transformation
     """
     d = celestial_vect[:,2]
     theta = celestial_vect[:,1]
     return d*d*np.cos(theta)
```

### Comparing `figaro-1.1.1/figaro/cosmology.c` & `figaro-1.1.2/figaro/cosmology.c`

 * *Files 0% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 {
     "distutils": {
         "depends": [
             "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
             "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
             "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
             "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/opt/local/include/lal/LALCosmologyCalculator.h"
         ],
         "extra_compile_args": [
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             "figaro",
             "/opt/local/etc//include",
+            "/opt/local/include/",
             "/opt/anaconda3/lib/python3.9/site-packages/numpy/core/include"
         ],
         "libraries": [
             "m",
             "lal"
         ],
         "library_dirs": [
```

### Comparing `figaro-1.1.1/figaro/cosmology.pxd` & `figaro-1.1.2/figaro/cosmology.pxd`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/cosmology.pyx` & `figaro-1.1.2/figaro/cosmology.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/credible_regions.py` & `figaro-1.1.2/figaro/credible_regions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,64 +6,64 @@
 # confidence calculations
 # -----------------------
 def FindNearest_Volume(ra, dec, dist, value):
     """
     Find the pixel that contains the triplet (ra', dec', D') stored in value.
     
     Arguments:
-        :np.ndarray ra:   right ascension values used to build the grid
-        :np.ndarray dec:  declination values used to build the grid
-        :np.ndarray dist: luminosity distance values used to build the grid
-        :iterable value:  triplet to locate (ra', dec', D')
+        np.ndarray ra:   right ascension values used to build the grid
+        np.ndarray dec:  declination values used to build the grid
+        np.ndarray dist: luminosity distance values used to build the grid
+        iterable value:  triplet to locate (ra', dec', D')
     
     Returns:
-        :np.ndarray: grid indices of pixel
+        np.ndarray: grid indices of pixel
     """
     idx = np.zeros(3, dtype = int)
     for i, (d, v) in enumerate(zip([ra, dec, dist], value)):
         idx[i] = int(np.abs(d-v).argmin())
     return idx
 
 def FindNearest_Grid(grid, value):
     """
     Find the closest grid point to value.
     
     Arguments:
-        :np.ndarray grid: grid points (N_pts, N_dim), as with figaro.utils.recursive_grid
-        :iterable value:  value to locate
+        np.ndarray grid: grid points (N_pts, N_dim), as with figaro.utils.recursive_grid
+        iterable value:  value to locate
     
     Returns:
-        :np.ndarray: grid index
+        np.ndarray: grid index
     """
     return abs(np.sum((grid - value)**2, axis = -1)).argmin()
 
 def FindHeights(args):
     """
     Find height correspinding to a certain credible level given a sorted array of probabilities and the corresponding cumulative
     
     Arguments:
-        :tuple args: tuple containing the sorted array, the cumulative array and a double corresponding to the credible level
+        tuple args: tuple containing the sorted array, the cumulative array and a double corresponding to the credible level
     
     Returns:
-        :double: height corresponding to the credible level
+        double: height corresponding to the credible level
     """
     (sortarr,cumarr,level) = args
     return sortarr[np.abs(cumarr-np.log(level)).argmin()]
 
 def FindHeightForLevel(inLogArr, adLevels, logdd):
     """
     Given a probability array, computes the heights corresponding to some given credible levels.
     
     Arguments:
-        :np.ndarray inLogArr: probability array
-        :iterable adLevels:   credible levels
-        :double logdd:        variables log differential (∑ log(dx_i))
+        np.ndarray inLogArr: probability array
+        iterable adLevels:   credible levels
+        double logdd:        variables log differential (∑ log(dx_i))
         
     Returns:
-        :np.ndarray: heights corresponding to adLevels
+        np.ndarray: heights corresponding to adLevels
     """
     # flatten and create reversed sorted list
     adSorted = np.ascontiguousarray(np.sort(inLogArr.flatten())[::-1])
     # create a normalized cumulative distribution
     adCum = fast_log_cumulative(adSorted + logdd)
     # find values closest to levels
     adHeights = []
@@ -75,44 +75,44 @@
     return adHeights
 
 def FindLevelForHeight(inLogArr, logvalue, logdd):
     """
     Given a probability array, computes the credible levels corresponding to a given height.
     
     Arguments:
-        :np.ndarray inLogArr: log probability array
-        :double logvalue:     height
-        :double logdd:        variables log differential (∑ log(dx_i))
+        np.ndarray inLogArr: log probability array
+        double logvalue:     height
+        double logdd:        variables log differential (∑ log(dx_i))
     
     Returns:
-        :np.ndarray: credible level corresponding to logvalue
+        np.ndarray: credible level corresponding to logvalue
     """
     # flatten and create reversed sorted list
     adSorted = np.ascontiguousarray(np.sort(inLogArr.flatten())[::-1])
     # create a normalized cumulative distribution
     adCum = fast_log_cumulative(adSorted + logdd)
     # find index closest to value
     idx = (np.abs(adSorted-logvalue)).argmin()
     return np.exp(adCum[idx])
 
 def ConfidenceVolume(log_volume_map, ra_grid, dec_grid, distance_grid, log_measure = None, adLevels = [0.50, 0.90]):
     """
     Compute the credible volume(s) for a 3D probability distribution
     
     Arguments:
-        :np.ndarray log_volume_map: probability density for each pixel
-        :np.ndarray ra_grid:        right ascension values used to build the grid
-        :np.ndarray dec_grid:       declination values used to build the grid
-        :np.ndarray distance_grid:  luminosity distance values used to build the grid
-        :iterable adLevels:         credible level(s)
+        np.ndarray log_volume_map: probability density for each pixel
+        np.ndarray ra_grid:        right ascension values used to build the grid
+        np.ndarray dec_grid:       declination values used to build the grid
+        np.ndarray distance_grid:  luminosity distance values used to build the grid
+        iterable adLevels:         credible level(s)
     
     Returns:
-        :np.ndarray: credible volume(s)
-        :iterable:   indices of pixels within credible volume(s)
-        :np.ndarray: height(s) corresponding to credible volume(s)
+        np.ndarray: credible volume(s)
+        iterable:   indices of pixels within credible volume(s)
+        np.ndarray: height(s) corresponding to credible volume(s)
     """
     dd  = np.diff(distance_grid)[0]
     ddec = np.diff(dec_grid)[0]
     dra = np.diff(ra_grid)[0]
     # create a normalized cumulative distribution
     log_volume_map_sorted = np.ascontiguousarray(np.sort(log_volume_map.flatten())[::-1])
     if log_measure is not None:
@@ -138,23 +138,23 @@
     return volume_confidence, index, np.array(adHeights)
 
 def ConfidenceArea(log_skymap, ra_grid, dec_grid, log_measure = None, adLevels = [0.50, 0.90]):
     """
     Compute the credible area(s) for a 2D probability distribution
     
     Arguments:
-        :np.ndarray log_skymap: probability density for each pixel
-        :np.ndarray ra_grid:    right ascension values used to build the grid
-        :np.ndarray dec_grid:   declination values used to build the grid
-        :iterable adLevels:     credible level(s)
+        np.ndarray log_skymap: probability density for each pixel
+        np.ndarray ra_grid:    right ascension values used to build the grid
+        np.ndarray dec_grid:   declination values used to build the grid
+        iterable adLevels:     credible level(s)
     
     Returns:
-        :np.ndarray: credible area(s)
-        :iterable:   indices of pixels within credible area(s)
-        :np.ndarray: height(s) corresponding to credible area(s)
+        np.ndarray: credible area(s)
+        iterable:   indices of pixels within credible area(s)
+        np.ndarray: height(s) corresponding to credible area(s)
     """
     # create a normalized cumulative distribution
     ddec = np.diff(dec_grid)[0]
     dra = np.diff(ra_grid)[0]
     log_skymap_sorted  = np.ascontiguousarray(np.sort(log_skymap.flatten())[::-1])
     if log_measure is not None:
         log_measure_sorted = np.ascontiguousarray(log_measure.flatten()[np.argsort(log_skymap.flatten())][::-1])
```

### Comparing `figaro-1.1.1/figaro/cumulative.c` & `figaro-1.1.2/figaro/cumulative.c`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/cumulative.pyx` & `figaro-1.1.2/figaro/cumulative.pyx`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/decorators.py` & `figaro-1.1.2/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/diagnostic.py` & `figaro-1.1.2/figaro/diagnostic.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 
 @njit
 def angular_coefficient(x, y):
     """
     Angular coefficient obtained from linear regression.
     
     Arguments:
-        :np.ndarray x: independent variables
-        :np.ndarray y: dependent variables
+        np.ndarray x: independent variables
+        np.ndarray y: dependent variables
     
     Returns:
-        :double: angular coefficient
+        double: angular coefficient
     """
     return np.sum((x - np.mean(x))*(y - np.mean(y)))/np.sum((x - np.mean(x))**2)
     
 def compute_angular_coefficients(x, L = None):
     """
     Given an array of points x, computes the angular coefficient for each adjacent chunk of length L.
     
     Arguments:
-        :np.ndarray x: array of points
-        :int L:        window length
+        np.ndarray x: array of points
+        int L:        window length
     
     Returns:
-        :np.ndarray: array of angular coefficients
+        np.ndarray: array of angular coefficients
     """
     if L is None:
        L = len(x)//10
     
     if L > len(x):
         raise FIGAROException("L must be smaller than the number of points you have")
         
@@ -52,25 +52,25 @@
     return a
 
 def plot_angular_coefficient(entropy, L = 500, ac_expected = None, out_folder = '.', name = 'event', step = 1, show = False, save = True):
     """
     Compute entropy angular coefficient and produce the relevant plot
     
     Arguments:
-        :iterable entropy:       container of mixture instances
-        :int L:                  window lenght
-        :double ac_expected:     expected angular coefficient
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :int step:               number of draws between entropy samples (if downsampled by some other method, for plotting purposes only)
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        iterable entropy:       container of mixture instances
+        int L:                  window lenght
+        double ac_expected:     expected angular coefficient
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        int step:               number of draws between entropy samples (if downsampled by some other method, for plotting purposes only)
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     
     Returns:
-        :np.ndarray: angular coefficients
+        np.ndarray: angular coefficients
     """
     S = compute_angular_coefficients(entropy, L = L)
     fig, ax = plt.subplots()
     if ac_expected is not None:
         ax.axhline(ac_expected, lw = 0.5, ls = '--', c = 'r')
     ax.plot(np.arange(len(S))*step+L, S, ls = '--', marker = '', color = 'steelblue', lw = 0.7)
     ax.set_ylabel('$\\frac{dS(N)}{dN}$')
@@ -84,21 +84,21 @@
 
 @njit
 def compute_autocorrelation(draws, mean, dx):
     """
     Computes autocorrelation of subsequent draws as <∫(draw[i]-mean)*(draw[i+t]-mean)*dx/∫(draw[i]-mean)**2*dx>
     
     Arguments:
-        :np.ndarray draws: evaluated mixtures (2d array)
-        :np.ndarray mean:  bin-wise mean of evaluated mixtures (1d array)
-        :double dx:        integration measure
+        np.ndarray draws: evaluated mixtures (2d array)
+        np.ndarray mean:  bin-wise mean of evaluated mixtures (1d array)
+        double dx:        integration measure
     
     Returns:
-        :int: upper bound of autocorrelation length
-        :np.ndarray: autocorrelation function
+        int: upper bound of autocorrelation length
+        np.ndarray: autocorrelation function
     """
     taumax          = draws.shape[0]//2
     n_draws         = draws.shape[0]
     autocorrelation = np.zeros(taumax, dtype = np.float64)
     N = 0.
     for i in prange(n_draws):
         N += np.sum((draws[i] - mean)*(draws[i] - mean))*dx/n_draws
@@ -111,24 +111,24 @@
     return taumax, autocorrelation
 
 def autocorrelation(draws, bounds = None, out_folder = '.', name = 'event', n_points = 1000, save = True, show = False):
     """
     Compute autocorrelation of a set of draws and produce the relevant plot
     
     Arguments:
-        :iterable draws:         container of mixture instances
-        :iterable bounds:        bounds of the interval over which the distributions are evaluated. It has to be passed as [[xmin,xmax]]. If None, draws bounds are used.
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :int n_points:           number of points for linspace
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        iterable draws:         container of mixture instances
+        iterable bounds:        bounds of the interval over which the distributions are evaluated. It has to be passed as [[xmin,xmax]]. If None, draws bounds are used.
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        int n_points:           number of points for linspace
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     
     Returns:
-        :np.ndarray: autocorrelation
+        np.ndarray: autocorrelation
     """
     all_bounds = np.atleast_2d([d.bounds[0] for d in draws])
     x_min = np.max(all_bounds[:,0])
     x_max = np.min(all_bounds[:,1])
 
     if bounds is not None:
         if not bounds[0] >= x_min:
@@ -160,19 +160,19 @@
     return ac
     
 def compute_entropy_single_draw(mixture, n_draws = 1e3, return_error = False):
     """
     Compute entropy for a single realisation of the DPGMM using Monte Carlo integration
     
     Arguments:
-        :mixture mixture: instance of mixture class (see mixture.py for definition)
-        :double n_draws:  number of MC draws
+        mixture mixture: instance of mixture class (see mixture.py for definition)
+        double n_draws:  number of MC draws
     
     Returns:
-        :double: entropy value
+        double: entropy value
     """
     samples = mixture.rvs(int(n_draws))
     logP    = mixture.logpdf(samples)
     entropy = np.mean(-logP)/log2e
     if not return_error:
         return entropy
     else:
@@ -180,19 +180,19 @@
         return entropy, dentropy
 
 def compute_entropy(draws, n_draws = 1e3, return_error = False):
     """
     Compute entropy for a list of realisations of the DPGMM using Monte Carlo integration
     
     Arguments:
-        :iterable draws: container of mixture class instaces (see mixture.py for definition)
-        :double n_draws: number of MC draws
+        iterable draws: container of mixture class instaces (see mixture.py for definition)
+        double n_draws: number of MC draws
     
     Returns:
-        :np.ndarray: entropy values
+        np.ndarray: entropy values
     """
     S = np.zeros(len(draws))
     if not return_error:
         for i, d in enumerate(draws):
             S[i] = compute_entropy_single_draw(d, n_draws)
         return S
     else:
@@ -202,25 +202,25 @@
         return S, dS
 
 def entropy(draws, out_folder = '.', exp_entropy = None, name = 'event', n_draws = 1e4, step = 1, show = False, save = True):
     """
     Compute entropy of a set of draws and produce the relevant plot
     
     Arguments:
-        :iterable draws:         container of mixture instances
-        :str or Path out_folder: output folder
-        :double exp_entropy:     expected value for entropy, expressed in bits
-        :str name:               name to be given to outputs
-        :int n_draws:            number of MC draws
-        :int step:               number of draws between entropy samples (if downsampled by some other method, for plotting purposes only)
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        iterable draws:         container of mixture instances
+        str or Path out_folder: output folder
+        double exp_entropy:     expected value for entropy, expressed in bits
+        str name:               name to be given to outputs
+        int n_draws:            number of MC draws
+        int step:               number of draws between entropy samples (if downsampled by some other method, for plotting purposes only)
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     
     Return:
-        :np.ndarray: entropy
+        np.ndarray: entropy
     """
     S = compute_entropy(draws, int(n_draws))
     fig, ax = plt.subplots()
     ax.plot(np.arange(1, len(draws)+1)*step, S, ls = '--', marker = '', lw = 0.7)
     if exp_entropy is not None:
         ax.axhline(exp_entropy, lw = 0.5, ls = '--', c = 'r')
     ax.set_xlabel('$N$')
```

### Comparing `figaro-1.1.1/figaro/exceptions.py` & `figaro-1.1.2/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/likelihood.py` & `figaro-1.1.2/figaro/likelihood.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,75 +23,75 @@
 
 @njit
 def scalar_product(v, M, n):
     """
     Scalar product: v*M*v^T
     
     Arguments:
-        :np.ndarray v: array
-        :np.ndarray M: matrix
-        :int n:        len(v)
+        np.ndarray v: array
+        np.ndarray M: matrix
+        int n:        len(v)
     
     Returns:
-        :double: v*M*v^T
+        double: v*M*v^T
     """
     res = 0.
     for i in prange(n):
         for j in prange(n):
             res = res + M[i,j]*v[i]*v[j]
     return res
 
 @njit
 def log_norm_1d(x, m, s):
     """
     1D Normal logpdf
     
     Arguments:
-        :double x: value
-        :double m: mean
-        :double s: var
+        double x: value
+        double m: mean
+        double s: var
     
     Returns:
         Normal(m,s).logpdf(x)
     """
     return -(x-m)**2/(2*s) - 0.5*np.log(2*np.pi*s)
 
 @njit
 def log_norm(x, mu, cov):
     """
     Multivariate Normal logpdf
     
     Arguments:
-        :np.ndarray x:   value
-        :np.ndarray mu:  mean vector
-        :np.ndarray cov: covariance matrix
+        np.ndarray x:   value
+        np.ndarray mu:  mean vector
+        np.ndarray cov: covariance matrix
     
     Returns:
-        :double: MultivariateNormal(m,s).logpdf(x)
+        double: MultivariateNormal(m,s).logpdf(x)
     """
     inv_cov  = inv_jit(cov)
     exponent = -0.5*scalar_product(x-mu, inv_cov, len(mu))
     lognorm  = 0.5*len(mu)*LOG2PI+0.5*logdet_jit(cov)
     return -lognorm+exponent
 
 @njit
 def log_norm_int(x, mu, cov_1, inv_cov_1, cov_2):
     """
     Multivariate Normal logpdf (tailored to this problem!)
     See https://arxiv.org/pdf/1811.04751v1.pdf
     
     Arguments:
-        :np.ndarray x:         value
-        :np.ndarray mu:        mean vector
-        :np.ndarray cov_1:     1st covariance matrix
-        :np.ndarray inv_cov_1: inverse of 1st covariance matrix
-        :np.ndarray cov_2:     2nd covariance matrix
+        np.ndarray x:         value
+        np.ndarray mu:        mean vector
+        np.ndarray cov_1:     1st covariance matrix
+        np.ndarray inv_cov_1: inverse of 1st covariance matrix
+        np.ndarray cov_2:     2nd covariance matrix
     
     Returns:
-        :double: MultivariateNormal(m,s).logpdf(x)
+        double: MultivariateNormal(m,s).logpdf(x)
     """
     inv_cov_2  = inv_jit(cov_2)
     inv_cov    = inv_cov_1@inv_jit(inv_cov_1+inv_cov_2)@inv_cov_2
     exponent   = -0.5*scalar_product(x-mu, inv_cov, len(mu))
     lognorm    = 0.5*len(mu)*LOG2PI+0.5*(logdet_jit(cov_1) + logdet_jit(cov_2) + logdet_jit(inv_cov_1+inv_cov_2))
     return -lognorm+exponent
 
@@ -101,38 +101,38 @@
 
 @njit
 def eval_mix_1d(mu, sigma, means, covs):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for all the components of a mixture (for predictive likelihood, 1D).
     
     Arguments:
-        :np.ndarray mu:    temptative mean of the parent mixture component
-        :np.ndarray sigma: temptative variance of the parent mixture component
-        :np.ndarray means: means of the event mixture components
-        :np.ndarray vars:  variances of the event mixture components
+        np.ndarray mu:    temptative mean of the parent mixture component
+        np.ndarray sigma: temptative variance of the parent mixture component
+        np.ndarray means: means of the event mixture components
+        np.ndarray vars:  variances of the event mixture components
     
     Returns:
-        :np.ndarray: probability for each event mixture components
+        np.ndarray: probability for each event mixture components
     """
     return np.array([log_norm_1d(means[i,0], mu, sigma+covs[i,0,0]) for i in prange(len(means))])
 
 @njit
 def evaluate_mixture_MC_draws_1d(mu, sigma, means, vars, w):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for a set of MC draws for mu and sigma.
     
     Arguments:
-        :np.ndarray mu:    MC draws for the mean of the parent mixture component
-        :np.ndarray sigma: MC draws for the variance of the parent mixture component
-        :np.ndarray means: means of the event mixture components
-        :np.ndarray vars:  variances of the event mixture components
-        :np.ndarray w:     component weights
+        np.ndarray mu:    MC draws for the mean of the parent mixture component
+        np.ndarray sigma: MC draws for the variance of the parent mixture component
+        np.ndarray means: means of the event mixture components
+        np.ndarray vars:  variances of the event mixture components
+        np.ndarray w:     component weights
     
     Returns:
-        :np.ndarray: probability for each MC draw
+        np.ndarray: probability for each MC draw
     """
     logP = np.zeros(len(mu), dtype = np.float64)
     for i in prange(len(mu)):
         logP[i] = logsumexp_jit(eval_mix_1d(mu[i], sigma[i], means, vars), b = w)
     return logP
 
 #------------#
@@ -141,37 +141,37 @@
 
 @njit
 def eval_mix(mu, sigma, means, covs):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for all the components of a mixture (for predictive likelihood, ND).
     
     Arguments:
-        :np.ndarray mu:    temptative mean of the parent mixture component
-        :np.ndarray sigma: temptative covariance matrix of the parent mixture component
-        :np.ndarray means: means of the event mixture components
-        :np.ndarray covs:  covariance matrices of the event mixture components
+        np.ndarray mu:    temptative mean of the parent mixture component
+        np.ndarray sigma: temptative covariance matrix of the parent mixture component
+        np.ndarray means: means of the event mixture components
+        np.ndarray covs:  covariance matrices of the event mixture components
     
     Returns:
-        :np.ndarray: probability for each event mixture components
+        np.ndarray: probability for each event mixture components
     """
     inv_sigma = inv_jit(sigma)
     return np.array([log_norm_int(means[i], mu, sigma, inv_sigma, covs[i]) for i in prange(len(means))])
 
 @njit
 def evaluate_mixture_MC_draws(mu, sigma, means, covs, w):
     """
     Computes N(mu_k| mu, (sigma_k^2+sigma^2) for a set of MC draws for mu and sigma.
     
     Arguments:
-        :np.ndarray mu:    MC draws for the mean vector of the parent mixture component
-        :np.ndarray sigma: MC draws for the covariance matrix of the parent mixture component
-        :np.ndarray means: means of the event mixture components
-        :np.ndarray covs:  covariance matrices of the event mixture components
-        :np.ndarray w:     component weights
+        np.ndarray mu:    MC draws for the mean vector of the parent mixture component
+        np.ndarray sigma: MC draws for the covariance matrix of the parent mixture component
+        np.ndarray means: means of the event mixture components
+        np.ndarray covs:  covariance matrices of the event mixture components
+        np.ndarray w:     component weights
     
     Returns:
-        :np.ndarray: probability for each MC draw
+        np.ndarray: probability for each MC draw
     """
     logP = np.zeros(len(mu), dtype = np.float64)
     for i in prange(len(mu)):
         logP[i] = logsumexp_jit(eval_mix(mu[i], sigma[i], means, covs), b = w)
     return logP
```

### Comparing `figaro-1.1.1/figaro/load.py` & `figaro-1.1.2/figaro/load.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,19 +49,19 @@
           }
 
 def _find_redshift(omega, dl):
     """
     Find redshift given a luminosity distance and a cosmology using Newton's method
     
     Arguments:
-        :CosmologicalParameters omega: cosmology (see cosmology.pyx for definition)
-        :double dl:                    luminosity distance
+        CosmologicalParameters omega: cosmology (see cosmology.pyx for definition)
+        double dl:                    luminosity distance
     
     Returns:
-        :double: redshift
+        double: redshift
     """
     def objective(z, omega, dl):
         return dl - omega.LuminosityDistance_double(z)
     return newton(objective,1.0,args=(omega,dl))
     
 def available_gw_pars():
     """
@@ -72,29 +72,29 @@
 def load_single_event(event, seed = False, par = None, n_samples = -1, h = 0.674, om = 0.315, ol = 0.685, volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None):
     '''
     Loads the data from .txt/.dat files (for simulations) or .h5/.hdf5 files (posteriors from GWTC) for a single event.
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of the available parameters.
     
     Arguments:
-        :str or Path file: file with samples
-        :bool seed:        fixes the seed to a default value (1) for reproducibility
-        :list-of-str par:  list with parameter(s) to extract from GW posteriors (m1, m2, mc, z, chi_effective)
-        :int n_samples:    number of samples for (random) downsampling. Default -1: all samples
-        :double h:         Hubble constant H0/100 [km/(s*Mpc)]
-        :double om:        matter density parameter
-        :double ol:        cosmological constant density parameter
-        :bool volume:      if True, loads RA, dec and Luminosity distance (for skymaps)
-        :str waveform:     waveform family to be used ('combined', 'seob', 'imr')
-        :double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
-        :double far_threshold: FAR threshold for event filtering. For injection analysis only.
+        str or Path file: file with samples
+        bool seed:        fixes the seed to a default value (1) for reproducibility
+        list-of-str par:  list with parameter(s) to extract from GW posteriors (m1, m2, mc, z, chi_effective)
+        int n_samples:    number of samples for (random) downsampling. Default -1: all samples
+        double h:         Hubble constant H0/100 [km/(s*Mpc)]
+        double om:        matter density parameter
+        double ol:        cosmological constant density parameter
+        bool volume:      if True, loads RA, dec and Luminosity distance (for skymaps)
+        str waveform:     waveform family to be used ('combined', 'seob', 'imr')
+        double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
+        double far_threshold: FAR threshold for event filtering. For injection analysis only.
         
     Returns:
-        :np.ndarray: samples
-        :np.ndarray: name
+        np.ndarray: samples
+        np.ndarray: name
     '''
     if seed:
         rdstate = np.random.RandomState(seed = 1)
     else:
         rdstate = np.random.RandomState()
     event = Path(event).resolve()
     name, ext = str(event).split('/')[-1].split('.')
@@ -136,28 +136,28 @@
 def load_data(path, seed = False, par = None, n_samples = -1, h = 0.674, om = 0.315, ol = 0.685, volume = False, waveform = 'combined', snr_threshold = None, far_threshold = None):
     '''
     Loads the data from .txt files (for simulations) or .h5/.hdf5/.dat files (posteriors from GWTC-x).
     Default cosmological parameters from Planck Collaboration (2021) in a flat Universe (https://www.aanda.org/articles/aa/pdf/2020/09/aa33910-18.pdf)
     Not all GW parameters are implemented: run figaro.load.available_gw_pars() for a list of available parameters.
     
     Arguments:
-        :str or Path path: folder with data files
-        :bool seed:        fixes the seed to a default value (1) for reproducibility
-        :list-of-str par:  list with parameter(s) to extract from GW posteriors
-        :int n_samples:    number of samples for (random) downsampling. Default -1: all samples
-        :double h:         Hubble constant H0/100 [km/(s*Mpc)]
-        :double om:        matter density parameter
-        :double ol:        cosmological constant density parameter
-        :str waveform:     waveform family to be used ('combined', 'seob', 'imr')
-        :double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
-        :double far_threshold: FAR threshold for event filtering. For injection analysis only.
+        str or Path path: folder with data files
+        bool seed:        fixes the seed to a default value (1) for reproducibility
+        list-of-str par:  list with parameter(s) to extract from GW posteriors
+        int n_samples:    number of samples for (random) downsampling. Default -1: all samples
+        double h:         Hubble constant H0/100 [km/(s*Mpc)]
+        double om:        matter density parameter
+        double ol:        cosmological constant density parameter
+        str waveform:     waveform family to be used ('combined', 'seob', 'imr')
+        double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
+        double far_threshold: FAR threshold for event filtering. For injection analysis only.
 
     Returns:
-        :np.ndarray: samples
-        :np.ndarray: names
+        np.ndarray: samples
+        np.ndarray: names
     '''
     folder      = Path(path).resolve()
     event_files = [Path(folder,f) for f in folder.glob('[!.]*')] # Ignores hidden files
     events      = []
     names       = []
     n_events    = len(event_files)
     removed_snr = False
@@ -228,24 +228,24 @@
         * SEOBNRv4
     For IMR waveforms, in descending order:
         * IMRPhenomXPHM
         * IMRPhenomPv2
         * IMRPhenomPv3HM
     
     Arguments:
-        :str event:            file to read
-        :str par:              parameter to extract
-        :tuple cosmology:      cosmological parameters (h, om, ol)
-        :int n_samples:        number of samples for (random) downsampling. Default -1: all samples
-        :str waveform:         waveform family to be used ('combined', 'imr', 'seob')
-        :double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
-        :double far_threshold: FAR threshold for event filtering. For injection analysis only.
+        str event:            file to read
+        str par:              parameter to extract
+        tuple cosmology:      cosmological parameters (h, om, ol)
+        int n_samples:        number of samples for (random) downsampling. Default -1: all samples
+        str waveform:         waveform family to be used ('combined', 'imr', 'seob')
+        double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
+        double far_threshold: FAR threshold for event filtering. For injection analysis only.
     
     Returns:
-        :np.ndarray:    samples
+        np.ndarray:    samples
     '''
     h, om, ol = cosmology
     omega = CosmologicalParameters(h, om, ol, -1, 0)
     if not waveform in supported_waveforms:
         raise FIGAROException("Unknown waveform: please use 'combined' (default), 'imr' or 'seob'")
     
     if far_threshold is not None and snr_threshold is not None:
@@ -471,18 +471,18 @@
                 return samples
 
 def save_density(draws, folder = '.', name = 'density', ext = 'pkl'):
     """
     Exports a list of figaro.mixture instances to file
 
     Arguments:
-        :list draws:         list of mixtures to be saved
-        :str or Path folder: folder in which the output file will be saved
-        :str name:           name to be given to output file
-        :str ext:            file extension (pkl or json)
+        list draws:         list of mixtures to be saved
+        str or Path folder: folder in which the output file will be saved
+        str name:           name to be given to output file
+        str ext:            file extension (pkl or json)
     """
     if ext == 'pkl':
         with open(Path(folder, name+'.pkl'), 'wb') as f:
             dill.dump(draws, f)
     elif ext == 'json':
         if len(np.shape(draws)) == 1:
             draws = np.atleast_2d(draws)
@@ -504,35 +504,35 @@
 
 def load_density(path):
     """
     Loads a list of figaro.mixture instances from path.
     If the requested file extension (pkl or json) is not available, it tries loading the other.
 
     Arguments:
-        :str or Path path: path with draws (file or folder)
+        str or Path path: path with draws (file or folder)
 
     Returns
-        :list: figaro.mixture object instances
+        list: figaro.mixture object instances
     """
     path = Path(path)
     if path.is_file():
         return _load_density_file(path)
     else:
         return [_load_density_file(file) for file in path.glob('*.[jp][sk][ol]*') if not file.stem == 'posteriors_single_event']
 
 def _load_density_file(file):
     """
     Loads a list of figaro.mixture instances from file.
     If the requested file extension (pkl or json) is not available, it tries loading the other.
 
     Arguments:
-        :str or Path file: file with draws
+        str or Path file: file with draws
 
     Returns
-        :list: figaro.mixture object instances
+        list: figaro.mixture object instances
     """
     file = Path(file)
     ext  = file.suffix
     if ext == '.pkl':
         try:
             return _load_pkl(file)
         except FileNotFoundError:
@@ -552,32 +552,32 @@
         raise FIGAROException("Extension {0} is not supported. Please provide .pkl or .json file.".format(file.suffix))
 
 def _load_pkl(file):
     """
     Loads a list of figaro.mixture instances from pkl file
 
     Arguments:
-        :str or Path file: file with draws
+        str or Path file: file with draws
 
     Returns
-        :list: figaro.mixture object instances
+        list: figaro.mixture object instances
     """
     with open(file, 'rb') as f:
         draws = dill.load(f)
     return draws
 
 def _load_json(file):
     """
     Loads a list of figaro.mixture instances from json file
 
     Arguments:
-        :str or Path file: file with draws
+        str or Path file: file with draws
 
     Returns
-        :list: figaro.mixture object instances
+        list: figaro.mixture object instances
     """
     with open(Path(file), 'r') as fjson:
         dictjson = json.loads(json.load(fjson))
     ll = []
     for list_of_dict in dictjson:
         draws = []
         for dict_ in list_of_dict:
```

### Comparing `figaro-1.1.1/figaro/marginal.py` & `figaro-1.1.2/figaro/marginal.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,40 @@
 @njit
 def _cond_mean_cov(vals, mu1, mu2, s11, s22, s12):
     """
     Compute mean and covariance for conditional Normal distribution.
     See https://stats.stackexchange.com/questions/348941/general-conditional-distributions-for-multivariate-gaussian-mixtures
     
     Arguments:
-        :np.ndarray vals: values to condition on
-        :np.ndarray mu1:  mean subvector (NOT conditioned)
-        :np.ndarray mu2:  mean subvector (conditioned)
-        :np.ndarray s11:  covariance submatrix (NOT conditioned)
-        :np.ndarray s22:  covariance submatrix (conditioned)
-        :np.ndarray s12:  off-diagonal
+        np.ndarray vals: values to condition on
+        np.ndarray mu1:  mean subvector (NOT conditioned)
+        np.ndarray mu2:  mean subvector (conditioned)
+        np.ndarray s11:  covariance submatrix (NOT conditioned)
+        np.ndarray s22:  covariance submatrix (conditioned)
+        np.ndarray s12:  off-diagonal
     
     Returns:
-        :np.ndarray: mean
-        :np.ndarray: covariance
+        np.ndarray: mean
+        np.ndarray: covariance
     """
     s22_inv = inv_jit(s22)
     mean = mu1 + s12@(s22_inv@(vals - mu2))
     cov  = s11 - s12@(s22_inv@s12.T)
     return mean, cov
 
 def _marginalise(mix, axis = -1):
     """
     Marginalise out one or more dimensions from a FIGARO mixture.
     
     Arguments:
-        :figaro.mixture.mixture draws: mixture
-        :int or list of int axis:      axis to marginalise on
+        figaro.mixture.mixture draws: mixture
+        int or list of int axis:      axis to marginalise on
     
     Returns:
-        :figaro.mixture.mixture: the marginalised mixture
+        figaro.mixture.mixture: the marginalised mixture
     """
     # Circular import
     from figaro.mixture import mixture
     ax     = np.atleast_1d(axis)
     dim    = mix.dim - len(ax)
     if dim < 1:
         raise FIGAROException("Cannot marginalise out all dimensions")
@@ -52,19 +52,19 @@
     return mixture(means, covs, mix.w, bounds, dim, mix.n_cl, mix.n_pts, probit = mix.probit)
 
 def marginalise(draws, axis = -1):
     """
     Marginalise out one or more dimensions from a FIGARO draw.
     
     Arguments:
-        :figaro.mixture.mixture draws: mixture(s)
-        :int or list of int axis:      axis to marginalise on
+        figaro.mixture.mixture draws: mixture(s)
+        int or list of int axis:      axis to marginalise on
     
     Returns:
-        :figaro.mixture.mixture: the marginalised mixture(s)
+        figaro.mixture.mixture: the marginalised mixture(s)
     """
     if axis == []:
         return draws
     if np.iterable(draws):
         return np.array([_marginalise(d, axis) for d in draws])
     else:
         return _marginalise(draws, axis)
@@ -74,23 +74,23 @@
     """
     Probability density conditioned on specific values of a subset of parameters.
     See:
      * https://stats.stackexchange.com/questions/348941/general-conditional-distributions-for-multivariate-gaussian-mixtures
      * https://stats.stackexchange.com/questions/30588/deriving-the-conditional-distributions-of-a-multivariate-normal-distribution
     
     Arguments:
-        :figaro.mixture.mixture mix: mixture
-        :iterable vals:              value(s) to condition on
-        :int or list of int dims:    dimension(s) associated with given vals (starting from 0)
-        :bool norm:                  normalize the distribution
-        :bool filter:                  filter the components with weight < tol
-        :double tol:                   tolerance on the sum of the weights
+        figaro.mixture.mixture mix: mixture
+        iterable vals:              value(s) to condition on
+        int or list of int dims:    dimension(s) associated with given vals (starting from 0)
+        bool norm:                  normalize the distribution
+        bool filter:                  filter the components with weight < tol
+        double tol:                   tolerance on the sum of the weights
     
     Returns:
-        :figaro.mixture.mixture: the conditioned mixture(s)
+        figaro.mixture.mixture: the conditioned mixture(s)
     """
     # Circular import
     from figaro.mixture import mixture
     ax   = np.atleast_1d(dims)
     vals = vals[ax]
     dim  = mix.dim - len(ax)
     idx  = np.array([i in ax for i in range(mix.dim)])
@@ -127,23 +127,23 @@
     return mixture(means[idx_filt], covs[idx_filt], np.exp(log_weights[idx_filt]), bounds, dim, len(log_weights[idx_filt]), mix.n_pts, probit = mix.probit, log_w = log_weights[idx_filt])
 
 def condition(draws, vals, dims, norm = True, filter = True, tol = 1e-4):
     """
     Probability density conditioned on specific values of a subset of parameters.
     
     Arguments:
-        :figaro.mixture.mixture draws: mixture(s)
-        :iterable vals:                value(s) to condition on
-        :int or list of int dims:      dimension(s) associated with given vals (starting from 0)
-        :bool norm:                    normalize the distribution
-        :bool filter:                  filter the components with weight < tol
-        :double tol:                   tolerance on the sum of the weights
+        figaro.mixture.mixture draws: mixture(s)
+        iterable vals:                value(s) to condition on
+        int or list of int dims:      dimension(s) associated with given vals (starting from 0)
+        bool norm:                    normalize the distribution
+        bool filter:                  filter the components with weight < tol
+        double tol:                   tolerance on the sum of the weights
     
     Returns:
-        :figaro.mixture.mixture: the conditioned mixture(s)
+        figaro.mixture.mixture: the conditioned mixture(s)
     """
     if np.iterable(draws):
         v       = np.mean(draws[0].bounds, axis = -1)
         v[dims] = vals
         return np.array([_condition(d, v, dims, norm, filter, tol) for d in draws])
     else:
         v       = np.mean(draws.bounds, axis = -1)
```

### Comparing `figaro-1.1.1/figaro/mixture.py` & `figaro-1.1.2/figaro/mixture.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 @njit
 def _student_t(df, t, mu, sigma, dim):
     """
     Multivariate student-t pdf.
     As in http://gregorygundersen.com/blog/2020/01/20/multivariate-t/
     
     Arguments:
-        :float df:         degrees of freedom
-        :float t:          variable (2d array)
-        :np.ndarray mu:    mean (2d array)
-        :np.ndarray sigma: variance
-        :int dim:          number of dimensions
+        float df:         degrees of freedom
+        float t:          variable (2d array)
+        np.ndarray mu:    mean (2d array)
+        np.ndarray sigma: variance
+        int dim:          number of dimensions
         
     Returns:
-        :float: student_t(df).logpdf(t)
+        float: student_t(df).logpdf(t)
     """
     vals, vecs = np.linalg.eigh(sigma)
     logdet     = np.log(vals).sum()
     valsinv    = np.array([1./v for v in vals])
     U          = vecs * np.sqrt(valsinv)
     dev        = t - mu
     maha       = np.square(np.dot(dev, U)).sum(axis=-1)
@@ -76,177 +76,177 @@
     C = dim/2. * np.log(df * np.pi)
     D = 0.5 * logdet
     E = -x * np.log1p((1./df) * maha)
 
     return (A - B - C - D + E)[0]
 
 @njit
-def update_alpha(alpha, n, K, burnin = 1000):
+def _update_alpha(alpha, n, K, burnin = 1000):
     """
     Update concentration parameter using a Metropolis-Hastings sampling scheme.
     
     Arguments:
-        :double alpha: Initial value for concentration parameter
-        :int n:        Number of samples
-        :int K:        Number of active clusters
-        :int burnin:   MH burnin
+        double alpha: Initial value for concentration parameter
+        int n:        Number of samples
+        int K:        Number of active clusters
+        int burnin:   MH burnin
     
     Returns:
-        :double: new concentration parameter value
+        double: new concentration parameter value
     """
     a_old = alpha
     n_draws = burnin+np.random.randint(100)
     for i in prange(n_draws):
         a_new = a_old + (np.random.random() - 0.5)
         if a_new > 0.:
             logP_old = _numba_gammaln(a_old) - _numba_gammaln(a_old + n) + K * np.log(a_old) - 1./a_old
             logP_new = _numba_gammaln(a_new) - _numba_gammaln(a_new + n) + K * np.log(a_new) - 1./a_new
             if logP_new - logP_old > np.log(np.random.random()):
                 a_old = a_new
     return a_old
 
 @njit
-def compute_t_pars(k, mu, nu, L, mean, S, N, dim):
+def _compute_t_pars(k, mu, nu, L, mean, S, N, dim):
     """
     Compute parameters for student-t distribution.
     
     Arguments:
-        :double k:        Normal std parameter (for NIW)
-        :np.ndarray mu:   Normal mean parameter (for NIW)
-        :int nu:          Inverse-Wishart df parameter (for NIW)
-        :np.ndarray L:    Inverse-Wishart scale matrix (for NIW)
-        :np.ndarray mean: samples mean
-        :np.ndarray S:    samples covariance
-        :int N:           number of samples
-        :int dim:         number of dimensions
+        double k:        Normal std parameter (for NIW)
+        np.ndarray mu:   Normal mean parameter (for NIW)
+        int nu:          Inverse-Wishart df parameter (for NIW)
+        np.ndarray L:    Inverse-Wishart scale matrix (for NIW)
+        np.ndarray mean: samples mean
+        np.ndarray S:    samples covariance
+        int N:           number of samples
+        int dim:         number of dimensions
     
     Returns:
-        :int:        degrees of fredom for student-t
-        :np.ndarray: scale matrix for student-t
-        :np.ndarray: mean for student-t
+        int:        degrees of fredom for student-t
+        np.ndarray: scale matrix for student-t
+        np.ndarray: mean for student-t
     """
     # Update hyperparameters
-    k_n, mu_n, nu_n, L_n = compute_hyperpars(k, mu, nu, L, mean, S, N)
+    k_n, mu_n, nu_n, L_n = _compute_hyperpars(k, mu, nu, L, mean, S, N)
     # Update t-parameters
     t_df    = nu_n - dim + 1
     t_shape = L_n*(k_n+1)/(k_n*t_df)
     return t_df, t_shape, mu_n
 
 @njit
-def compute_hyperpars(k, mu, nu, L, mean, S, N):
+def _compute_hyperpars(k, mu, nu, L, mean, S, N):
     """
     Update hyperparameters for Normal Inverse Gamma/Wishart (NIG/NIW).
     See https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf
     
     Arguments:
-        :double k:        Normal std parameter (for NIG/NIW)
-        :np.ndarray mu:   Normal mean parameter (for NIG/NIW)
-        :int nu:          Gamma df parameter (for NIG/NIW)
-        :np.ndarray L:    Gamma scale matrix (for NIG/NIW)
-        :np.ndarray mean: samples mean
-        :np.ndarray S:    samples covariance
-        :int N:           number of samples
+        double k:        Normal std parameter (for NIG/NIW)
+        np.ndarray mu:   Normal mean parameter (for NIG/NIW)
+        int nu:          Gamma df parameter (for NIG/NIW)
+        np.ndarray L:    Gamma scale matrix (for NIG/NIW)
+        np.ndarray mean: samples mean
+        np.ndarray S:    samples covariance
+        int N:           number of samples
     
     Returns:
-        :double:     updated Normal std parameter (for NIG/NIW)
-        :np.ndarray: updated Normal mean parameter (for NIG/NIW)
-        :int:        updated Gamma df parameter (for NIG/NIW)
-        :np.ndarray: updated Gamma scale matrix (for NIG/NIW)
+        double:     updated Normal std parameter (for NIG/NIW)
+        np.ndarray: updated Normal mean parameter (for NIG/NIW)
+        int:        updated Gamma df parameter (for NIG/NIW)
+        np.ndarray: updated Gamma scale matrix (for NIG/NIW)
     """
     k_n  = k + N
     mu_n = (mu*k + N*mean)/k_n
     nu_n = nu + N
     L_n  = L + S + k*N*((mean - mu).T@(mean - mu))/k_n
     return k_n, mu_n, nu_n, L_n
 
 @njit
-def compute_component_suffstats(x, mean, S, N, p_mu, p_k, p_nu, p_L):
+def _compute_component_suffstats(x, mean, S, N, p_mu, p_k, p_nu, p_L):
     """
     Update mean, covariance, number of samples and maximum a posteriori for mean and covariance.
     
     Arguments:
-        :np.ndarray x:    sample to add
-        :np.ndarray mean: mean of samples already in the cluster
-        :np.ndarray cov:  covariance of samples already in the cluster
-        :int N:           number of samples already in the cluster
-        :np.ndarray p_mu: NIG Normal mean parameter
-        :double p_k:      NIG Normal std parameter
-        :int p_nu:        NIG Gamma df parameter
-        :np.ndarray p_L:  NIG Gamma scale matrix
+        np.ndarray x:    sample to add
+        np.ndarray mean: mean of samples already in the cluster
+        np.ndarray cov:  covariance of samples already in the cluster
+        int N:           number of samples already in the cluster
+        np.ndarray p_mu: NIG Normal mean parameter
+        double p_k:      NIG Normal std parameter
+        int p_nu:        NIG Gamma df parameter
+        np.ndarray p_L:  NIG Gamma scale matrix
     
     Returns:
-        :np.ndarray: updated mean
-        :np.ndarray: updated covariance
-        :int:        updated number of samples
-        :np.ndarray: mean (maximum a posteriori)
-        :np.ndarray: covariance (maximum a posteriori)
+        np.ndarray: updated mean
+        np.ndarray: updated covariance
+        int:        updated number of samples
+        np.ndarray: mean (maximum a posteriori)
+        np.ndarray: covariance (maximum a posteriori)
     """
     new_mean  = (mean*N+x)/(N+1)
     new_S     = (S + N*mean.T@mean + x.T@x) - new_mean.T@new_mean*(N+1)
     new_N     = N+1
     new_mu    = ((p_mu*p_k + new_N*new_mean)/(p_k + new_N))[0]
     new_sigma = (p_L + new_S + p_k*new_N*((new_mean - p_mu).T@(new_mean - p_mu))/(p_k + new_N))/(p_nu + new_N - x.shape[-1] - 1)
     
     return new_mean, new_S, new_N, new_mu, new_sigma
 
 #-------------------#
 # Auxiliary classes #
 #-------------------#
 
-class prior:
+class _prior:
     """
     Class to store the NIW prior parameters
     See https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf, sec. 9
     
     Arguments:
-        :double k:        Normal std parameter
-        :np.ndarray mu:   Normal mean parameter
-        :int nu:          Wishart df parameter
-        :np.ndarray L:    Wishart scale matrix
+        double k:        Normal std parameter
+        np.ndarray mu:   Normal mean parameter
+        int nu:          Wishart df parameter
+        np.ndarray L:    Wishart scale matrix
     
     Returns:
-        :prior: instance of prior class
+        prior: instance of prior class
     """
     def __init__(self, k, L, nu, mu):
         self.k   = k
         self.nu  = np.max([nu, mu.shape[-1]+2])
         self.L   = L*(self.nu-mu.shape[-1]-1)
         self.mu  = mu
 
-class component:
+class _component:
     """
     Class to store the relevant informations for each component in the mixture.
     
     Arguments:
-        :np.ndarray x: sample added to the new component
-        :prior prior:  instance of the prior class with NIG/NIW prior parameters
+        np.ndarray x: sample added to the new component
+        prior prior:  instance of the prior class with NIG/NIW prior parameters
     
     Returns:
-        :component: instance of component class
+        component: instance of component class
     """
     def __init__(self, x, prior):
         self.N     = 1
         self.mean  = x
         self.S     = np.identity(x.shape[-1])*0.
         self.mu    = np.atleast_2d((prior.mu*prior.k + self.N*self.mean)/(prior.k + self.N)).astype(np.float64)[0]
         self.sigma = np.identity(x.shape[-1]).astype(np.float64)*prior.L/(prior.nu - x.shape[-1] - 1)
 
-class component_h:
+class _component_h:
     """
     Class to store the relevant informations for each component in the mixture.
     To be used in hierarchical inference.
     
     Arguments:
-        :np.ndarray x:  event added to the new component
-        :int dim:       number of dimensions
-        :prior prior:   instance of the prior class with NIG/NIW prior parameters
-        :double logL_D: logLikelihood denominator
+        np.ndarray x:  event added to the new component
+        int dim:       number of dimensions
+        prior prior:   instance of the prior class with NIG/NIW prior parameters
+        double logL_D: logLikelihood denominator
     
     Returns:
-        :component_h: instance of component_h class
+        component_h: instance of component_h class
     """
     def __init__(self, x, dim, prior, logL_D, mu_MC, sigma_MC, b_ones):
         self.dim    = dim
         self.N      = 1
         self.events = [x]
         self.means  = [x.means]
         self.covs   = [x.covs]
@@ -258,15 +258,15 @@
         idx        = np.random.choice(len(mu_MC), p = np.exp(logL_D - log_norm_D))
         self.mu    = np.copy(mu_MC[idx])
         self.sigma = np.copy(sigma_MC[idx])
         if dim == 1:
             self.mu = np.atleast_2d(self.mu).T
             self.sigma = np.atleast_2d(self.sigma).T
             
-class _density:
+class density:
     """
     Class to initialise a common set of methods for mixture models. Not to be used.
     """
     def __init__(self):
         pass
         
     def __call__(self, x):
@@ -298,44 +298,44 @@
 
     @probit
     def _pdf(self, x):
         """
         Evaluate mixture at point(s) x
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return self._pdf_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
 
     @probit
     def _logpdf(self, x):
         """
         Evaluate log mixture at point(s) x
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return self._logpdf_probit(x) - probit_logJ(x, self.bounds, self.probit)
 
     def fast_pdf(self, x):
         """
         Fast pdf evaluation using FIGARO implementation of log_norm (JIT) rather than Numpy's.
         WARNING: it is meant to be used with MCMC samplers, therefore accepts only one point at a time.
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at
+            np.ndarray x: point to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         x = np.atleast_1d(x)
         if x.shape == (1,self.dim):
             return self._fast_pdf(x[0])
         elif x.shape == (self.dim,):
             return self._fast_pdf(x)
         else:
@@ -343,18 +343,18 @@
 
     def fast_logpdf(self, x):
         """
         Fast logpdf evaluation using FIGARO implementation of log_norm (JIT) rather than Numpy's.
         WARNING: it is meant to be used with MCMC samplers, therefore accepts only one point at a time.
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at
+            np.ndarray x: point to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         x = np.atleast_1d(x)
         if x.shape == (1,self.dim):
             return self._fast_logpdf(x[0])
         elif x.shape == (self.dim,):
             return self._fast_logpdf(x)
         else:
@@ -362,155 +362,155 @@
 
     @probit
     def _fast_pdf(self, x):
         """
         Evaluate mixture at point x
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at
+            np.ndarray x: point to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return self._fast_pdf_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
 
     @probit
     def _fast_logpdf(self, x):
         """
         Evaluate log mixture at point x
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at
+            np.ndarray x: point to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return self._fast_logpdf_probit(x) - probit_logJ(x, self.bounds, self.probit)
 
     def _fast_pdf_probit(self, x):
         """
         Evaluate mixture at point x in probit space
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at (in probit space)
+            np.ndarray x: point to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return np.sum(np.array([w*np.exp(log_norm(x[0], mean, cov)) for mean, cov, w in zip(self.means, self.covs, self.w)]), axis = 0)
 
     def _fast_logpdf_probit(self, x):
         """
         Evaluate log mixture at point x in probit space
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at (in probit space)
+            np.ndarray x: point to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return logsumexp(np.array([w + log_norm(x[0], mean, cov) for mean, cov, w in zip(self.means, self.covs, self.log_w)]), axis = 0)
 
     @probit
     def _pdf_no_jacobian(self, x):
         """
         Evaluate mixture at point(s) x without jacobian
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return self._pdf_probit(x)
 
     def _pdf_probit(self, x):
         """
         Evaluate mixture at point(s) x in probit space
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return np.sum(np.array([w*mn(mean, cov, allow_singular = True).pdf(x) for mean, cov, w in zip(self.means, self.covs, self.w)]), axis = 0)
     
     @probit
     def _pdf_array(self, x):
         """
         Evaluate every mixture component at point(s) x.
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the components at
+            np.ndarray x: point(s) to evaluate the components at
         
         Returns:
-            :np.ndarray: component.pdf(x) for each mixture component
+            np.ndarray: component.pdf(x) for each mixture component
         """
         return _pdf_array_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
 
     def _pdf_array_probit(self, x):
         """
         Evaluate every mixture component at point(s) x.
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the components at (in probit space)
+            np.ndarray x: point(s) to evaluate the components at (in probit space)
         
         Returns:
-            :np.ndarray: component.pdf(x) for each mixture component
+            np.ndarray: component.pdf(x) for each mixture component
         """
         return np.array([w*mn(mean, cov, allow_singular = True).pdf(x) for mean, cov, w in zip(self.means, self.covs, self.w)])
 
     @probit
     def _fast_pdf_array(self, x):
         """
         Evaluate every mixture component at point(s) x.
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the components at
+            np.ndarray x: point(s) to evaluate the components at
         
         Returns:
-            :np.ndarray: component.pdf(x) for each mixture component
+            np.ndarray: component.pdf(x) for each mixture component
         """
         return _fast_pdf_array_probit(x) * np.exp(-probit_logJ(x, self.bounds, self.probit))
 
     def _fast_pdf_array_probit(self, x):
         """
         Evaluate every mixture component at point(s) x.
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the components at (in probit space)
+            np.ndarray x: point(s) to evaluate the components at (in probit space)
         
         Returns:
-            :np.ndarray: component.pdf(x) for each mixture component
+            np.ndarray: component.pdf(x) for each mixture component
         """
         return np.array([w*np.exp(log_norm(x[0], mean, cov)) for mean, cov, w in zip(self.means, self.covs, self.w)])
 
     @probit
     def _logpdf_no_jacobian(self, x):
         """
         Evaluate log mixture at point(s) x without jacobian
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return self._logpdf_probit(x)
 
     def _logpdf_probit(self, x):
         """
         Evaluate log mixture at point(s) x in probit space
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return logsumexp(np.array([w + mn(mean, cov, allow_singular = True).logpdf(x) for mean, cov, w in zip(self.means, self.covs, self.log_w)]), axis = 0)
 
     def cdf(self, x):
         if self.dim > 1:
             raise FIGAROException("cdf is provided only for 1-dimensional distributions")
         if len(np.shape(x)) < 2:
@@ -526,58 +526,58 @@
 
     @probit
     def _cdf(self, x):
         """
         Evaluate mixture cdf at point(s) x
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.cdf(x)
+            np.ndarray: mixture.cdf(x)
         """
         return np.sum(np.array([w*norm(mean[0], cov[0,0]).cdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.w)]), axis = 0)
 
     @probit
     def _logcdf(self, x):
         """
         Evaluate mixture log cdf at point(s) x
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at
+            np.ndarray x: point(s) to evaluate the mixture at
         
         Returns:
-            :np.ndarray: mixture.logcdf(x)
+            np.ndarray: mixture.logcdf(x)
         """
         return logsumexp(np.array([w + norm(mean[0], cov[0,0]).logcdf(x) for mean, cov, w in zip(self.means, np.sqrt(self.covs), self.log_w)]), axis = 0)
 
     @from_probit
     def rvs(self, size = 1):
         """
         Draw samples from mixture
         
         Arguments:
-            :int size: number of samples to draw
+            int size: number of samples to draw
         
         Returns:
-            :np.ndarray: samples
+            np.ndarray: samples
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to draw samples from an empty mixture.\n If you are using the density_from_samples() method, you may want to draw samples from the output of that method.")
         return self._rvs_probit(size)
         
     def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
         
         Arguments:
-            :int size: number of samples to draw
+            int size: number of samples to draw
         
         Returns:
-            :np.ndarray: samples in probit space
+            np.ndarray: samples in probit space
         """
         idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = size)
         ctr = Counter(idx)
         if self.dim > 1:
             samples = np.empty(shape = (1,self.dim))
             for i, n in zip(ctr.keys(), ctr.values()):
                 samples = np.concatenate((samples, np.atleast_2d(mn(self.means[i], self.covs[i], allow_singular = True).rvs(size = n))))
@@ -588,18 +588,18 @@
         return np.array(samples[1:])
     
     def gradient(self, x):
         """
         Gradient of the mixture.
         
         Arguments:
-            :np.ndarray x: point to evaluate the gradient at
+            np.ndarray x: point to evaluate the gradient at
         
         Returns:
-            :np.ndarray: gradient
+            np.ndarray: gradient
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
         if len(np.shape(x)) < 2:
             if self.dim == 1:
                 x = np.atleast_2d(x).T
             else:
@@ -609,18 +609,18 @@
         return g
     
     def log_gradient(self, x):
         """
         Logarithmic gradient of the mixture.
         
         Arguments:
-            :np.ndarray x: point to evaluate the gradient at
+            np.ndarray x: point to evaluate the gradient at
         
         Returns:
-            :np.ndarray: logarithmic gradient
+            np.ndarray: logarithmic gradient
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to evaluate an empty mixture.\n If you are using the density_from_samples() method, you may want to evaluate the output of that method.")
         if len(np.shape(x)) < 2:
             if self.dim == 1:
                 x = np.atleast_2d(x).T
             else:
@@ -630,55 +630,55 @@
         return g
     
     def _gradient(self, x):
         """
         Gradient of the mixture.
         
         Arguments:
-            :np.ndarray x: point to evaluate the gradient at
+            np.ndarray x: point to evaluate the gradient at
         
         Returns:
-            :np.ndarray: gradient
+            np.ndarray: gradient
         """
         return self._fast_pdf(x)*self._log_gradient(x)
     
     @probit
     def _log_gradient(self, x):
         """
         Logarithmic gradient of the mixture.
         
         Arguments:
-            :np.ndarray x: point to evaluate the gradient at
+            np.ndarray x: point to evaluate the gradient at
         
         Returns:
-            :np.ndarray: logarithmic gradient
+            np.ndarray: logarithmic gradient
         """
         p = self._pdf_array_probit(x)
         B = np.array([-np.dot(inv_jit(sigma),(x - mu)) for mu, sigma in zip(self.means, self.covs)])
         try:
             return np.average(B, weights = p, axis = 0) + log_gradient_inv_jacobian(x, self.bounds, self.probit)
         except ZeroDivisionError:
             return np.zeros(x.shape[-1])
 
-class mixture(_density):
+class mixture(density):
     """
     Class to store a single draw from DPGMM/(H)DPGMM.
-    Methods inherited from _density class.
+    Methods inherited from density class.
     
     Arguments:
-        :iterable means:    component means
-        :iterable covs:     component covariances
-        :np.ndarray w:      component weights
-        :np.ndarray bounds: bounds of probit transformation
-        :int dim:           number of dimensions
-        :int n_cl:          number of clusters in the mixture
-        :bool probit:       whether to use the probit transformation or not
+        iterable means:    component means
+        iterable covs:     component covariances
+        np.ndarray w:      component weights
+        np.ndarray bounds: bounds of probit transformation
+        int dim:           number of dimensions
+        int n_cl:          number of clusters in the mixture
+        bool probit:       whether to use the probit transformation or not
     
     Returns:
-        :mixture: instance of mixture class
+        mixture: instance of mixture class
     """
     def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, probit = True, log_w = None):
         self.means  = means
         self.covs   = covs
         if log_w is None:
             self.w      = w
             self.log_w  = np.log(w)
@@ -692,66 +692,68 @@
         self.probit = probit
     
     def marginalise(self, axis = -1):
         """
         Marginalise out one or more dimensions from the mixture.
         
         Arguments:
-            :int or list of int axis: axis to marginalise on. Default: last
+            int or list of int axis: axis to marginalise on. Default: last
         
         Returns:
-            :figaro.mixture.mixture: marginalised mixture
+            figaro.mixture.mixture: marginalised mixture
         """
         return _marginalise(self, axis)
     
-    def condition(self, vals, dims, norm = True):
+    def condition(self, vals, dims, norm = True, filter = True, tol = 1e-3):
         """
         Mixture conditioned on specific values of a subset of parameters.
         
         Arguments:
-            :iterable vals:           value(s) to condition on
-            :int or list of int dims: dimension(s) associated with given vals (starting from 0)
-            :bool norm:               whether to normalize the distribution or not
+            iterable vals:           value(s) to condition on
+            int or list of int dims: dimension(s) associated with given vals (starting from 0)
+            bool norm:               whether to normalize the distribution or not
+            bool filter:             filter the components with weight < tol
+            double tol:              tolerance on the sum of the weights
         
         Returns:
-            :figaro.mixture.mixture: conditioned mixture
+            figaro.mixture.mixture: conditioned mixture
         """
         v       = np.mean(self.bounds, axis = -1)
         v[dims] = vals
-        return _condition(self, v, dims, norm)
+        return _condition(self, v, dims, norm, filter, tol = 1e-3)
     
 #-------------------#
 # Inference classes #
 #-------------------#
 
-class DPGMM(_density):
+class DPGMM(density):
     """
     Class to infer a distribution given a set of samples.
     
     Arguments:
-        :iterable bounds:     boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
-        :iterable prior_pars: NIW prior parameters (k, L, nu, mu)
-        :double alpha0:       initial guess for concentration parameter
-        :bool probit:         whether to use the probit transformation or not
+        iterable bounds:     boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
+        iterable prior_pars: NIW prior parameters (k, L, nu, mu)
+        double alpha0:       initial guess for concentration parameter
+        bool probit:         whether to use the probit transformation or not
     
     Returns:
-        :DPGMM: instance of DPGMM class
+        DPGMM: instance of DPGMM class
     """
     def __init__(self, bounds,
                        prior_pars = None,
                        alpha0     = 1.,
                        probit     = True,
                        ):
         self.probit = probit
         self.bounds = np.atleast_2d(bounds)
         self.dim    = len(self.bounds)
         if prior_pars is not None:
-            self.prior = prior(*prior_pars)
+            self.prior = _prior(*prior_pars)
         else:
-            self.prior = prior(*get_priors(bounds = self.bounds, probit = self.probit))
+            self.prior = _prior(*get_priors(bounds = self.bounds, probit = self.probit))
         self.alpha      = alpha0
         self.alpha_0    = alpha0
         self.mixture    = []
         self.w          = []
         self.log_w      = []
         self.N_list     = []
         self.n_cl       = 0
@@ -761,71 +763,71 @@
         return self.pdf(x)
 
     def initialise(self, prior_pars = None):
         """
         Initialise the mixture to initial conditions.
         
         Arguments:
-            :iterable prior_pars: NIW prior parameters (k, L, nu, mu). If None, old parameters are kept
+            iterable prior_pars: NIW prior parameters (k, L, nu, mu). If None, old parameters are kept
         """
         self.alpha    = self.alpha_0
         self.mixture  = []
         self.w        = []
         self.log_w    = []
         self.N_list   = []
         self.n_cl     = 0
         self.n_pts    = 0
         if prior_pars is not None:
-            self.prior = prior(*prior_pars)
+            self.prior = _prior(*prior_pars)
         
     def _add_datapoint_to_component(self, x, ss):
         """
         Update component parameters after assigning a sample to a component
         
         Arguments:
-            :np.ndarray x: sample
-            :component ss: component to update
+            np.ndarray x: sample
+            component ss: component to update
         
         Returns:
-            :component: updated component
+            component: updated component
         """
-        new_mean, new_S, new_N, new_mu, new_sigma = compute_component_suffstats(x, ss.mean, ss.S, ss.N, self.prior.mu, self.prior.k, self.prior.nu, self.prior.L)
+        new_mean, new_S, new_N, new_mu, new_sigma = _compute_component_suffstats(x, ss.mean, ss.S, ss.N, self.prior.mu, self.prior.k, self.prior.nu, self.prior.L)
         ss.mean  = new_mean
         ss.S     = new_S
         ss.N     = new_N
         ss.mu    = new_mu
         ss.sigma = new_sigma
         return ss
     
     def _log_predictive_likelihood(self, x, ss):
         """
         Compute log likelihood of drawing sample x from component ss given the samples that are already assigned to that component.
         
         Arguments:
-            :np.ndarray x: sample
-            :component ss: component to update
+            np.ndarray x: sample
+            component ss: component to update
         
         Returns:
-            :double: log Likelihood
+            double: log Likelihood
         """
         if ss is None:
-            ss = component(np.zeros(self.dim), prior = self.prior)
+            ss = _component(np.zeros(self.dim), prior = self.prior)
             ss.N = 0.
-        t_df, t_shape, mu_n = compute_t_pars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
+        t_df, t_shape, mu_n = _compute_t_pars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N, self.dim)
         return _student_t(df = t_df, t = x, mu = mu_n, sigma = t_shape, dim = self.dim)
 
     def _cluster_assignment_distribution(self, x):
         """
         Compute the marginal distribution of cluster assignment for each cluster.
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         
         Returns:
-            :dict: p_i for each component
+            dict: p_i for each component
         """
         scores = np.zeros(self.n_cl+1)
         for i in range(self.n_cl+1):
             if i == 0:
                 ss        = None
                 scores[i] = np.log(self.alpha)
             else:
@@ -836,20 +838,20 @@
         return np.exp(scores - norm)
 
     def _assign_to_cluster(self, x):
         """
         Assign the new sample x to an existing cluster or to a new cluster according to the marginal distribution of cluster assignment.
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         """
         scores = self._cluster_assignment_distribution(x)
         cid = np.random.choice(self.n_cl+1, p=scores)
         if cid == 0:
-            self.mixture.append(component(x, prior = self.prior))
+            self.mixture.append(_component(x, prior = self.prior))
             self.N_list.append(1.)
             self.n_cl += 1
         else:
             self.mixture[int(cid)-1] = self._add_datapoint_to_component(x, self.mixture[int(cid)-1])
             self.N_list[int(cid)-1] += 1
         # Update weights
         self.w = np.array(self.N_list)
@@ -858,18 +860,18 @@
         return
     
     def density_from_samples(self, samples):
         """
         Reconstruct the probability density from a set of samples.
         
         Arguments:
-            :iterable samples: samples set
+            iterable samples: samples set
         
         Returns:
-            :mixture: the inferred mixture
+            mixture: the inferred mixture
         """
         np.random.shuffle(samples)
         samples = np.ascontiguousarray(samples)
         for s in samples:
             self.add_new_point(s)
         d = self.build_mixture()
         self.initialise()
@@ -877,48 +879,48 @@
     
     @probit
     def add_new_point(self, x):
         """
         Update the probability density reconstruction adding a new sample
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         """
         self.n_pts += 1
         self._assign_to_cluster(np.atleast_2d(x))
-        self.alpha = update_alpha(self.alpha, self.n_pts, self.n_cl)
+        self.alpha = _update_alpha(self.alpha, self.n_pts, self.n_cl)
 
     def build_mixture(self):
         """
         Instances a mixture class representing the inferred distribution
         
         Returns:
-            :mixture: the inferred distribution
+            mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
         means     = np.zeros((self.n_cl, self.dim))
         variances = np.zeros((self.n_cl, self.dim, self.dim))
         for i, ss in enumerate(self.mixture):
-            k_n, mu_n, nu_n, L_n = compute_hyperpars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
+            k_n, mu_n, nu_n, L_n = _compute_hyperpars(self.prior.k, self.prior.mu, self.prior.nu, self.prior.L, ss.mean, ss.S, ss.N)
             variances[i] = invwishart(df = nu_n, scale = L_n).rvs()
             means[i]     = mn(mean = mu_n[0], cov = variances[i]/k_n, allow_singular = True).rvs()
         w = dirichlet(self.w*self.n_pts+self.alpha/self.n_cl).rvs()[0]
         return mixture(means, variances, w, self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
 
-    # Methods to overwrite _density methods
+    # Methods to overwrite density methods
     def _rvs_probit(self, size = 1):
         """
         Draw samples from mixture in probit space
         
         Arguments:
-            :int size: number of samples to draw
+            int size: number of samples to draw
         
         Returns:
-            :np.ndarray: samples in probit space
+            np.ndarray: samples in probit space
         """
         idx = np.random.choice(np.arange(self.n_cl), p = self.w, size = size)
         ctr = Counter(idx)
         if self.dim > 1:
             samples = np.empty(shape = (1,self.dim))
             for i, n in zip(ctr.keys(), ctr.values()):
                 samples = np.concatenate((samples, np.atleast_2d(mn(self.mixture[i].mu, self.mixture[i].sigma, allow_singular = True).rvs(size = n))))
@@ -929,72 +931,72 @@
         return samples[1:]
 
     def _pdf_probit(self, x):
         """
         Evaluate mixture at point(s) x in probit space
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return np.sum(np.array([w*mn(comp.mu, comp.sigma, allow_singular = True).pdf(x) for comp, w in zip(self.mixture, self.w)]), axis = 0)
 
     def _logpdf_probit(self, x):
         """
         Evaluate log mixture at point(s) x in probit space
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return logsumexp(np.array([w + mn(comp.mu, comp.sigma, allow_singular = True).logpdf(x) for comp, w in zip(self.mixture, self.log_w)]), axis = 0)
 
     def _fast_pdf_probit(self, x):
         """
         Evaluate mixture at point x in probit space
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at (in probit space)
+            np.ndarray x: point to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         return np.sum(np.array([w*np.exp(log_norm(x[0], comp.mean, comp.cov)) for comp, w in zip(self.mixture, self.w)]), axis = 0)
 
     def _fast_logpdf_probit(self, x):
         """
         Evaluate log mixture at point x in probit space
         
         Arguments:
-            :np.ndarray x: point to evaluate the mixture at (in probit space)
+            np.ndarray x: point to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         return logsumexp(np.array([w + log_norm(x[0], comp.mean, comp.cov) for comp, w in zip(self.mixture, self.log_w)]), axis = 0)
 
 class HDPGMM(DPGMM):
     """
     Class to infer a distribution given a set of observations (each being a set of samples).
     Child of DPGMM class
     
     Arguments:
-        :iterable bounds:  boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
-        :double alpha0:    initial guess for concentration parameter
-        :double MC_draws:  number of MC draws for integral
-        :bool probit:      whether to use the probit transformation or not
-        :double sigma_min: lower bound for Jeffreys' prior on standard deviation
-        :double sigma_max: upper bound for Jeffreys' prior on standard deviation
+        iterable bounds:  boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
+        double alpha0:    initial guess for concentration parameter
+        double MC_draws:  number of MC draws for integral
+        bool probit:      whether to use the probit transformation or not
+        double sigma_min: lower bound for Jeffreys' prior on standard deviation
+        double sigma_max: upper bound for Jeffreys' prior on standard deviation
     
     Returns:
-        :HDPGMM: instance of HDPGMM class
+        HDPGMM: instance of HDPGMM class
     """
     def __init__(self, bounds,
                        alpha0     = 1.,
                        prior_pars = None,
                        MC_draws   = None,
                        probit     = True,
                        ):
@@ -1039,30 +1041,30 @@
             self.sigma_MC = np.array([r*np.outer(s,s) for r, s in zip(rhos, np.sqrt(self.sigma_MC))])
             
     def add_new_point(self, ev):
         """
         Update the probability density reconstruction adding a new sample
         
         Arguments:
-            :iterable x: set of single-event draws from a DPGMM inference
+            iterable ev: set of single-event draws from a DPGMM inference
         """
         self.n_pts += 1
         x = np.random.choice(ev)
         self._assign_to_cluster(x)
-        self.alpha = update_alpha(self.alpha, self.n_pts, self.n_cl)
+        self.alpha = _update_alpha(self.alpha, self.n_pts, self.n_cl)
 
     def _cluster_assignment_distribution(self, x):
         """
         Compute the marginal distribution of cluster assignment for each cluster.
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         
         Returns:
-            :dict: p_i for each component
+            dict: p_i for each component
         """
         scores = np.zeros(self.n_cl+1)
         logL_N = np.zeros((self.n_cl+1, self.MC_draws))
         
         if self.dim == 1:
             logL_x = evaluate_mixture_MC_draws_1d(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w)
         else:
@@ -1083,23 +1085,23 @@
         return scores, logL_N
 
     def _assign_to_cluster(self, x):
         """
         Assign the new sample x to an existing cluster or to a new cluster according to the marginal distribution of cluster assignment.
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         """
         scores, logL_N = self._cluster_assignment_distribution(x)
         try:
             cid = np.random.choice(self.n_cl+1, p=scores)
         except ValueError:
             cid = 0
         if cid == 0:
-            self.mixture.append(component_h(x, self.dim, self.prior, logL_N[cid], self.mu_MC, self.sigma_MC, self.b_ones))
+            self.mixture.append(_component_h(x, self.dim, self.prior, logL_N[cid], self.mu_MC, self.sigma_MC, self.b_ones))
             self.N_list.append(1.)
             self.n_cl += 1
         else:
             self.mixture[int(cid)-1] = self._add_datapoint_to_component(x, self.mixture[int(cid)-1], logL_N[int(cid)])
             self.N_list[int(cid)-1] += 1
         # Update weights
         self.w = np.array(self.N_list)
@@ -1108,20 +1110,20 @@
         return
 
     def _add_datapoint_to_component(self, x, ss, logL_D):
         """
         Update component parameters after assigning a sample to a component
         
         Arguments:
-            :np.ndarray x: sample
-            :component ss: component to update
-            :double logL_D: log Likelihood denominator
+            np.ndarray x: sample
+            component ss: component to update
+            double logL_D: log Likelihood denominator
         
         Returns:
-            :component: updated component
+            component: updated component
         """
         ss.events.append(x)
         ss.means.append(x.means)
         ss.covs.append(x.covs)
         ss.log_w.append(x.log_w)
         ss.logL_D = logL_D
 
@@ -1138,29 +1140,29 @@
         return ss
 
     def build_mixture(self):
         """
         Instances a mixture class representing the inferred distribution
         
         Returns:
-            :mixture: the inferred distribution
+            mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
         return mixture(np.array([comp.mu for comp in self.mixture]), np.array([comp.sigma for comp in self.mixture]), np.array(self.w), self.bounds, self.dim, self.n_cl, self.n_pts, probit = self.probit)
 
     def density_from_samples(self, events):
         """
         Reconstruct the probability density from a set of samples.
         
         Arguments:
-            :iterable samples: set of single-event draws from DPGMM
+            iterable samples: set of single-event draws from DPGMM
         
         Returns:
-            :mixture: the inferred mixture
+            mixture: the inferred mixture
         """
         np.random.shuffle(events)
         for ev in events:
             self.add_new_point(ev)
         d = self.build_mixture()
         self.initialise()
         return d
```

### Comparing `figaro-1.1.1/figaro/montecarlo.py` & `figaro-1.1.2/figaro/montecarlo.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     Monte Carlo integration using FIGARO reconstructions.
         ∫p(x)q(x)dx ~ ∑p(x_i)/N with x_i ~ q(x)
     
     p(x) must have a pdf() method and q(x) must have a rvs() method.
     Lists of p and q are also accepted.
     
     Arguments:
-        :list or class instance p: the probability density to evaluate. Must have a pdf() method.
-        :list or class instance q: the probability density to sample from. Must have a rvs() method.
-        :int n_draws:              number of MC draws
-        :bool error:               whether to return the uncertainty on the integral value or not.
+        list or class instance p: the probability density to evaluate. Must have a pdf() method.
+        list or class instance q: the probability density to sample from. Must have a rvs() method.
+        int n_draws:              number of MC draws
+        bool error:               whether to return the uncertainty on the integral value or not.
     
     Return:
-        :double: integral value
-        :double: uncertainty (if error = True)
+        double: integral value
+        double: uncertainty (if error = True)
     """
     # Check that both p and q are iterables or callables:
     if not ((hasattr(p, 'pdf') or np.iterable(p)) and (hasattr(q, 'rvs') or np.iterable(q))):
         raise FIGAROException("p and q must be list of callables or having pdf/rvs methods")
     # Number of p draws and methods check
     if np.iterable(p):
         if not np.alltrue([hasattr(pi, 'pdf') for pi in p]):
```

### Comparing `figaro-1.1.1/figaro/pipelines/create_glade.py` & `figaro-1.1.2/figaro/pipelines/create_glade.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/entropy.py` & `figaro-1.1.2/figaro/pipelines/entropy.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/gen_mock_data.py` & `figaro-1.1.2/figaro/pipelines/gen_mock_data.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/hierarchical_inference.py` & `figaro-1.1.2/figaro/pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/par_hierarchical_inference.py` & `figaro-1.1.2/figaro/pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/par_probability_density.py` & `figaro-1.1.2/figaro/pipelines/par_probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/ppplot.py` & `figaro-1.1.2/figaro/pipelines/ppplot.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/pipelines/probability_density.py` & `figaro-1.1.2/figaro/pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/plot.py` & `figaro-1.1.2/figaro/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,32 +99,32 @@
 projection_registry.register(PPPlot)
 
 def plot_median_cr(draws, injected = None, samples = None, selfunc = None, bounds = None, out_folder = '.', name = 'density', n_pts = 1000, label = None, unit = None, hierarchical = False, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = None):
     """
     Plot the recovered 1D distribution along with the injected distribution and samples from the true distribution (both if available).
     
     Arguments:
-        :iterable draws:                  container for mixture instances
-        :callable or np.ndarray injected: injected distribution (if available)
-        :np.ndarray samples:              samples from the true distribution (if available)
-        :callable or np.ndarray selfunc:  selection function (if available)
-        :iterable bounds:                 bounds for the recovered distribution. If None, bounds from mixture instances are used.
-        :str or Path out_folder:          output folder
-        :str name:                        name to be given to outputs
-        :int n_pts:                       number of points for linspace
-        :str label:                       LaTeX-style quantity label, for plotting purposes
-        :str unit:                        LaTeX-style quantity unit, for plotting purposes
-        :bool hierarchical:               hierarchical inference, for plotting purposes
-        :bool save:                       whether to save the plots or not
-        :bool show:                       whether to show the plots during the run or not
-        :bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
-        :float true_value:                true value to infer
-        :str true_value_label:            label to assign to the true value marker
-        :str injected_label:              label to assign to the injected distribution
-        :str median_label:                label to assign to the reconstruction
+        iterable draws:                  container for mixture instances
+        callable or np.ndarray injected: injected distribution (if available)
+        np.ndarray samples:              samples from the true distribution (if available)
+        callable or np.ndarray selfunc:  selection function (if available)
+        iterable bounds:                 bounds for the recovered distribution. If None, bounds from mixture instances are used.
+        str or Path out_folder:          output folder
+        str name:                        name to be given to outputs
+        int n_pts:                       number of points for linspace
+        str label:                       LaTeX-style quantity label, for plotting purposes
+        str unit:                        LaTeX-style quantity unit, for plotting purposes
+        bool hierarchical:               hierarchical inference, for plotting purposes
+        bool save:                       whether to save the plots or not
+        bool show:                       whether to show the plots during the run or not
+        bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
+        float true_value:                true value to infer
+        str true_value_label:            label to assign to the true value marker
+        str injected_label:              label to assign to the injected distribution
+        str median_label:                label to assign to the reconstruction
     """
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
             median_label = '\mathrm{DPGMM}'
     
@@ -297,31 +297,31 @@
     
 
 def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None):
     """
     Plot the recovered multidimensional distribution along with samples from the true distribution (if available) as corner plot.
     
     Arguments:
-        :iterable draws:         container for mixture instances
-        :int dim:                number of dimensions
-        :np.ndarray samples:     samples from the true distribution (if available)
-        :iterable bounds:        bounds for the recovered distribution. If None, bounds from mixture instances are used.
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :list-of-str labels:     LaTeX-style quantity label, for plotting purposes
-        :list-of-str units:      LaTeX-style quantity unit, for plotting purposes
-        :bool hierarchical:      hierarchical inference, for plotting purposes
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
-        :bool subfolder:         whether to save in a dedicated subfolder
-        :int n_pts:              number of grid points (same for each dimension)
-        :iterable true_value:    true value to plot
-        :iterable levels:        credible levels to plot
-        :bool scatter_points:    scatter samples on 2d plots
-        :str median_label:       label to assign to the reconstruction
+        iterable draws:         container for mixture instances
+        int dim:                number of dimensions
+        np.ndarray samples:     samples from the true distribution (if available)
+        iterable bounds:        bounds for the recovered distribution. If None, bounds from mixture instances are used.
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        list-of-str labels:     LaTeX-style quantity label, for plotting purposes
+        list-of-str units:      LaTeX-style quantity unit, for plotting purposes
+        bool hierarchical:      hierarchical inference, for plotting purposes
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
+        bool subfolder:         whether to save in a dedicated subfolder
+        int n_pts:              number of grid points (same for each dimension)
+        iterable true_value:    true value to plot
+        iterable levels:        credible levels to plot
+        bool scatter_points:    scatter samples on 2d plots
+        str median_label:       label to assign to the reconstruction
     """
     
     dim = draws[0].dim
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
@@ -518,31 +518,31 @@
 def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False):
     """
     Plot a 1D distribution along with samples from the true distribution (if available).
     Differently from plot_median_cr, this method requires the distribution to be already evaluated.
     For FIGARO mixture instances, please use plot_median_cr.
 
     Arguments:
-        :iterable x:                      values at which realisations are evaluated
-        :iterable draws:                  container for realisations
-        :callable or np.ndarray injected: injected distribution (if available)
-        :np.ndarray samples:              samples from the true distribution (if available)
-        :str or Path out_folder:          output folder
-        :str name:                        name to be given to outputs
-        :str label:                       LaTeX-style quantity label, for plotting purposes
-        :str unit:                        LaTeX-style quantity unit, for plotting purposes
-        :bool save:                       whether to save the plots or not
-        :bool show:                       whether to show the plots during the run or not
-        :bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
-        :float true_value:                true value to infer
-        :str true_value_label:            label to assign to the true value marker
-        :str injected_label:              label to assign to the injected distribution
-        :str median_label:                label to assign to the median distribution
-        :bool logx:                       x log scale
-        :bool logy:                       y log scale
+        iterable x:                      values at which realisations are evaluated
+        iterable draws:                  container for realisations
+        callable or np.ndarray injected: injected distribution (if available)
+        np.ndarray samples:              samples from the true distribution (if available)
+        str or Path out_folder:          output folder
+        str name:                        name to be given to outputs
+        str label:                       LaTeX-style quantity label, for plotting purposes
+        str unit:                        LaTeX-style quantity unit, for plotting purposes
+        bool save:                       whether to save the plots or not
+        bool show:                       whether to show the plots during the run or not
+        bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
+        float true_value:                true value to infer
+        str true_value_label:            label to assign to the true value marker
+        str injected_label:              label to assign to the injected distribution
+        str median_label:                label to assign to the median distribution
+        bool logx:                       x log scale
+        bool logy:                       y log scale
     """
     
     if not np.shape(x)[0] == np.shape(draws)[-1]:
         raise ValueError("x and each draw must have the same length")
     
     percentiles = [50, 5, 16, 84, 95]
     p = {}
@@ -628,20 +628,20 @@
     
 
 def plot_n_clusters_alpha(n_cl, alpha, out_folder = '.', name = 'event', show = False, save = True):
     """
     Plot the number of clusters and the concentration parameter as functions of the number of samples.
     
     Arguments:
-        :np.ndarray n_cl:        number of active clusters
-        :np.ndarray alpha:       concentration parameter
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        np.ndarray n_cl:        number of active clusters
+        np.ndarray alpha:       concentration parameter
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     """
     fig, ax = plt.subplots()
     ax1 = ax.twinx()
     ax.plot(np.arange(1, len(n_cl)+1), n_cl, ls = '--', marker = '', lw = 0.7, color = 'k')
     ax1.plot(np.arange(1, len(alpha)+1), alpha, ls = '--', marker = '', lw = 0.7, color = 'r')
     ax.set_xlabel('$t$')
     ax.set_ylabel('$N_{\mathrm{cl}}(t)$', color = 'k')
@@ -653,21 +653,21 @@
     plt.close()
 
 def pp_plot_cdf(draws, injection, n_points = 1000, out_folder = '.', name = 'event', show = False, save = True):
     """
     Make pp-plot comparing draws cdfs and injection cdf
     
     Arguments:
-        :iterable draws:         container of mixture instances
-        :callable injection:     injected density
-        :int n_points:           number of points for linspace
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        iterable draws:         container of mixture instances
+        callable injection:     injected density
+        int n_points:           number of points for linspace
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     """
     all_bounds = np.atleast_2d([d.bounds[0] for d in draws])
     x_min = np.max(all_bounds[:,0])
     x_max = np.min(all_bounds[:,1])
     x = np.linspace(x_min, x_max, n_points)
     
     functions     = np.array([mix(x) for mix in draws])
@@ -692,20 +692,20 @@
     plt.close()
 
 def pp_plot_levels(CR_levels, median_CR = None, out_folder = '.', name = 'MDC', show = False, save = True):
     """
     Make pp-plot.
     
     Arguments:
-        :iterable CR:            2D array with credible levels for each event
-        :iterable median_CR:     credible levels of medians
-        :str or Path out_folder: output folder
-        :str name:               name to be given to outputs
-        :bool save:              whether to save the plot or not
-        :bool show:              whether to show the plot during the run or not
+        iterable CR:            2D array with credible levels for each event
+        iterable median_CR:     credible levels of medians
+        str or Path out_folder: output folder
+        str name:               name to be given to outputs
+        bool save:              whether to save the plot or not
+        bool show:              whether to show the plot during the run or not
     """
     CR_levels = np.atleast_1d(CR_levels)
     if len(CR_levels.shape) > 1:
         CR_levels = CR_levels.T
     n_evs     = CR_levels.shape[-1]
     L         = np.linspace(0,1,n_evs+2)
```

### Comparing `figaro-1.1.1/figaro/plot_settings.py` & `figaro-1.1.2/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.1.1/figaro/threeDvolume.py` & `figaro-1.1.2/figaro/threeDvolume.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,36 +43,36 @@
 
 @njit
 def log_add(x, y):
     """
     Compute log(np.exp(x) + np.exp(y))
     
     Arguments:
-        :double x: first addend (log)
-        :double y: second addend (log)
+        double x: first addend (log)
+        double y: second addend (log)
     
     Returns:
-        :double: log(np.exp(x) + np.exp(y))
+        double: log(np.exp(x) + np.exp(y))
     """
     if x >= y:
         return x+np.log1p(np.exp(y-x))
     else:
         return y+np.log1p(np.exp(x-y))
 
 @njit
 def log_add_array(x,y):
     """
     Compute log(np.exp(x) + np.exp(y)) element-wise
     
     Arguments:
-        :np.ndarray x: first addend (log)
-        :np.ndarray y: second addend (log)
+        np.ndarray x: first addend (log)
+        np.ndarray y: second addend (log)
     
     Returns:
-        :np.ndarray: log(np.exp(x) + np.exp(y)) element-wise
+        np.ndarray: log(np.exp(x) + np.exp(y)) element-wise
     """
     res = np.zeros(len(x), dtype = np.float64)
     for i in prange(len(x)):
         res[i] = log_add(x[i],y[i])
     return res
 
 # natural sorting.
@@ -91,38 +91,38 @@
 
 class VolumeReconstruction(DPGMM):
     """
     Class to reconstruct the 3D probability density given a set of samples or during a PE run.
     Child class of DPGMM class (defined in mixture.py)
     
     Arguments:
-        :double max_dist:          maximum distance (in Mpc)
-        :str or Path out_folder:   output folder
-        :tuple prior_pars:         NIW prior parameters (k, L, nu, mu - see https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf)
-        :double alpha0:            initial guess for concentration parameter
-        :list-of-int n_gridpoints: number of gridpoints for each dimension (ra, dec, dist). Default is set to have a 0.25 deg^2 resolution
-        :str name:                 name to be given to output folders and files
-        :list-of-str labels:       plot labels
-        :list-of-double levels:    credible levels (between 0 and 1)
-        :bool latex:               if True, LaTeX is used for plots (if available)
-        :bool incr_plot:           if True, produce plots at fixed number of samples. Otherwise, skymaps are produced at the end of the inference only
-        :str or Path glade_file:   file containing GLADE+ (hdf5 file created using the create_glade.py pipeline)
-        :dict cosmology:           dictionary containing h = H0/100 km/(s*Mpc), om (matter density parameter) and ol (cosmological constant density). Default from Planck (2021)
-        :int n_gal_to_plot:        number of galaxies to include in galaxy plots
-        :double region_to_plot:    credible region to plot
-        :bool entropy:             use entropy to assess convergence and begin producing skymaps
-        :list-of-double true_host: position of the true host, if known
-        :str host_name:            host name, for plotting purposes
-        :int entropy_step:         interval (expressed as number of draws) between two subsequent entropy evaluations
-        :int entropy_ac_step:      window lenght for entropy angular coefficient
-        :int n_sign_changes:       number of zero-crossings before beginning producing skymaps (requires entropy = True)
-        :bool virtual_observatory: places the virtual observatory fov behind galaxy plots. Warning: under development, might not work
+        double max_dist:          maximum distance (in Mpc)
+        str or Path out_folder:   output folder
+        tuple prior_pars:         NIW prior parameters (k, L, nu, mu - see https://www.cs.ubc.ca/~murphyk/Papers/bayesGauss.pdf)
+        double alpha0:            initial guess for concentration parameter
+        list-of-int n_gridpoints: number of gridpoints for each dimension (ra, dec, dist). Default is set to have a 0.25 deg^2 resolution
+        str name:                 name to be given to output folders and files
+        list-of-str labels:       plot labels
+        list-of-double levels:    credible levels (between 0 and 1)
+        bool latex:               if True, LaTeX is used for plots (if available)
+        bool incr_plot:           if True, produce plots at fixed number of samples. Otherwise, skymaps are produced at the end of the inference only
+        str or Path glade_file:   file containing GLADE+ (hdf5 file created using the create_glade.py pipeline)
+        dict cosmology:           dictionary containing h = H0/100 km/(s*Mpc), om (matter density parameter) and ol (cosmological constant density). Default from Planck (2021)
+        int n_gal_to_plot:        number of galaxies to include in galaxy plots
+        double region_to_plot:    credible region to plot
+        bool entropy:             use entropy to assess convergence and begin producing skymaps
+        list-of-double true_host: position of the true host, if known
+        str host_name:            host name, for plotting purposes
+        int entropy_step:         interval (expressed as number of draws) between two subsequent entropy evaluations
+        int entropy_ac_step:      window lenght for entropy angular coefficient
+        int n_sign_changes:       number of zero-crossings before beginning producing skymaps (requires entropy = True)
+        bool virtual_observatory: places the virtual observatory fov behind galaxy plots. Warning: under development, might not work
     
     Returns:
-        :VolumeReconstruction: instance of VolumeReconstruction class
+        VolumeReconstruction: instance of VolumeReconstruction class
     """
     def __init__(self, max_dist,
                        out_folder          = '.',
                        prior_pars          = (1e-3, np.identity(3)*0.01**2, 10, np.zeros(3)),
                        alpha0              = 1,
                        n_gridpoints        = [720, 360, 100], # RA, dec, DL
                        name                = 'skymap',
@@ -258,16 +258,16 @@
         self.make_folders()
     
     def initialise(self, true_host = None, out_folder = None, incr_plot = None, entropy = None, name = None):
         """
         Initialise the mixture to initial conditions to analyse a new event.
         
         Arguments:
-            :list-of-doubles true_host: true host for a new GW event
-            :str or Path out_folder:    new output folder
+            list-of-doubles true_host: true host for a new GW event
+            str or Path out_folder:    new output folder
         """
         self.volume_already_evaluated = False
         super().initialise()
         self.true_host   = true_host
         self.R_S         = []
         self.ac          = []
         self.areas_N     = {cr:[] for cr in self.levels}
@@ -299,15 +299,15 @@
         
     def load_glade(self, glade_file):
         """
         Load GLADE+ from hdf5 file.
         This is tailored to the GLADE+ hdf5 file created by the create_glade.py pipeline.
         
         Arguments:
-            :str or Path glade_file: glade file to be uploaded
+            str or Path glade_file: glade file to be uploaded
         """
         self.glade_header =  ' '.join(['ra', 'dec', 'z', 'm_B', 'm_K', 'm_W1', 'm_bJ', 'logp'])
         with h5py.File(glade_file, 'r') as f:
             ra  = np.array(f['ra'])
             dec = np.array(f['dec'])
             z   = np.array(f['z'])
             B   = np.array(f['m_B'])
@@ -352,47 +352,47 @@
 
     def _pdf_probit(self, x):
         """
         Evaluate mixture at point(s) x in probit space.
         Overwrites parent method to avoid memory issues in 3D grid or catalog evaluation
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.pdf(x)
+            np.ndarray: mixture.pdf(x)
         """
         p = np.zeros(len(x))
         for comp, wi in zip(self.mixture, self.w):
             p += wi*mn(comp.mu, comp.sigma).pdf(x)
         return p
     
     def _logpdf_probit(self, x):
         """
         Evaluate log mixture at point(s) x in probit space.
         Overwrites parent method to avoid memory issues in 3D grid or catalog evaluation
         
         Arguments:
-            :np.ndarray x: point(s) to evaluate the mixture at (in probit space)
+            np.ndarray x: point(s) to evaluate the mixture at (in probit space)
         
         Returns:
-            :np.ndarray: mixture.logpdf(x)
+            np.ndarray: mixture.logpdf(x)
         """
         p = -np.ones(len(x))*np.inf
         for comp, wi in zip(self.mixture, self.log_w):
             p = log_add_array(p, wi + mn(comp.mu, comp.sigma).logpdf(x))
         return p
 
     def add_new_point(self, x):
         """
         Update the probability density reconstruction adding a new sample
         Sample must be in celestial coordinate and in the following order: [ra, dec, dist].
         
         Arguments:
-            :np.ndarray x: sample
+            np.ndarray x: sample
         """
         self.volume_already_evaluated = False
         cart_x = celestial_to_cartesian(x)
         super().add_new_point(cart_x)
         if self.flag_skymap and self.n_pts == self.next_plot:
             self.N.append(self.next_plot)
             self.next_plot = 2*self.next_plot
@@ -400,29 +400,29 @@
             self.make_volume_map(n_gals = self.n_gal_to_plot)
     
     def sample_from_volume(self, n_samps):
         """
         Draw samples from volume
         
         Arguments:
-            :int n_samps: number of samples to draw
+            int n_samps: number of samples to draw
         
         Returns:
-            :np.ndarray: samples in celestial coordinates (ra, dec, D)
+            np.ndarray: samples in celestial coordinates (ra, dec, D)
         """
         samples = self.rvs(n_samps)
         return cartesian_to_celestial(samples)
     
     def plot_samples(self, n_samps, initial_samples = None):
         """
         Plot samples from DPGMM reconstruction along with PE samples (if available)
         
         Arguments:
-            :int n_samps:                number of samples to draw
-            :np.ndarray initial_samples: PE samples
+            int n_samps:                number of samples to draw
+            np.ndarray initial_samples: PE samples
         """
         mix_samples = self.sample_from_volume(n_samps)
         if initial_samples is not None:
             if self.true_host is not None:
                 c = corner(initial_samples, color = 'coral', labels = self.labels, truths = self.true_host, hist_kwargs={'density':True, 'label':'$\mathrm{Samples}$'})
             else:
                 c = corner(initial_samples, color = 'coral', labels = self.labels, hist_kwargs={'density':True, 'label':'$\mathrm{Samples}$'})
@@ -506,15 +506,15 @@
     
     def evaluate_catalog(self, final_map = False):
         """
         Evaluate the probability of being the host for each entry in the galaxy catalog and rank it accordingly.
         If the inference is finished, save credible areas/volumes.
         
         Arguments:
-            :bool final_map: flag to raise if the inference is finished
+            bool final_map: flag to raise if the inference is finished
         """
         log_p_cat                  = self._logpdf_probit(self.probit_catalog) + self.log_inv_J_cat - self.log_norm_p_vol
         self.log_p_cat_to_plot     = log_p_cat[np.where(log_p_cat > self.volume_heights[np.where(self.levels == self.region)])]
         self.p_cat_to_plot         = np.exp(self.log_p_cat_to_plot)
         self.cat_to_plot_celestial = self.catalog[np.where(log_p_cat > self.volume_heights[np.where(self.levels == self.region)])]
         self.cat_to_plot_cartesian = self.cartesian_catalog[np.where(log_p_cat > self.volume_heights[np.where(self.levels == self.region)])]
         
@@ -526,15 +526,15 @@
             np.savetxt(Path(self.catalog_folder, 'CR_'+self.name+'.txt'), np.array([self.areas[np.where(self.levels == self.region)], self.volumes[np.where(self.levels == self.region)]]).T, header = 'area volume')
     
     def make_skymap(self, final_map = False):
         """
         Produce skymap.
         
         Arguments:
-            :bool final_map: flag to raise if the inference is finished
+            bool final_map: flag to raise if the inference is finished
         """
         self.evaluate_skymap()
         fig = plt.figure()
         ax = fig.add_subplot(111)
         c = ax.contourf(self.ra_2d, self.dec_2d, self.p_skymap.T, 500, cmap = 'Reds')
         ax.set_rasterization_zorder(-10)
         c1 = ax.contour(self.ra_2d, self.dec_2d, self.log_p_skymap.T, np.sort(self.skymap_heights), colors = 'black', linewidths = 0.5, linestyles = 'dashed')
@@ -561,16 +561,16 @@
         plt.close()
     
     def make_volume_map(self, final_map = False, n_gals = 100):
         """
         Produce volume map as 3D and 2D scatter plot of galaxies, if a catalog is provided.
         
         Arguments:
-            :bool final_map: flag to raise if the inference is finished
-            :int n_gals:     number of galaxies to plot
+            bool final_map: flag to raise if the inference is finished
+            int n_gals:     number of galaxies to plot
         """
         self.evaluate_volume_map()
         if self.catalog is None:
             return
             
         self.evaluate_catalog(final_map)
         
@@ -761,15 +761,15 @@
         
     def density_from_samples(self, samples):
         """
         Reconstruct the probability density from a set of samples.
         Samples must be in celestial coordinate and in the following order: [ra, dec, dist].
         
         Arguments:
-            :iterable samples: set of volume samples
+            iterable samples: set of volume samples
         """
         np.random.shuffle(samples)
         # Checking the posteriors are properly ordered:
         check_ra   = np.logical_and(samples[:,0] > 0, samples[:,0] < 2*np.pi).all()
         check_dec  = np.logical_and(samples[:,1] > -np.pi/2., samples[:,1] < np.pi/2.).all()
         check_dist = np.logical_and(samples[:,2] > 0, samples[:,2] < self.max_dist).all()
         if not (check_ra and check_dec and check_dist):
```

### Comparing `figaro-1.1.1/figaro/transform.py` & `figaro-1.1.2/figaro/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     cdf_normal is the cumulative distribution function of the unit normal distribution.
     WARNING: returns NAN if x is not in [xmin, xmax].
     
     t(x) = cdf^-1_normal((x-x_min)/(x_max - x_min))
 
     
     Arguments:
-        :np.ndarray x:      sample(s) to transform (2d array)
-        :np.ndarray bounds: limits for each dimension (2d array, [[xmin, xmax], [ymin, ymax]...])
+        np.ndarray x:      sample(s) to transform (2d array)
+        np.ndarray bounds: limits for each dimension (2d array, [[xmin, xmax], [ymin, ymax]...])
         
     Returns:
-        :np.ndarray: sample(s)
+        np.ndarray: sample(s)
     '''
     dbounds = bounds[:,1]-bounds[:,0]
     sigma   = dbounds*0.34
     cdf = (x - bounds[:,0])/dbounds
     o = np.sqrt(2.0)*erfinv(2*cdf-1)*sigma
     return o
 
@@ -34,19 +34,19 @@
     '''
     Coordinate change from probit to natural space.
     cdf_normal is the cumulative distribution function of the unit normal distribution.
     
     x(t) = xmin + (xmax-xmin)*cdf_normal(t|0,1)
     
     Arguments:
-        :np.ndarray x:      sample(s) to antitransform (2d array)
-        :np.ndarray bounds: limits for each dimension (2d array, [[xmin, xmax], [ymin, ymax]...])
+        np.ndarray x:      sample(s) to antitransform (2d array)
+        np.ndarray bounds: limits for each dimension (2d array, [[xmin, xmax], [ymin, ymax]...])
         
     Returns:
-        :np.ndarray: sample(s)
+        np.ndarray: sample(s)
     '''
     dbounds = bounds[:,1]-bounds[:,0]
     sigma   = dbounds*0.34
     cdf = 0.5*(1.0+erf(x/(np.sqrt(2.0)*sigma)))
     o = bounds[:,0]+dbounds*cdf
     return o
```

### Comparing `figaro-1.1.1/figaro/utils.py` & `figaro-1.1.2/figaro/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 #-----------#
 
 def recursive_grid(bounds, n_pts, get_1d = False):
     """
     Recursively generates the n-dimensional grid points (extremes are excluded).
     
     Arguments:
-        :list-of-lists bounds: extremes for each dimension (excluded)
-        :int n_pts:            number of points for each dimension
-        :bool get_1d:          return list of 1d-arrays (one per dimension)
+        list-of-lists bounds: extremes for each dimension (excluded)
+        int n_pts:            number of points for each dimension
+        bool get_1d:          return list of 1d-arrays (one per dimension)
         
     Returns:
-        :np.ndarray: grid
-        :np.ndarray: differential for each grid
-        :np.ndarray: list of 1d-arrays (one per dimension)
+        np.ndarray: grid
+        np.ndarray: differential for each grid
+        np.ndarray: list of 1d-arrays (one per dimension)
     """
     bounds = np.atleast_2d(bounds)
     n_pts  = np.atleast_1d(n_pts)
     if len(bounds) == 1:
         d  = np.linspace(bounds[0,0], bounds[0,1], n_pts[0])
         dD = d[1]-d[0]
         if get_1d:
@@ -55,21 +55,21 @@
         return np.array(grid), diff
 
 def rejection_sampler(n_draws, f, bounds, selfunc = None):
     """
     1D rejection sampler, allows for a selection function
     
     Arguments:
-        :int n_draws:      number of draws
-        :callable f:       probability density to sample from
-        :iterable bounds:  upper and lower bound
-        :callable selfunc: selection function, must support numpy arrays
+        int n_draws:      number of draws
+        callable f:       probability density to sample from
+        iterable bounds:  upper and lower bound
+        callable selfunc: selection function, must support numpy arrays
     
     Returns:
-        :np.ndarray: samples
+        np.ndarray: samples
     """
     n_draws = int(n_draws)
     if selfunc is None:
         selfunc = lambda x: 1
     x   = np.linspace(bounds[0], bounds[1], 1000)
     top = np.max(f(x)*selfunc(x))
     samples = []
@@ -81,39 +81,39 @@
     return np.array(samples).flatten()[:n_draws]
 
 def get_priors(bounds, samples = None, mean = None, std = None, cov = None, df = None, k = None, a = None, scale = None, probit = True, hierarchical = False):
     """
     This method takes the prior parameters for the Normal-Inverse-Wishart distribution in the natural space and returns them as parameters in the probit space, ordered as required by FIGARO. In the following, D will denote the dimensionality of the inferred distribution.
 
     Four parameters are returned:
-    * df, is the number of degrees of freedom for the Inverse Wishart distribution,. It must be greater than D+1. If this parameter is None or does not satisfy the condition df > D+1, the default value D+2 is used;
-    * k is the scale parameter for the multivariate Normal distribution. Suggested values are  k <~ 1e-1. If None, the default value 1e-2 is used.
-    * mu is the mean of the multivariate Normal distribution. It can be either estimated from the available samples or passed directly as a 1D array with length D (the keyword argument mean overrides the samples). If None, the default value 0 (corresponding to the parameter space center) is used.
-    * L is the expected value for the Inverse Wishart distribution. This parameter can be either (in descending priority order):
-        * passed as 2D array with shape (D,D), the covariance matrix - keyword cov;
-        * passed as 1D array with shape (D,) or double: vector of standard deviations (if double, it assumes that the same std has to be used for all dimensions) - keyword std;
-        * estimated from samples - keyword samples.
+        * df, is the number of degrees of freedom for the Inverse Wishart distribution,. It must be greater than D+1. If this parameter is None or does not satisfy the condition df > D+1, the default value D+2 is used;
+        * k is the scale parameter for the multivariate Normal distribution. Suggested values are  k <~ 1e-1. If None, the default value 1e-2 is used.
+        * mu is the mean of the multivariate Normal distribution. It can be either estimated from the available samples or passed directly as a 1D array with length D (the keyword argument mean overrides the samples). If None, the default value 0 (corresponding to the parameter space center) is used.
+        * L is the expected value for the Inverse Wishart distribution. This parameter can be either (in descending priority order):
+            * passed as 2D array with shape (D,D), the covariance matrix - keyword cov;
+            * passed as 1D array with shape (D,) or double: vector of standard deviations (if double, it assumes that the same std has to be used for all dimensions) - keyword std;
+            * estimated from samples - keyword samples.
        
     The order in which they are returned is (k,L,df,mu).
     
     Arguments:
-        :np.ndarray bounds:              boundaries for probit transformation
-        :np.ndarray samples:             2D [DPGMM] or 3D [(H)DPGMM] array with samples
-        :double or np.ndarray mean:      mean [DPGMM]
-        :double or np.ndarray std:       expected standard deviation (if double, the same std is used for all dimensions, if np.ndarray must match the number of dimensions) [DPGMM and (H)DPGMM]
-        :np.ndarray cov:                 covariance matrix [DPGMM]
-        :int df:                         degrees of freedom for Inverse Wishart distribution [DPGMM]
-        :double k:                       scale parameter for Normal distribution [DPGMM]
-        :double a:                       shape parameter for the Inverse Gamma distribution [(H)DPGMM]
-        :double scale:                   fraction of samples std [DPGMM]
-        :bool probit:                    whether the probit transformation will be applied or not
-        :bool hierarchical:              returns the prior pars for (H)DPGMM rather than for DPGMM
+        np.ndarray bounds:              boundaries for probit transformation
+        np.ndarray samples:             2D [DPGMM] or 3D [(H)DPGMM] array with samples
+        double or np.ndarray mean:      mean [DPGMM]
+        double or np.ndarray std:       expected standard deviation (if double, the same std is used for all dimensions, if np.ndarray must match the number of dimensions) [DPGMM and (H)DPGMM]
+        np.ndarray cov:                 covariance matrix [DPGMM]
+        int df:                         degrees of freedom for Inverse Wishart distribution [DPGMM]
+        double k:                       scale parameter for Normal distribution [DPGMM]
+        double a:                       shape parameter for the Inverse Gamma distribution [(H)DPGMM]
+        double scale:                   fraction of samples std [DPGMM]
+        bool probit:                    whether the probit transformation will be applied or not
+        bool hierarchical:              returns the prior pars for (H)DPGMM rather than for DPGMM
         
     Returns:
-        :tuple: prior parameters ordered as in (H)/DPGMM
+        tuple: prior parameters ordered as in (H)/DPGMM
     """
     bounds = np.atleast_2d(bounds)
     dim = len(bounds)
     if scale is None:
         scale = 5.
     if samples is not None:
         if not np.iterable(samples[0]):
@@ -219,19 +219,19 @@
         return (k_out, L_out, df_out, mu_out)
 
 def rvs_median(draws, size = 1):
     """
     Generates samples from median distribution of a set of draws.
     
     Arguments:
-        :iterable draws: container for mixture instances
-        :int size:    number of samples
+        iterable draws: container for mixture instances
+        int size:    number of samples
     
     Returns:
-        :np.ndarray: samples
+        np.ndarray: samples
     """
     idx = np.random.choice(np.arange(len(draws)), size = int(size))
     ctr = Counter(idx)
     samples = np.empty(shape = (1, draws[0].dim))
     for i, n in zip(ctr.keys(), ctr.values()):
         samples = np.concatenate((samples, draws[i].rvs(n)))
     return samples[1:]
@@ -240,23 +240,23 @@
     """
     Builds mixtures composed of a single Gaussian distribution.
     WARNING: due to the probit coordinate change, a Gaussian distribution in the natural space does not correspond to a Gaussian distribution in the probit space.
     The resulting distributions, therefore, are just an approximation. This approximation holds for distributions which are far from boundaries.
     In general, a more robust (but slower) approach would be to draw samples from each original Gaussian distribution and to use them to make a hierarchical inference.
     
     Arguments:
-        :np.ndarray mu:     mean for each Gaussian distribution
-        :np.ndarray cov:    covariance matrix for each Gaussian distribution
-        :np.ndarray bounds: boundaries for probit transformation
-        :str out_folder:    output folder
-        :bool save:         whether to save the draws or not
-        :int n_samps:       number of samples to estimate mean and covariance in probit space
+        np.ndarray mu:     mean for each Gaussian distribution
+        np.ndarray cov:    covariance matrix for each Gaussian distribution
+        np.ndarray bounds: boundaries for probit transformation
+        str out_folder:    output folder
+        bool save:         whether to save the draws or not
+        int n_samps:       number of samples to estimate mean and covariance in probit space
     
     Returns:
-        :np.ndarray: mixtures
+        np.ndarray: mixtures
     """
     # Here to avoid circular import
     from figaro.mixture import mixture
     bounds = np.atleast_2d(bounds)
     
     out_folder = Path(out_folder)
     if not out_folder.exists():
@@ -312,16 +312,16 @@
 #-------------#
 
 def save_options(options, out_folder, name = None):
     """
     Saves options for the run (reproducibility)
     
     Arguments:
-        :obj options:            options
-        :str or Path out_folder: folder where to save the option file
+        obj options:            options
+        str or Path out_folder: folder where to save the option file
     """
     if name is None:
         filename = 'options_log.ini'
     else:
         filename = 'options_log_{0}.ini'.format(name)
     with open(Path(out_folder, filename), 'w') as logfile:
         logfile.write('[OPTIONS]\n')
@@ -329,19 +329,19 @@
             logfile.write('{0} = {1}\n'.format(key,val))
 
 def load_options(opts, file):
     """
     Loads options for the run (reproducibility)
     
     Arguments:
-        :obj opts:         options object
-        :str or Path file: file with options
+        obj opts:         options object
+        str or Path file: file with options
     
     Returns:
-        :obj: options
+        obj: options
     """
     with open(file, 'r') as logfile:
         config = configparser.RawConfigParser()
         config.read(file)
         opts_dict = dict(config.items('OPTIONS'))
     for key in opts_dict.keys():
         if opts_dict[key] in ['True', 'False']:
```

### Comparing `figaro-1.1.1/figaro.egg-info/PKG-INFO` & `figaro-1.1.2/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.1.1
+Version: 1.1.2
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Home-page: https://github.com/sterinaldi/figaro
 Author: Stefano Rinaldi, Walter Del Pozzo, Daniele Sanfratello
 Author-email: stefano.rinaldi@phd.unipi.it, walter.delpozzo@unipi.it, d.sanfratello@studenti.unipi.it
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

