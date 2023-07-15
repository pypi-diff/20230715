# Comparing `tmp/jaxip-0.7.0.tar.gz` & `tmp/jaxip-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.7.0.tar", last modified: Mon Jul 10 18:19:33 2023, max compression
+gzip compressed data, was "jaxip-0.7.1.tar", last modified: Sat Jul 15 14:24:53 2023, max compression
```

## Comparing `jaxip-0.7.0.tar` & `jaxip-0.7.1.tar`

### file list

```diff
@@ -1,149 +1,148 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.939054 jaxip-0.7.0/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.7.0/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      801 2023-07-10 18:19:00.000000 jaxip-0.7.0/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.7.0/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.7.0/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5649 2023-07-10 18:19:33.939054 jaxip-0.7.0/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5062 2023-07-10 18:19:00.000000 jaxip-0.7.0/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.863057 jaxip-0.7.0/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.7.0/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.863057 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.847057 jaxip-0.7.0/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.867056 jaxip-0.7.0/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-10 18:10:15.000000 jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.867056 jaxip-0.7.0/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.0/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.7.0/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6412 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.7.0/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       77 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.7.0/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.871056 jaxip-0.7.0/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.7.0/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.7.0/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.7.0/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.7.0/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      662 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-05-17 19:30:18.000000 jaxip-0.7.0/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-07-10 18:10:04.000000 jaxip-0.7.0/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      951 2023-07-10 18:19:00.000000 jaxip-0.7.0/docs/jaxip.simulation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-05-10 20:36:05.000000 jaxip-0.7.0/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.7.0/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-07-10 18:10:04.000000 jaxip-0.7.0/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.7.0/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.7.0/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.7.0/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.875056 jaxip-0.7.0/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.7.0/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.891055 jaxip-0.7.0/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      232 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1486 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3683 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3354 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    17756 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.891055 jaxip-0.7.0/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      154 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6451 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/datasets/runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      929 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/datasets/transformer.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.895055 jaxip-0.7.0/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.899055 jaxip-0.7.0/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.7.0/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5312 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7828 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7467 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.899055 jaxip-0.7.0/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.903055 jaxip-0.7.0/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.7.0/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2902 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.907055 jaxip-0.7.0/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1979 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1844 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.919055 jaxip-0.7.0/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.7.0/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9217 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9374 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.7.0/jaxip/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    19007 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11345 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3627 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/pytree.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.919055 jaxip-0.7.0/jaxip/simulation/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.7.0/jaxip/simulation/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2143 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/lj.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4331 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     8523 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2515 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/run.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/simulation/thermostat.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      766 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/types.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.7.0/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.923055 jaxip-0.7.0/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1418 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2012 2023-07-10 18:19:00.000000 jaxip-0.7.0/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.7.0/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.7.0/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.887056 jaxip-0.7.0/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5649 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3295 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-07-10 18:19:33.000000 jaxip-0.7.0/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-07-10 18:19:33.939054 jaxip-0.7.0/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.7.0/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.927054 jaxip-0.7.0/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-10 18:19:33.935054 jaxip-0.7.0/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.7.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.7.0/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.0/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.7.0/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5108 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2569 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3137 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4106 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3445 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4825 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2850 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5897 2023-07-10 18:19:00.000000 jaxip-0.7.0/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-07-10 18:04:56.000000 jaxip-0.7.0/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.847498 jaxip-0.7.1/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.7.1/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.7.1/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      829 2023-07-15 14:24:44.000000 jaxip-0.7.1/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.7.1/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.7.1/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5671 2023-07-15 14:24:53.847498 jaxip-0.7.1/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5084 2023-07-15 14:24:44.000000 jaxip-0.7.1/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.775498 jaxip-0.7.1/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.7.1/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.747497 jaxip-0.7.1/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.743497 jaxip-0.7.1/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.779498 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.747497 jaxip-0.7.1/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.7.1/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6459 2023-07-15 14:24:44.000000 jaxip-0.7.1/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.7.1/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       77 2023-07-10 18:19:00.000000 jaxip-0.7.1/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.7.1/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.7.1/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.7.1/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.7.1/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.7.1/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-07-15 14:16:29.000000 jaxip-0.7.1/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      495 2023-07-15 14:24:44.000000 jaxip-0.7.1/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-07-15 14:16:29.000000 jaxip-0.7.1/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      951 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.7.1/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.7.1/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.7.1/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.7.1/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.787498 jaxip-0.7.1/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.7.1/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.799498 jaxip-0.7.1/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      232 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1486 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3683 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3354 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17758 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.803498 jaxip-0.7.1/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       84 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6494 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/datasets/runner.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.807498 jaxip-0.7.1/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.815498 jaxip-0.7.1/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.7.1/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5312 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7828 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7467 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.815498 jaxip-0.7.1/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.819498 jaxip-0.7.1/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2879 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.823498 jaxip-0.7.1/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1979 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1844 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.827498 jaxip-0.7.1/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9522 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9374 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.7.1/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19007 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11345 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3627 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.831498 jaxip-0.7.1/jaxip/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.7.1/jaxip/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2143 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/lj.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4331 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9132 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2515 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/run.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      766 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.7.1/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.835498 jaxip-0.7.1/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1418 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2012 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.7.1/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.791498 jaxip-0.7.1/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5671 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3265 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-15 14:24:23.000000 jaxip-0.7.1/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-07-15 14:24:53.847498 jaxip-0.7.1/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.7.1/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.843498 jaxip-0.7.1/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.847498 jaxip-0.7.1/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.7.1/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.1/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.7.1/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5108 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2569 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3137 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4106 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3445 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5269 2023-07-15 14:24:44.000000 jaxip-0.7.1/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2850 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5897 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/weights.008.pkl
```

### Comparing `jaxip-0.7.0/CONTRIBUTING.rst` & `jaxip-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/HISTORY.rst` & `jaxip-0.7.1/HISTORY.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 =======
 History
 =======
 
 0.7.x (2023-07-10)
 -------------------
 * Refactored structure including design, documentation, and performance (JIT kernels)
+* Refactored RuNNer dataset
 
 0.6.x (2023-06-18)
 -------------------
 * Implemented Molecular dynamics (MD) and Monte-Carlo (MC) simulators
 
 0.5.x (2023-03-02)
 -------------------
```

### Comparing `jaxip-0.7.0/LICENSE` & `jaxip-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/PKG-INFO` & `jaxip-0.7.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.7.0
+Version: 0.7.1
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -37,30 +37,30 @@
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
 development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, material science. 
+for use in computational physics, chemistry, and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
-* It uses `autograd` to make defining new descriptors straightforward.
+* It uses `automatic differentiation` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional 
         neural network potential (HDNNP) proposed by Behler et al. 
         (`2007 <https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.146401>`_).
@@ -149,15 +149,15 @@
         # Or loading from files
         #nnp.load()
 
         # Total energy
         nnp(structure)
 
         # Force components
-        nnp.compute_force(structure)
+        nnp.compute_forces(structure)
 
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
```

### Comparing `jaxip-0.7.0/README.rst` & `jaxip-0.7.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
 development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, material science. 
+for use in computational physics, chemistry, and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
-* It uses `autograd` to make defining new descriptors straightforward.
+* It uses `automatic differentiation` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional 
         neural network potential (HDNNP) proposed by Behler et al. 
         (`2007 <https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.146401>`_).
@@ -131,15 +131,15 @@
         # Or loading from files
         #nnp.load()
 
         # Total energy
         nnp(structure)
 
         # Force components
-        nnp.compute_force(structure)
+        nnp.compute_forces(structure)
 
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
```

### Comparing `jaxip-0.7.0/docs/Makefile` & `jaxip-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png` & `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png` & `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png` & `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_38_0.png` & `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_45_0.png` & `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/_build/html/_images/notebooks_getting_started_51_0.png` & `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/conf.py` & `jaxip-0.7.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 extensions = extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
     "sphinx.ext.todo",
     "sphinx.ext.mathjax",
     "sphinx_autodoc_typehints",
-    "sphinxcontrib.autodoc_pydantic",
+    # "sphinxcontrib.autodoc_pydantic",
     "nbsphinx",
     # "sphinx_gallery.load_style",
     # "nbsphinx_link",
     # "IPython.sphinxext.ipython_console_highlighting",
 ]
 
 
@@ -97,15 +97,15 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "English"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
@@ -217,12 +217,15 @@
 
 curdir = os.path.dirname(os.path.abspath(__file__))
 notebooks_dir = os.path.join(curdir, "notebooks")
 if os.path.exists(notebooks_dir):
     shutil.rmtree(notebooks_dir)
 os.makedirs(notebooks_dir, exist_ok=True)
 
-for filename in ("getting_started.ipynb", "training.ipynb"):
+for filename in (
+    "getting_started.ipynb",
+    "training_potential.ipynb",
+):
     shutil.copyfile(  # copytree(
         os.path.join(curdir, "..", "examples", filename),
         os.path.join(curdir, "notebooks", filename),
     )
```

### Comparing `jaxip-0.7.0/docs/images/flowchart.drawio.png` & `jaxip-0.7.1/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/images/water.png` & `jaxip-0.7.1/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/installation.rst` & `jaxip-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.atoms.rst` & `jaxip-0.7.1/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.datasets.rst` & `jaxip-0.7.1/docs/jaxip.utils.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,53 @@
-jaxip.datasets package
-======================
+jaxip.utils package
+===================
 
 Submodules
 ----------
 
-jaxip.datasets.dataset module
------------------------------
+jaxip.utils.attribute module
+----------------------------
 
-.. automodule:: jaxip.datasets.dataset
+.. automodule:: jaxip.utils.attribute
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.datasets.runner module
-----------------------------
+jaxip.utils.batch module
+------------------------
+
+.. automodule:: jaxip.utils.batch
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.utils.compare module
+--------------------------
+
+.. automodule:: jaxip.utils.compare
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+jaxip.utils.profiler module
+---------------------------
 
-.. automodule:: jaxip.datasets.runner
+.. automodule:: jaxip.utils.profiler
    :members:
    :undoc-members:
    :show-inheritance:
 
-jaxip.datasets.transformer module
----------------------------------
+jaxip.utils.tokenize module
+---------------------------
 
-.. automodule:: jaxip.datasets.transformer
+.. automodule:: jaxip.utils.tokenize
    :members:
    :undoc-members:
    :show-inheritance:
 
 Module contents
 ---------------
 
-.. automodule:: jaxip.datasets
+.. automodule:: jaxip.utils
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `jaxip-0.7.0/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.7.1/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.descriptors.rst` & `jaxip-0.7.1/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.models.nn.rst` & `jaxip-0.7.1/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.potentials.nnp.rst` & `jaxip-0.7.1/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.rst` & `jaxip-0.7.1/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/jaxip.simulation.rst` & `jaxip-0.7.1/docs/jaxip.simulation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/make.bat` & `jaxip-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/theory.rst` & `jaxip-0.7.1/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/docs/usage.rst` & `jaxip-0.7.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/__init__.py` & `jaxip-0.7.1/jaxip/__init__.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/atoms/_structure.py` & `jaxip-0.7.1/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/atoms/box.py` & `jaxip-0.7.1/jaxip/atoms/box.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/atoms/element.py` & `jaxip-0.7.1/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/atoms/neighbor.py` & `jaxip-0.7.1/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/atoms/structure.py` & `jaxip-0.7.1/jaxip/atoms/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,15 @@
             energy_offset = energy_offset.at[self.select(element)].set(
                 atom_energy[element]
             )
         return energy_offset
 
     def remove_energy_offset(self, atom_energy: Dict[Element, float]) -> None:
         """
-        Remove the input reference energies to individual atoms and the total energy.
+        Remove the input reference energies from individual atoms and the total energy.
 
         :param atom_energy: atom reference energy
         :type atom_energy: Dict[Element, float]]
         """
         energy_offset: Array = self._get_energy_offset(atom_energy)
         self.energies -= energy_offset
         self.total_energy -= energy_offset.sum()
```

### Comparing `jaxip-0.7.0/jaxip/config.py` & `jaxip-0.7.1/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/datasets/runner.py` & `jaxip-0.7.1/jaxip/datasets/runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,127 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from pathlib import Path
-from typing import DefaultDict, Dict, List, Optional, TextIO
+from typing import Dict, Iterator, List, Optional, TextIO
 
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.dataset import DatasetInterface
-from jaxip.datasets.transformer import ToStructure, TransformerInterface
 from jaxip.logger import logger
+from jaxip.types import Dtype, _dtype
 from jaxip.utils.tokenize import tokenize
 
 
 class RunnerDataset(DatasetInterface):
     """
-    Dataset for `RuNNer`_ data file format.
 
-    The input structure file contains atom info and simulation box.
-    Each snapshot contains two per-atom and collective properties as follows:
+    The dataset used for the input data format of `RuNNer`_ consists of atomic attributes
+    and simulation box information. Within each snapshot, there are two types of
+    properties: `per-atom` properties and `collective` properties.
 
-    * `per-atom` properties include the element name, positions, energy, charge, force components, etc.
-    * `collective` properties such as lattice, total energy, and total charge.
+    The per-atom properties encompass various attributes like the element name,
+    positions, energy, charge, force components, and more.
+
+    On the other hand, the collective properties include attributes
+    such as lattice parameters, total energy, and total charge.
 
     .. _RuNNer: https://www.uni-goettingen.de/de/560580.html
     """
 
     def __init__(
         self,
         filename: Path,
         persist: bool = False,
-        transform: Optional[TransformerInterface] = None,
+        dtype: Optional[Dtype] = None,
     ) -> None:
         """
-        Initialize the `RuNNer`_ structure dataset.
+        Create a `RuNNer`_ structure dataset by initializing it from an input file.
 
-        :param filename: Path
-        :type filename: path to the RuNNer structure file
-        :param persist: Persist structure data in the memory, defaults to False
+        :param filename: input file name
+        :type filename: Path
+        :param persist: Persist any loaded structure data in the memory, defaults to False
         :type persist: bool, optional
-        :param transform: applied transformation on raw data, default is ToStructure.
+        :param dtype: floating point precision for the structure data, defaults to None
+        :type dtype: Optional[Dtype], optional
 
         .. _RuNNer: https://www.uni-goettingen.de/de/560580.html
         """
         self.filename: Path = Path(filename)
         self.persist: bool = persist
-        self.transform: TransformerInterface = (
-            ToStructure() if transform is None else transform
-        )
-        self._cached_structures: Dict[int, Structure] = dict()
-        self._current_index: int = 0
+        self._cache: Dict[int, Structure] = dict()
+        self.dtype = dtype if dtype is not None else _dtype.FLOATX
 
     def __len__(self) -> int:
-        """Return number of structures."""
+        """Return number of available structures."""
         num_structures: int = 0
         with open(str(self.filename), "r") as file:
-            while self._ignore_next_structure(file):
+            while self._ignore_next(file):
                 num_structures += 1
         return num_structures
 
     def __getitem__(self, index: int) -> Structure:
         """
-        Return i-th structure data.
+        Return i-th structure.
 
         This is a lazy call which means that only required section
-        of data is loaded from the file into the memory.
+        of data is loaded into the memory.
         """
         return self._read_from_cache(index)
 
-    def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__name__}"
-            f"(filename='{str(self.filename)}', transform={self.transform})"
-        )
-
-    # ----------------------------------------------
-
-    def _read_next_structure(self, file: TextIO) -> Dict[str, List]:
+    def read_sequential(self) -> Iterator[Structure]:
         """
-        Read the next structure from the input file.
+        Read structures sequentially.
+
+        It must be noted that reading data in a consecutive manner is
+        faster compared to random indexing read.
 
-        :param file: input structure file handler
-        :type file: TextIO
-        :return: a sample of thr dataset
-        :rtype: Dict
+        :return: Structure
+        :rtype: Iterator[Structure]
         """
-        data: DefaultDict = defaultdict(list)
+        logger.debug("Read structures sequentially")
+        index: int = 0
+        with open(str(self.filename), "r") as file:
+            while True:
+                data = self._read_next(file)
+                if not data:
+                    break
+                structure = self._to_structure(data)
+                if self.persist:
+                    if index in self._cache:
+                        yield self._cache[index]
+                    else:
+                        self._cache[index] = structure
+                yield structure
+                index += 1
+
+    def preload(self) -> None:
+        """
+        Preload (cache) all structures into memory.
+
+        This ensures that any structure can be rapidly loaded from memory in subsequent operations.
+        """
+        self.persist = True
+        for _ in self.read_sequential():
+            pass
+
+    @classmethod
+    def _read_next(cls, file: TextIO) -> Dict[str, List]:
+        """Read next structure data between `begin` and `end` keywords."""
+        data = defaultdict(list)
+        read_block: bool = False
         while True:
-            line: str = file.readline()
+            line = file.readline()
+            if not line:
+                break
+            keyword, _ = tokenize(line)
+            if keyword == "begin":
+                read_block = True
+                break
+        while read_block:
+            line = file.readline()
             if not line:
                 break
             keyword, tokens = tokenize(line)
             if keyword == "atom":
                 data["positions"].append([float(t) for t in tokens[:3]])
                 data["elements"].append(tokens[3])
                 data["charges"].append(float(tokens[4]))
@@ -100,91 +132,53 @@
             elif keyword == "energy":
                 data["total_energy"].append(float(tokens[0]))
             elif keyword == "charge":
                 data["total_charge"].append(float(tokens[0]))
             elif keyword == "comment":
                 data["comment"].append(" ".join(line.split()[1:]))
             elif keyword == "end":
-                break
+                read_block = False
         return data
 
-    def _ignore_next_structure(self, file: TextIO) -> bool:
-        """
-        Ignore the next structure.
-
-        :param file: input structure file handler
-        :type file: TextIO
-        :return: whether the ignoring of next structure was successful or not
-        :rtype: bool
-        """
+    @classmethod
+    def _ignore_next(cls, file: TextIO) -> bool:
         while True:
             line = file.readline()
             if not line:
                 return False
-            keyword, tokens = tokenize(line)
+            keyword, _ = tokenize(line)
             if keyword == "end":
                 break
         return True
 
-    def _read_structure(self, index: int) -> Structure:
-        """
-        Read the i-th structure from the input file.
-
-        :param index: index for structures
-        :type index: int
-        :return: Structure
-        :rtype: Any
-        """
-        logger.debug(f"Reading structure[{index}]")
+    def _read(self, index: int) -> Structure:
+        logger.debug(f"load structure({index=})")
         with open(str(self.filename), "r") as file:
             for _ in range(index):
-                self._ignore_next_structure(file)
-            sample = self._read_next_structure(file)
-            if not sample:
-                raise IndexError(f"index {index} is out of bound with size {len(self)}")
-        return self.transform(sample)
+                self._ignore_next(file)
+            data = self._read_next(file)
+            if not data:
+                raise IndexError(
+                    f"The given index {index} is out of bound (len={len(self)})"
+                )
+        return self._to_structure(data)
 
-    def _read_from_cache(self, index: int) -> Structure:
-        """
-        Read from the cached structures if the `persist` input flag is enabled.
+    def _to_structure(self, data: Dict[str, List]) -> Structure:
+        return Structure.from_dict(data, dtype=self.dtype)
 
-        :param index: index for structures
-        :type index: int
-        :return: Structure
-        :rtype: Any
-        """
+    def _read_from_cache(self, index: int) -> Structure:
+        """Read the desired structure from cache, if possible."""
         if not self.persist:
-            return self._read_structure(index)
-
-        sample: Structure
-        if index not in self._cached_structures:
-            sample = self._read_structure(index)
-            self._cached_structures[index] = sample
+            return self._read(index)
+        if index not in self._cache:
+            structure = self._read(index)
+            self._cache[index] = structure
+            return structure
         else:
-            sample = self._cached_structures[index]
-
-        return sample
+            return self._cache[index]
 
-    # ----------------------------------------------
-
-    def __next__(self) -> Structure:
-        """
-        Iterate directly over the dataset.
-
-        .. warning::
-            Due to its slow performance, lack of shuffling, and no parallel loading,
-            it is recommended to be only used for testing.
-
-        :raises StopIteration: stop iteration
-        :return: Return next structure
-        :rtype: Transformed structure
-        """
-        try:
-            sample: Structure = self.__getitem__(self._current_index)
-            self._current_index += 1
-            return sample
-        except IndexError:
-            self._current_index = 0
-            raise StopIteration
-
-    def __iter__(self) -> RunnerDataset:
-        return self
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}"
+            f"(filename='{str(self.filename)}'"
+            f", persist={self.persist}, dtype={self.dtype.dtype})"
+        )
```

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/angular.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/cutoff.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/cutoff.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/radial.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.7.1/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/descriptor.py` & `jaxip-0.7.1/jaxip/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/descriptors/scaler.py` & `jaxip-0.7.1/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/logger.py` & `jaxip-0.7.1/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/models/nn/activation.py` & `jaxip-0.7.1/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/models/nn/initializer.py` & `jaxip-0.7.1/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/models/nn/network.py` & `jaxip-0.7.1/jaxip/models/nn/network.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from flax import linen as nn
 from frozendict import frozendict
 
 from jaxip.logger import logger
 from jaxip.models.model import ModelInterface
 from jaxip.models.nn.activation import _activation_function_map
-from jaxip.types import Array, Dtype
-from jaxip.types import _dtype
+from jaxip.types import Array, Dtype, _dtype
 
 
 class NeuralNetworkModel(nn.Module, ModelInterface):
     """Neural network model that outputs energy."""
 
     hidden_layers: Tuple[Tuple[int, str], ...]
     output_layer: Tuple[int, str] = (1, "identity")
```

### Comparing `jaxip-0.7.0/jaxip/potentials/_energy.py` & `jaxip-0.7.1/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/_force.py` & `jaxip-0.7.1/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/atomic_potential.py` & `jaxip-0.7.1/jaxip/potentials/atomic_potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.7.1/jaxip/potentials/nnp/gradient_descent.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
 
     def _init_train_state(self) -> Dict[Element, TrainState]:
         """Initialize train state for each element."""
 
         def generate_train_state():
             for element in self.potential.elements:
                 yield element, TrainState.create(
-                    apply_fn=self.potential.atomic_potential[element].model.apply,
+                    apply_fn=self.potential.atomic_potential[
+                        element
+                    ].model.apply,
                     params=self.potential.model_params[element],
                     tx=self.optimizer,  # [element]?
                 )
 
         return {element: state for element, state in generate_train_state()}
 
     # ------------------------------------------------------------------------
@@ -115,20 +117,26 @@
             loss_per_epoch: Array = jnp.array(0.0)
             loss_energy_per_epoch: Array = jnp.array(0.0)
             loss_force_per_epoch: Array = jnp.array(0.0)
             num_updates_per_epoch: int = 0
 
             # Loop over batches
             for _ in tqdm(range(steps)):
-                structures: List[Structure] = random.choices(dataset, k=batch_size)
+                structures: List[Structure] = random.choices(
+                    dataset, k=batch_size
+                )
                 xbatch = tuple(
-                    structure.get_per_element_inputs() for structure in structures
+                    structure.get_per_element_inputs()
+                    for structure in structures
                 )
                 ybatch = tuple(
-                    (structure.total_energy, structure.get_per_element_forces())
+                    (
+                        structure.total_energy,
+                        structure.get_per_element_forces(),
+                    )
                     for structure in structures
                 )
 
                 batch = xbatch, ybatch
                 states, metrics = self.train_step(states, batch)
 
                 loss_per_epoch += metrics["loss"]
@@ -166,17 +174,20 @@
             batch_size = len(xbatch)
 
             loss_energy_per_batch: Array = jnp.array(0.0)
             loss_force_per_batch: Array = jnp.array(0.0)
 
             for inputs, (true_energy, true_forces) in zip(xbatch, ybatch):
                 positions = {
-                    element: input.atom_position for element, input in inputs.items()
+                    element: input.atom_positions
+                    for element, input in inputs.items()
                 }
-                natoms: int = sum(array.shape[0] for array in positions.values())
+                natoms: int = sum(
+                    array.shape[0] for array in positions.values()
+                )
 
                 if np.random.rand() < self.force_fraction:
                     # ------ Force ------
                     forces = _compute_force(
                         frozendict(self.potential.atomic_potential),
                         positions,
                         params,
@@ -197,23 +208,27 @@
                     energy = _energy_fn(
                         frozendict(self.potential.atomic_potential),
                         positions,
                         params,
                         inputs,
                     )
                     loss_energy = (
-                        self.criterion(logits=energy, targets=true_energy) / natoms
+                        self.criterion(logits=energy, targets=true_energy)
+                        / natoms
                     )
                     loss_energy_per_batch += loss_energy
 
             loss_energy_per_batch /= batch_size
             loss_force_per_batch /= batch_size
             loss_per_batch = loss_energy_per_batch + loss_force_per_batch
 
-            return loss_per_batch, (loss_energy_per_batch, loss_force_per_batch)
+            return loss_per_batch, (
+                loss_energy_per_batch,
+                loss_force_per_batch,
+            )
 
         value_and_grad_fn = value_and_grad(loss_fn, has_aux=True)
 
         (loss, (loss_energy, loss_force)), grads = value_and_grad_fn(
             {element: state.params for element, state in states.items()}
         )
         states = {
```

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.7.1/jaxip/potentials/nnp/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/metrics.py` & `jaxip-0.7.1/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/nnp.py` & `jaxip-0.7.1/jaxip/potentials/nnp/nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/potential.py` & `jaxip-0.7.1/jaxip/potentials/nnp/potential.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/potentials/nnp/settings.py` & `jaxip-0.7.1/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/pytree.py` & `jaxip-0.7.1/jaxip/pytree.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/simulation/lj.py` & `jaxip-0.7.1/jaxip/simulation/lj.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/simulation/mc.py` & `jaxip-0.7.1/jaxip/simulation/mc.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/simulation/md.py` & `jaxip-0.7.1/jaxip/simulation/md.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,21 +31,48 @@
 def _get_temperature(velocities: Array, masses: Array) -> Array:
     kinetic_energy = _get_kinetic_energy(velocities, masses)
     natoms = velocities.shape[0]
     return 2 * kinetic_energy / (3 * natoms * KB)
 
 
 @jax.jit
-def _get_virial_term(
+def _get_virial(
     velocities: Array,
     masses: Array,
     positions: Array,
     forces: Array,
 ) -> Array:
-    return 2 * _get_kinetic_energy(velocities, masses) + (positions * forces).sum()
+    return (
+        2 * _get_kinetic_energy(velocities, masses)
+        + (positions * forces).sum()
+    )
+
+
+@jax.jit
+def _get_verlet_new_positions(
+    positions: Array,
+    velocities: Array,
+    forces: Array,
+    time_step: Array,
+) -> Array:
+    return (
+        positions
+        + velocities * time_step
+        + 0.5 * forces * time_step * time_step
+    )
+
+
+@jax.jit
+def _get_verlet_new_velocities(
+    velocities: Array,
+    forces: Array,
+    new_forces: Array,
+    time_step: Array,
+) -> Array:
+    return velocities + 0.5 * (forces + new_forces) * time_step
 
 
 def _get_potential_energy(
     potential: PotentialInterface,
     structure: Structure,
 ) -> Array:
     return potential(structure)
@@ -119,15 +146,17 @@
             logger.info(f"Generating random velocities ({temperature:0.2f} K)")
             self.velocities = self.generate_random_velocities(
                 temperature, masses=self.masses, seed=random_seed
             )
 
         if (self.thermostat is None) and (temperature is not None):
             logger.info(f"Initializing thermostat ({temperature:0.2f} K)")
-            logger.info("Setting default thermostat constant to 100x time step")
+            logger.info(
+                "Setting default thermostat constant to 100x time step"
+            )
             self.thermostat = BrendsenThermostat(
                 target_temperature=temperature,
                 time_constant=100 * self.time_step,
             )
 
         self.step: int = 0
         self.elapsed_time: float = 0.0
@@ -143,21 +172,22 @@
         self.temperature = _get_temperature(self.velocities, self.masses)
         if self.thermostat is not None:
             self.velocities = self.thermostat.get_rescaled_velocities(self)
             self.temperature = _get_temperature(self.velocities, self.masses)
 
     def verlet_integration(self) -> None:
         """Update atom positions and velocities based on Verlet algorithm."""
-        new_positions = (
-            self.positions
-            + self.velocities * self.time_step
-            + 0.5 * self.forces * self.time_step * self.time_step
+        arraylike_time_step = jnp.array(self.time_step)
+        new_positions = _get_verlet_new_positions(
+            self.positions, self.velocities, self.forces, arraylike_time_step
         )
         new_forces = _compute_forces(self.potential, self._structure)
-        self.velocities += 0.5 * (self.forces + new_forces) * self.time_step
+        self.velocities = _get_verlet_new_velocities(
+            self.velocities, self.forces, new_forces, arraylike_time_step
+        )
         self.forces = new_forces
         self._structure = replace(self._structure, positions=new_positions)
 
     @classmethod
     def generate_random_velocities(
         cls,
         temperature: float,
@@ -165,15 +195,17 @@
         seed: int,
     ) -> Array:
         """Generate Maxwell-Boltzmann distributed random velocities."""
         key = jax.random.PRNGKey(seed)
         masses = masses.reshape(-1, 1)
         natoms = masses.shape[0]
         velocities = jax.random.normal(key, shape=(natoms, 3))
-        velocities *= jnp.sqrt(temperature / _get_temperature(velocities, masses))
+        velocities *= jnp.sqrt(
+            temperature / _get_temperature(velocities, masses)
+        )
         velocities -= _calculate_center_of_mass(velocities, masses)
         return velocities
 
     def repr_physical_params(self) -> str:
         """Represent current physical parameters."""
         return (
             f"{self.step:<10} "
@@ -205,15 +237,15 @@
         )
 
     def get_pressure(self) -> Array:
         assert (
             self._structure.box
         ), "Calulating pressure... input structure must have PBC box"
         volume = self._structure.box.volume
-        virial = _get_virial_term(
+        virial = _get_virial(
             self.velocities,
             self.masses,
             self.positions,
             self.forces,
         )
         return virial / (3.0 * volume)  # type: ignore
```

### Comparing `jaxip-0.7.0/jaxip/simulation/run.py` & `jaxip-0.7.1/jaxip/simulation/run.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/simulation/thermostat.py` & `jaxip-0.7.1/jaxip/simulation/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/types.py` & `jaxip-0.7.1/jaxip/types.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/units.py` & `jaxip-0.7.1/jaxip/units.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/utils/attribute.py` & `jaxip-0.7.1/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/utils/batch.py` & `jaxip-0.7.1/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/utils/compare.py` & `jaxip-0.7.1/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/utils/profiler.py` & `jaxip-0.7.1/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip/utils/tokenize.py` & `jaxip-0.7.1/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/jaxip.egg-info/PKG-INFO` & `jaxip-0.7.1/jaxip.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.7.0
+Version: 0.7.1
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -37,30 +37,30 @@
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
 development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, material science. 
+for use in computational physics, chemistry, and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
 See `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
-* It uses `autograd` to make defining new descriptors straightforward.
+* It uses `automatic differentiation` to make defining new descriptors straightforward.
 * Jaxip is written purely in Python and optimized with `just-in-time` (JIT) compilation.
 * It also supports `GPU-accelerated` computing, which can significantly speed up preprocessing and model training.
 
 .. warning::
         This package is under heavy development and the current focus is on the implementation of high-dimensional 
         neural network potential (HDNNP) proposed by Behler et al. 
         (`2007 <https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.98.146401>`_).
@@ -149,15 +149,15 @@
         # Or loading from files
         #nnp.load()
 
         # Total energy
         nnp(structure)
 
         # Force components
-        nnp.compute_force(structure)
+        nnp.compute_forces(structure)
 
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
```

### Comparing `jaxip-0.7.0/jaxip.egg-info/SOURCES.txt` & `jaxip-0.7.1/jaxip.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 jaxip/atoms/box.py
 jaxip/atoms/element.py
 jaxip/atoms/neighbor.py
 jaxip/atoms/structure.py
 jaxip/datasets/__init__.py
 jaxip/datasets/dataset.py
 jaxip/datasets/runner.py
-jaxip/datasets/transformer.py
 jaxip/descriptors/__init__.py
 jaxip/descriptors/descriptor.py
 jaxip/descriptors/scaler.py
 jaxip/descriptors/acsf/__init__.py
 jaxip/descriptors/acsf/_acsf.py
 jaxip/descriptors/acsf/acsf.py
 jaxip/descriptors/acsf/angular.py
```

### Comparing `jaxip-0.7.0/setup.py` & `jaxip-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.7.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.7.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/h2o.data` & `jaxip-0.7.1/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/h2o.json` & `jaxip-0.7.1/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_acsf.py` & `jaxip-0.7.1/tests/test_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_mc.py` & `jaxip-0.7.1/tests/test_mc.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_md.py` & `jaxip-0.7.1/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_nn.py` & `jaxip-0.7.1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_nnp.py` & `jaxip-0.7.1/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_runner.py` & `jaxip-0.7.1/tests/test_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 from pathlib import Path
 from typing import Tuple
 
+from jaxip.types import _dtype
+
 os.environ["JAX_ENABLE_X64"] = "1"
 os.environ["JAX_PLATFORM_NAME"] = "cpu"
 
 import jax.numpy as jnp
 import pytest
 
 from jaxip.atoms.structure import Structure
 from jaxip.datasets.runner import RunnerDataset
 
-h2o_filename = Path("tests", "h2o.data")
+H2O_FILENAME = Path("tests", "h2o.data")
 H2O_DATA = {
     "lattice": [
         [11.8086403654, 0.0, 0.0],
         [0.0, 11.8086403654, 0.0],
         [0.0, 0.0, 11.8086403654],
     ],
     "positions": [
@@ -43,15 +45,28 @@
         0.452464,
         -0.432144,
         -0.0865354,
         0.430147,
         -0.0713622,
         -0.317081,
     ],
-    "energies": [-0.0, -0.0, -0.0, -0.0, -0.0, -0.0, 0.0, -0.0, -0.0, -0.0, -0.0, -0.0],
+    "energies": [
+        -0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+        0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+        -0.0,
+    ],
     "forces": [
         [0.0576867169, -0.2578270722, -0.2339365489],
         [-0.5157027617, -1.4143481512, -0.1199800167],
         [0.261360575, 2.1511972322, 0.444809068],
         [0.1560563599, -0.4345566594, -0.2367582949],
         [0.3723498983, 0.1835258917, -0.51876176],
         [-0.4569867202, -0.1613043018, 0.6545692241],
@@ -65,54 +80,60 @@
     "total_energy": [-32.2949885081],
     "total_charge": [-6e-07],
     "atom_types": [2, 1, 1, 2, 1, 1, 2, 1, 1, 2, 1, 1],
 }
 
 
 class TestRunnerDataset:
-    h2o: RunnerDataset = RunnerDataset(filename=h2o_filename)
-    h2o_raw: RunnerDataset = RunnerDataset(
-        filename=h2o_filename, transform=lambda x: x  # type: ignore
+    h2o: RunnerDataset = RunnerDataset(filename=H2O_FILENAME)
+    h2o_persist: RunnerDataset = RunnerDataset(
+        filename=H2O_FILENAME, persist=True
+    )
+    h2o_float64: RunnerDataset = RunnerDataset(
+        filename=H2O_FILENAME, dtype=jnp.float64
     )
-    h2o_persist: RunnerDataset = RunnerDataset(filename=h2o_filename, persist=True)
 
     @pytest.mark.parametrize(
-        "dataset",
+        "dataset, expected",
         [
-            h2o,
+            (
+                h2o,
+                (2, Structure),
+            ),
         ],
     )
-    def test_mandatory_methods(
+    def test_general(
         self,
         dataset: RunnerDataset,
+        expected: Tuple,
     ) -> None:
-        getattr(dataset, "__len__")
-        getattr(dataset, "__getitem__")
+        num_structures = len(dataset)
+        assert num_structures == expected[0]
+        for index in range(num_structures):
+            assert isinstance(dataset[index], expected[1])
 
     @pytest.mark.parametrize(
         "dataset, expected",
         [
             (
                 h2o,
-                (2, Structure),
+                (_dtype.FLOATX,),
             ),
             (
-                h2o_raw,
-                (2, dict),
+                h2o_float64,
+                (jnp.float64,),
             ),
         ],
     )
-    def test_general(
+    def test_dtype(
         self,
         dataset: RunnerDataset,
         expected: Tuple,
     ) -> None:
-        assert len(dataset) == expected[0]
-        for index in range(len(dataset)):
-            assert isinstance(dataset[index], expected[1])
+        assert dataset.dtype == expected[0]
 
     @pytest.mark.parametrize(
         "dataset, expected",
         [
             (
                 h2o,
                 (0, 0, 0, 0),
@@ -124,21 +145,21 @@
         ],
     )
     def test_caching(
         self,
         dataset: RunnerDataset,
         expected: Tuple,
     ) -> None:
-        assert len(dataset._cached_structures) == expected[0]
+        assert len(dataset._cache) == expected[0]
         dataset[0]
-        assert len(dataset._cached_structures) == expected[1]
+        assert len(dataset._cache) == expected[1]
         dataset[0]
-        assert len(dataset._cached_structures) == expected[2]
+        assert len(dataset._cache) == expected[2]
         dataset[1]
-        assert len(dataset._cached_structures) == expected[3]
+        assert len(dataset._cache) == expected[3]
 
     @pytest.mark.parametrize(
         "dataset, expected",
         [
             (
                 h2o,
                 tuple(
@@ -152,12 +173,19 @@
         self,
         dataset: RunnerDataset,
         expected: Tuple,
     ) -> None:
         structure: Structure = dataset[1]
         for i, attr in enumerate(Structure._get_atom_attributes()):
             if attr == "positions":
-                assert jnp.allclose(
-                    structure.positions, structure.box.shift_inside_box(expected[i])
-                )
+                if structure.box is not None:
+                    assert jnp.allclose(
+                        structure.positions,
+                        structure.box.shift_inside_box(expected[i]),
+                    )
+                else:
+                    assert jnp.allclose(
+                        structure.positions,
+                        expected[i],
+                    )
             else:
                 assert jnp.allclose(getattr(structure, attr), expected[i])
```

### Comparing `jaxip-0.7.0/tests/test_scaler.py` & `jaxip-0.7.1/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/test_structure.py` & `jaxip-0.7.1/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/weights.001.pkl` & `jaxip-0.7.1/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.0/tests/weights.008.pkl` & `jaxip-0.7.1/tests/weights.008.pkl`

 * *Files identical despite different names*

