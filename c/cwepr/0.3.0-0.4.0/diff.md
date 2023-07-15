# Comparing `tmp/cwepr-0.3.0.tar.gz` & `tmp/cwepr-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cwepr-0.3.0.tar", last modified: Sun Jul 24 08:28:20 2022, max compression
+gzip compressed data, was "dist/cwepr-0.4.0.tar", last modified: Sat Jul 15 15:23:20 2023, max compression
```

## Comparing `cwepr-0.3.0.tar` & `cwepr-0.4.0.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/
--rw-r--r--   0 till      (1000) adm          (4)      470 2021-06-02 15:39:14.000000 cwepr-0.3.0/.gitignore
--rw-r--r--   0 till      (1000) adm          (4)      422 2022-06-12 19:29:57.000000 cwepr-0.3.0/.prospector.yaml
--rw-r--r--   0 till      (1000) adm          (4)     2301 2022-06-12 19:25:46.000000 cwepr-0.3.0/CITATION.cff
--rw-r--r--   0 till      (1000) adm          (4)     1332 2022-06-12 19:25:46.000000 cwepr-0.3.0/LICENSE
--rw-r--r--   0 till      (1000) adm          (4)      267 2021-11-28 13:51:52.000000 cwepr-0.3.0/MANIFEST.in
--rw-r--r--   0 till      (1000) adm          (4)     6717 2022-07-24 08:28:20.000000 cwepr-0.3.0/PKG-INFO
--rw-r--r--   0 till      (1000) adm          (4)     4763 2022-06-12 19:25:46.000000 cwepr-0.3.0/README.rst
--rw-r--r--   0 till      (1000) adm          (4)        6 2022-07-24 08:27:03.000000 cwepr-0.3.0/VERSION
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/bin/
--rwxr-xr-x   0 till      (1000) adm          (4)     2018 2021-06-19 12:36:42.000000 cwepr-0.3.0/bin/incrementVersion.sh
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/
--rw-r--r--   0 till      (1000) adm          (4)       57 2020-05-31 10:15:55.000000 cwepr-0.3.0/cwepr/__init__.py
--rw-r--r--   0 till      (1000) adm          (4)    29432 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/analysis.py
--rw-r--r--   0 till      (1000) adm          (4)     3747 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/dataset.py
--rw-r--r--   0 till      (1000) adm          (4)     2869 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/exceptions.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/io/
--rw-r--r--   0 till      (1000) adm          (4)     1562 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/io/__init__.py
--rw-r--r--   0 till      (1000) adm          (4)    10711 2022-06-12 19:25:46.000000 cwepr-0.3.0/cwepr/io/bes3t.py
--rw-r--r--   0 till      (1000) adm          (4)      739 2022-06-12 19:25:46.000000 cwepr-0.3.0/cwepr/io/dsc_keys.yaml
--rw-r--r--   0 till      (1000) adm          (4)    10988 2022-06-12 19:34:54.000000 cwepr-0.3.0/cwepr/io/esp_winepr.py
--rw-r--r--   0 till      (1000) adm          (4)     5015 2022-06-12 19:35:05.000000 cwepr-0.3.0/cwepr/io/exporter.py
--rw-r--r--   0 till      (1000) adm          (4)     4619 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/io/factory.py
--rw-r--r--   0 till      (1000) adm          (4)    18054 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/io/magnettech.py
--rw-r--r--   0 till      (1000) adm          (4)    24849 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/io/niehs.py
--rw-r--r--   0 till      (1000) adm          (4)      556 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/io/par_defaults.yaml
--rw-r--r--   0 till      (1000) adm          (4)      597 2022-06-12 19:25:46.000000 cwepr-0.3.0/cwepr/io/par_keys.yaml
--rw-r--r--   0 till      (1000) adm          (4)     2175 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/io/txt_file.py
--rw-r--r--   0 till      (1000) adm          (4)    20318 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/metadata.py
--rw-r--r--   0 till      (1000) adm          (4)      500 2021-05-05 18:16:37.000000 cwepr-0.3.0/cwepr/metadata_mapper_cwepr.yaml
--rw-r--r--   0 till      (1000) adm          (4)    29106 2022-07-24 08:26:25.000000 cwepr-0.3.0/cwepr/plotting.py
--rw-r--r--   0 till      (1000) adm          (4)    41711 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/processing.py
--rw-r--r--   0 till      (1000) adm          (4)    13911 2022-06-12 19:25:46.000000 cwepr-0.3.0/cwepr/report.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/de/
--rw-r--r--   0 till      (1000) adm          (4)     2006 2021-06-19 12:36:42.000000 cwepr-0.3.0/cwepr/templates/de/DokuwikiCaption.txt.jinja
--rw-r--r--   0 till      (1000) adm          (4)     4747 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/templates/de/modulation_sweep_analysis_report.tex.jinja
--rw-r--r--   0 till      (1000) adm          (4)     4747 2021-06-02 20:18:09.000000 cwepr-0.3.0/cwepr/templates/de/power_sweep_report.tex.jinja
--rw-r--r--   0 till      (1000) adm          (4)     2275 2021-05-31 15:48:39.000000 cwepr-0.3.0/cwepr/templates/de/report.tex.jinja
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/en/
--rw-r--r--   0 till      (1000) adm          (4)     2004 2021-06-19 12:36:42.000000 cwepr-0.3.0/cwepr/templates/en/DokuwikiCaption.txt.jinja
--rw-r--r--   0 till      (1000) adm          (4)     4918 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/templates/en/Infofile.info.jinja
--rw-r--r--   0 till      (1000) adm          (4)     2233 2021-05-31 15:48:39.000000 cwepr-0.3.0/cwepr/templates/en/power_sweep_report_generic.tex.jinja
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/report/
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/report/latex/
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/report/latex/de/
--rw-r--r--   0 till      (1000) adm          (4)     1129 2022-06-12 19:34:36.000000 cwepr-0.3.0/cwepr/templates/report/latex/de/kolophon.tex
--rw-r--r--   0 till      (1000) adm          (4)     3020 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/templates/report/latex/de/metadaten_experimentell.tex
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr/templates/report/latex/en/
--rw-r--r--   0 till      (1000) adm          (4)     1097 2022-06-12 19:34:36.000000 cwepr-0.3.0/cwepr/templates/report/latex/en/colophon.tex
--rw-r--r--   0 till      (1000) adm          (4)     3031 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/templates/report/latex/en/metadata_experimental.tex
--rw-r--r--   0 till      (1000) adm          (4)     2967 2021-11-28 13:51:52.000000 cwepr-0.3.0/cwepr/utils.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/cwepr.egg-info/
--rw-r--r--   0 till      (1000) adm          (4)     6717 2022-07-24 08:28:19.000000 cwepr-0.3.0/cwepr.egg-info/PKG-INFO
--rw-r--r--   0 till      (1000) adm          (4)     6133 2022-07-24 08:28:19.000000 cwepr-0.3.0/cwepr.egg-info/SOURCES.txt
--rw-r--r--   0 till      (1000) adm          (4)        1 2022-07-24 08:28:19.000000 cwepr-0.3.0/cwepr.egg-info/dependency_links.txt
--rw-r--r--   0 till      (1000) adm          (4)      108 2022-07-24 08:28:19.000000 cwepr-0.3.0/cwepr.egg-info/requires.txt
--rw-r--r--   0 till      (1000) adm          (4)        6 2022-07-24 08:28:19.000000 cwepr-0.3.0/cwepr.egg-info/top_level.txt
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/docs/
--rw-r--r--   0 till      (1000) adm          (4)      939 2021-05-20 20:14:04.000000 cwepr-0.3.0/docs/CalculatedDataset.yaml
--rw-r--r--   0 till      (1000) adm          (4)     2878 2021-06-03 10:26:42.000000 cwepr-0.3.0/docs/ExperimentalDataset.yaml
--rw-r--r--   0 till      (1000) adm          (4)      741 2021-06-02 15:28:38.000000 cwepr-0.3.0/docs/Makefile
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/docs/_templates/
--rw-r--r--   0 till      (1000) adm          (4)      756 2021-06-02 15:34:40.000000 cwepr-0.3.0/docs/_templates/page.html
--rw-r--r--   0 till      (1000) adm          (4)      803 2021-06-02 15:34:40.000000 cwepr-0.3.0/docs/_templates/versions.html
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/docs/api/
--rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.analysis.rst
--rw-r--r--   0 till      (1000) adm          (4)      127 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.dataset.rst
--rw-r--r--   0 till      (1000) adm          (4)      136 2021-05-20 20:05:57.000000 cwepr-0.3.0/docs/api/cwepr.exceptions.rst
--rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.io.bes3t.rst
--rw-r--r--   0 till      (1000) adm          (4)      145 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/api/cwepr.io.esp_winepr.rst
--rw-r--r--   0 till      (1000) adm          (4)      139 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.io.exporter.rst
--rw-r--r--   0 till      (1000) adm          (4)      136 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.io.factory.rst
--rw-r--r--   0 till      (1000) adm          (4)      145 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.io.magnettech.rst
--rw-r--r--   0 till      (1000) adm          (4)      289 2022-07-24 08:26:25.000000 cwepr-0.3.0/docs/api/cwepr.io.rst
--rw-r--r--   0 till      (1000) adm          (4)      139 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/api/cwepr.io.txt_file.rst
--rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.metadata.rst
--rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.plotting.rst
--rw-r--r--   0 till      (1000) adm          (4)      136 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.processing.rst
--rw-r--r--   0 till      (1000) adm          (4)      124 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/api/cwepr.report.rst
--rw-r--r--   0 till      (1000) adm          (4)      121 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/api/cwepr.utils.rst
--rw-r--r--   0 till      (1000) adm          (4)     1001 2022-07-24 08:26:25.000000 cwepr-0.3.0/docs/api/index.rst
--rw-r--r--   0 till      (1000) adm          (4)     1456 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/audience.rst
--rw-r--r--   0 till      (1000) adm          (4)     3061 2022-07-24 08:27:03.000000 cwepr-0.3.0/docs/changelog.rst
--rw-r--r--   0 till      (1000) adm          (4)     4835 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/concepts.rst
--rw-r--r--   0 till      (1000) adm          (4)     7733 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/conf.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/docs/cwepr/
--rw-r--r--   0 till      (1000) adm          (4)    11620 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/cwepr/analysis.rst
--rw-r--r--   0 till      (1000) adm          (4)     2732 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/cwepr/index.rst
--rw-r--r--   0 till      (1000) adm          (4)    13338 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/cwepr/processing.rst
--rw-r--r--   0 till      (1000) adm          (4)    14821 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/cwepr/recording.rst
--rw-r--r--   0 till      (1000) adm          (4)    16958 2020-05-31 10:15:55.000000 cwepr-0.3.0/docs/cwepr-favicon.ico
--rw-r--r--   0 till      (1000) adm          (4)    38260 2020-05-31 10:15:55.000000 cwepr-0.3.0/docs/cwepr-logo.png
--rw-r--r--   0 till      (1000) adm          (4)     1693 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/dataset-structure.rst
--rw-r--r--   0 till      (1000) adm          (4)      398 2021-05-20 20:11:01.000000 cwepr-0.3.0/docs/datasets2yaml.py
--rw-r--r--   0 till      (1000) adm          (4)     5382 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/developers.rst
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/docs/examples/
--rw-r--r--   0 till      (1000) adm          (4)     1019 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/examples/first-overview.rst
--rw-r--r--   0 till      (1000) adm          (4)     1182 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/examples/index.rst
--rw-r--r--   0 till      (1000) adm          (4)      409 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/examples/list.rst
--rw-r--r--   0 till      (1000) adm          (4)     1024 2021-11-28 13:51:52.000000 cwepr-0.3.0/docs/examples/power-sweep-analysis.rst
--rw-r--r--   0 till      (1000) adm          (4)     7346 2022-07-24 08:26:25.000000 cwepr-0.3.0/docs/index.rst
--rw-r--r--   0 till      (1000) adm          (4)     3007 2021-11-28 13:51:53.000000 cwepr-0.3.0/docs/installing.rst
--rw-r--r--   0 till      (1000) adm          (4)     4859 2021-01-31 18:04:25.000000 cwepr-0.3.0/docs/introduction.rst
--rw-r--r--   0 till      (1000) adm          (4)     3166 2021-11-28 13:51:53.000000 cwepr-0.3.0/docs/literature.bib
--rw-r--r--   0 till      (1000) adm          (4)      787 2020-05-31 10:15:55.000000 cwepr-0.3.0/docs/make.bat
--rw-r--r--   0 till      (1000) adm          (4)      807 2021-11-28 13:51:53.000000 cwepr-0.3.0/docs/people.rst
--rw-r--r--   0 till      (1000) adm          (4)     1652 2022-07-24 08:26:25.000000 cwepr-0.3.0/docs/roadmap.rst
--rw-r--r--   0 till      (1000) adm          (4)    11755 2022-07-24 08:26:25.000000 cwepr-0.3.0/docs/usecases.rst
--rw-r--r--   0 till      (1000) adm          (4)       47 2021-06-03 10:28:05.000000 cwepr-0.3.0/requirements.txt
--rw-r--r--   0 till      (1000) adm          (4)       38 2022-07-24 08:28:20.000000 cwepr-0.3.0/setup.cfg
--rw-r--r--   0 till      (1000) adm          (4)     1838 2021-11-28 13:51:53.000000 cwepr-0.3.0/setup.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/tests/
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/tests/io/
--rw-r--r--   0 till      (1000) adm          (4)     4788 2022-06-12 19:25:46.000000 cwepr-0.3.0/tests/io/test_bes3t.py
--rw-r--r--   0 till      (1000) adm          (4)     4408 2022-06-12 19:25:46.000000 cwepr-0.3.0/tests/io/test_esp_winepr.py
--rw-r--r--   0 till      (1000) adm          (4)     1879 2021-05-28 19:26:44.000000 cwepr-0.3.0/tests/io/test_exporter.py
--rw-r--r--   0 till      (1000) adm          (4)     2779 2022-07-24 08:26:25.000000 cwepr-0.3.0/tests/io/test_factory.py
--rw-r--r--   0 till      (1000) adm          (4)     6587 2022-06-12 19:25:46.000000 cwepr-0.3.0/tests/io/test_magnettech.py
--rw-r--r--   0 till      (1000) adm          (4)      401 2021-05-28 19:26:44.000000 cwepr-0.3.0/tests/io/test_txt_file.py
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/tests/io/testdata/
--rwxr-xr-x   0 till      (1000) adm          (4)     2933 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)    24000 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)     2055 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.info
--rwxr-xr-x   0 till      (1000) adm          (4)     2759 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)    96000 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)     2081 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.info
--rwxr-xr-x   0 till      (1000) adm          (4)     3075 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)   239920 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)       80 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.YGF
--rwxr-xr-x   0 till      (1000) adm          (4)     2099 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.info
--rwxr-xr-x   0 till      (1000) adm          (4)     3286 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)   335888 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)      112 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.YGF
--rwxr-xr-x   0 till      (1000) adm          (4)     2093 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.info
--rwxr-xr-x   0 till      (1000) adm          (4)     2962 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)   320000 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)      160 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.YGF
--rwxr-xr-x   0 till      (1000) adm          (4)     2134 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.info
--rw-r--r--   0 till      (1000) adm          (4)     2110 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/EMX-winEPR.info
--rwxr-xr-x   0 till      (1000) adm          (4)      327 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/EMX-winEPR.par
--rwxr-xr-x   0 till      (1000) adm          (4)     4096 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/EMX-winEPR.spc
--rw-r--r--   0 till      (1000) adm          (4)     2270 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/ESP.info
--rw-r--r--   0 till      (1000) adm          (4)      267 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/ESP.par
--rw-r--r--   0 till      (1000) adm          (4)     4096 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/ESP.spc
-drwxr-xr-x   0 till      (1000) adm          (4)        0 2022-07-24 08:28:20.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/
--rwxr-xr-x   0 till      (1000) adm          (4)   221427 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120018656_goniometersweep-testdata_F_gon_0dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221869 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120054089_goniometersweep-testdata_F_gon_10dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221437 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120129135_goniometersweep-testdata_F_gon_20dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221798 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120204063_goniometersweep-testdata_F_gon_30dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221738 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120238999_goniometersweep-testdata_F_gon_40dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221870 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120314263_goniometersweep-testdata_F_gon_50dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222003 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120349297_goniometersweep-testdata_F_gon_60dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221882 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120424603_goniometersweep-testdata_F_gon_70dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221748 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120500130_goniometersweep-testdata_F_gon_80dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   221750 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120536148_goniometersweep-testdata_F_gon_90dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222485 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120611356_goniometersweep-testdata_F_gon_100dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222293 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120646202_goniometersweep-testdata_F_gon_110dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222209 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120721430_goniometersweep-testdata_F_gon_120dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222087 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120756411_goniometersweep-testdata_F_gon_130dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222219 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120831365_goniometersweep-testdata_F_gon_140dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222505 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120906619_goniometersweep-testdata_F_gon_150dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222460 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120941813_goniometersweep-testdata_F_gon_160dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222149 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_121017977_goniometersweep-testdata_F_gon_170dg.xml
--rwxr-xr-x   0 till      (1000) adm          (4)   222425 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_121054028_goniometersweep-testdata_F_gon_180dg.xml
--rw-r--r--   0 till      (1000) adm          (4)     1981 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/magnettech-goniometer.info
--rw-r--r--   0 till      (1000) adm          (4)     1450 2022-07-24 08:26:25.000000 cwepr-0.3.0/tests/io/testdata/modulation-amplitude-analysis.yaml
--rw-r--r--   0 till      (1000) adm          (4)    35398 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/noisy_data.txt
--rw-r--r--   0 till      (1000) adm          (4)    38314 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/not_noisy_data.txt
--rw-r--r--   0 till      (1000) adm          (4)   208494 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/phase-45_noise0.000.txt
--rw-r--r--   0 till      (1000) adm          (4)    50859 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/phase-45_noise0.000_small.txt
--rw-r--r--   0 till      (1000) adm          (4)    50554 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/phase-45_noise0.100.txt
--rw-r--r--   0 till      (1000) adm          (4)    35381 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/phase_shift.txt
--rw-r--r--   0 till      (1000) adm          (4)     1308 2022-07-24 08:26:25.000000 cwepr-0.3.0/tests/io/testdata/power-sweep-analysis.yaml
--rw-r--r--   0 till      (1000) adm          (4)    35511 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/sinus_baseline.txt
--rwxr-xr-x   0 till      (1000) adm          (4)     2947 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DSC
--rwxr-xr-x   0 till      (1000) adm          (4)     8000 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DTA
--rwxr-xr-x   0 till      (1000) adm          (4)     2057 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.info
--rw-r--r--   0 till      (1000) adm          (4)     1993 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/test-magnettech.info
--rwxr-xr-x   0 till      (1000) adm          (4)   220079 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/io/testdata/test-magnettech.xml
--rwxr-xr-x   0 till      (1000) adm          (4)      432 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/winepr.par
--rwxr-xr-x   0 till      (1000) adm          (4)     8192 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/io/testdata/winepr.spc
--rw-r--r--   0 till      (1000) adm          (4)    11879 2022-07-24 08:26:25.000000 cwepr-0.3.0/tests/test_analysis.py
--rw-r--r--   0 till      (1000) adm          (4)      695 2021-01-31 18:04:25.000000 cwepr-0.3.0/tests/test_dataset.py
--rw-r--r--   0 till      (1000) adm          (4)     8044 2022-06-12 19:25:46.000000 cwepr-0.3.0/tests/test_plotting.py
--rw-r--r--   0 till      (1000) adm          (4)     7604 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/test_processing.py
--rw-r--r--   0 till      (1000) adm          (4)     7454 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/test_report.py
--rw-r--r--   0 till      (1000) adm          (4)     1734 2021-11-28 13:51:53.000000 cwepr-0.3.0/tests/test_utils.py
--rw-r--r--   0 till      (1000) adm          (4)      582 2021-06-03 10:26:42.000000 cwepr-0.3.0/tox.ini
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/
+-rw-r--r--   0 till      (1000) adm          (4)      470 2021-06-02 15:39:14.000000 cwepr-0.4.0/.gitignore
+-rw-r--r--   0 till      (1000) adm          (4)      422 2022-06-12 19:29:57.000000 cwepr-0.4.0/.prospector.yaml
+-rw-r--r--   0 till      (1000) adm          (4)     2301 2022-06-12 19:25:46.000000 cwepr-0.4.0/CITATION.cff
+-rw-r--r--   0 till      (1000) adm          (4)     1332 2022-06-12 19:25:46.000000 cwepr-0.4.0/LICENSE
+-rw-r--r--   0 till      (1000) adm          (4)      267 2021-11-28 13:51:52.000000 cwepr-0.4.0/MANIFEST.in
+-rw-r--r--   0 till      (1000) adm          (4)     6717 2023-07-15 15:23:20.000000 cwepr-0.4.0/PKG-INFO
+-rw-r--r--   0 till      (1000) adm          (4)     4763 2022-06-12 19:25:46.000000 cwepr-0.4.0/README.rst
+-rw-r--r--   0 till      (1000) adm          (4)        5 2023-07-15 15:23:09.000000 cwepr-0.4.0/VERSION
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/bin/
+-rwxr-xr-x   0 till      (1000) adm          (4)     2018 2021-06-19 12:36:42.000000 cwepr-0.4.0/bin/incrementVersion.sh
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/
+-rw-r--r--   0 till      (1000) adm          (4)       57 2020-05-31 10:15:55.000000 cwepr-0.4.0/cwepr/__init__.py
+-rw-r--r--   0 till      (1000) adm          (4)    30930 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/analysis.py
+-rw-r--r--   0 till      (1000) adm          (4)     3747 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/dataset.py
+-rw-r--r--   0 till      (1000) adm          (4)     2869 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/exceptions.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/io/
+-rw-r--r--   0 till      (1000) adm          (4)     1625 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/__init__.py
+-rw-r--r--   0 till      (1000) adm          (4)    10707 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/bes3t.py
+-rw-r--r--   0 till      (1000) adm          (4)      739 2022-06-12 19:25:46.000000 cwepr-0.4.0/cwepr/io/dsc_keys.yaml
+-rw-r--r--   0 till      (1000) adm          (4)    10831 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/esp_winepr.py
+-rw-r--r--   0 till      (1000) adm          (4)     5008 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/exporter.py
+-rw-r--r--   0 till      (1000) adm          (4)     6112 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/factory.py
+-rw-r--r--   0 till      (1000) adm          (4)    37481 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/magnettech.py
+-rw-r--r--   0 till      (1000) adm          (4)      875 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/magnettech_keys.yaml
+-rw-r--r--   0 till      (1000) adm          (4)    24847 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/niehs.py
+-rw-r--r--   0 till      (1000) adm          (4)      556 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/io/par_defaults.yaml
+-rw-r--r--   0 till      (1000) adm          (4)      597 2022-06-12 19:25:46.000000 cwepr-0.4.0/cwepr/io/par_keys.yaml
+-rw-r--r--   0 till      (1000) adm          (4)     2779 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/io/txt_file.py
+-rw-r--r--   0 till      (1000) adm          (4)    21452 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/metadata.py
+-rw-r--r--   0 till      (1000) adm          (4)      512 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/metadata_mapper_cwepr.yaml
+-rw-r--r--   0 till      (1000) adm          (4)    29106 2022-07-24 08:26:25.000000 cwepr-0.4.0/cwepr/plotting.py
+-rw-r--r--   0 till      (1000) adm          (4)    44466 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/processing.py
+-rw-r--r--   0 till      (1000) adm          (4)    13889 2023-07-15 15:22:21.000000 cwepr-0.4.0/cwepr/report.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/de/
+-rw-r--r--   0 till      (1000) adm          (4)     2006 2021-06-19 12:36:42.000000 cwepr-0.4.0/cwepr/templates/de/DokuwikiCaption.txt.jinja
+-rw-r--r--   0 till      (1000) adm          (4)     4747 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/templates/de/modulation_sweep_analysis_report.tex.jinja
+-rw-r--r--   0 till      (1000) adm          (4)     4747 2021-06-02 20:18:09.000000 cwepr-0.4.0/cwepr/templates/de/power_sweep_report.tex.jinja
+-rw-r--r--   0 till      (1000) adm          (4)     2275 2021-05-31 15:48:39.000000 cwepr-0.4.0/cwepr/templates/de/report.tex.jinja
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/en/
+-rw-r--r--   0 till      (1000) adm          (4)     2004 2021-06-19 12:36:42.000000 cwepr-0.4.0/cwepr/templates/en/DokuwikiCaption.txt.jinja
+-rw-r--r--   0 till      (1000) adm          (4)     4918 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/templates/en/Infofile.info.jinja
+-rw-r--r--   0 till      (1000) adm          (4)     2233 2021-05-31 15:48:39.000000 cwepr-0.4.0/cwepr/templates/en/power_sweep_report_generic.tex.jinja
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/report/
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/report/latex/
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/report/latex/de/
+-rw-r--r--   0 till      (1000) adm          (4)     1129 2022-06-12 19:34:36.000000 cwepr-0.4.0/cwepr/templates/report/latex/de/kolophon.tex
+-rw-r--r--   0 till      (1000) adm          (4)     3020 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/templates/report/latex/de/metadaten_experimentell.tex
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr/templates/report/latex/en/
+-rw-r--r--   0 till      (1000) adm          (4)     1097 2022-06-12 19:34:36.000000 cwepr-0.4.0/cwepr/templates/report/latex/en/colophon.tex
+-rw-r--r--   0 till      (1000) adm          (4)     3031 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/templates/report/latex/en/metadata_experimental.tex
+-rw-r--r--   0 till      (1000) adm          (4)     2967 2021-11-28 13:51:52.000000 cwepr-0.4.0/cwepr/utils.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/
+-rw-r--r--   0 till      (1000) adm          (4)     6717 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/PKG-INFO
+-rw-r--r--   0 till      (1000) adm          (4)     6163 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/SOURCES.txt
+-rw-r--r--   0 till      (1000) adm          (4)        1 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/dependency_links.txt
+-rw-r--r--   0 till      (1000) adm          (4)      108 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/requires.txt
+-rw-r--r--   0 till      (1000) adm          (4)        6 2023-07-15 15:23:20.000000 cwepr-0.4.0/cwepr.egg-info/top_level.txt
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/docs/
+-rw-r--r--   0 till      (1000) adm          (4)      939 2021-05-20 20:14:04.000000 cwepr-0.4.0/docs/CalculatedDataset.yaml
+-rw-r--r--   0 till      (1000) adm          (4)     2878 2021-06-03 10:26:42.000000 cwepr-0.4.0/docs/ExperimentalDataset.yaml
+-rw-r--r--   0 till      (1000) adm          (4)      741 2021-06-02 15:28:38.000000 cwepr-0.4.0/docs/Makefile
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/docs/_templates/
+-rw-r--r--   0 till      (1000) adm          (4)      756 2021-06-02 15:34:40.000000 cwepr-0.4.0/docs/_templates/page.html
+-rw-r--r--   0 till      (1000) adm          (4)      803 2021-06-02 15:34:40.000000 cwepr-0.4.0/docs/_templates/versions.html
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/docs/api/
+-rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.analysis.rst
+-rw-r--r--   0 till      (1000) adm          (4)      127 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.dataset.rst
+-rw-r--r--   0 till      (1000) adm          (4)      136 2021-05-20 20:05:57.000000 cwepr-0.4.0/docs/api/cwepr.exceptions.rst
+-rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.io.bes3t.rst
+-rw-r--r--   0 till      (1000) adm          (4)      145 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/api/cwepr.io.esp_winepr.rst
+-rw-r--r--   0 till      (1000) adm          (4)      139 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.io.exporter.rst
+-rw-r--r--   0 till      (1000) adm          (4)      136 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.io.factory.rst
+-rw-r--r--   0 till      (1000) adm          (4)      145 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.io.magnettech.rst
+-rw-r--r--   0 till      (1000) adm          (4)      289 2022-07-24 08:26:25.000000 cwepr-0.4.0/docs/api/cwepr.io.rst
+-rw-r--r--   0 till      (1000) adm          (4)      139 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/api/cwepr.io.txt_file.rst
+-rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.metadata.rst
+-rw-r--r--   0 till      (1000) adm          (4)      130 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.plotting.rst
+-rw-r--r--   0 till      (1000) adm          (4)      136 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.processing.rst
+-rw-r--r--   0 till      (1000) adm          (4)      124 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/api/cwepr.report.rst
+-rw-r--r--   0 till      (1000) adm          (4)      121 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/api/cwepr.utils.rst
+-rw-r--r--   0 till      (1000) adm          (4)     1001 2022-07-24 08:26:25.000000 cwepr-0.4.0/docs/api/index.rst
+-rw-r--r--   0 till      (1000) adm          (4)     1456 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/audience.rst
+-rw-r--r--   0 till      (1000) adm          (4)     4412 2023-07-15 15:23:09.000000 cwepr-0.4.0/docs/changelog.rst
+-rw-r--r--   0 till      (1000) adm          (4)     4931 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/concepts.rst
+-rw-r--r--   0 till      (1000) adm          (4)     7723 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/conf.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/docs/cwepr/
+-rw-r--r--   0 till      (1000) adm          (4)    11649 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/cwepr/analysis.rst
+-rw-r--r--   0 till      (1000) adm          (4)     2732 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/cwepr/index.rst
+-rw-r--r--   0 till      (1000) adm          (4)    13338 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/cwepr/processing.rst
+-rw-r--r--   0 till      (1000) adm          (4)    20729 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/cwepr/recording.rst
+-rw-r--r--   0 till      (1000) adm          (4)    16958 2020-05-31 10:15:55.000000 cwepr-0.4.0/docs/cwepr-favicon.ico
+-rw-r--r--   0 till      (1000) adm          (4)    38260 2020-05-31 10:15:55.000000 cwepr-0.4.0/docs/cwepr-logo.png
+-rw-r--r--   0 till      (1000) adm          (4)     1693 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/dataset-structure.rst
+-rw-r--r--   0 till      (1000) adm          (4)      398 2021-05-20 20:11:01.000000 cwepr-0.4.0/docs/datasets2yaml.py
+-rw-r--r--   0 till      (1000) adm          (4)     5584 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/developers.rst
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/docs/examples/
+-rw-r--r--   0 till      (1000) adm          (4)     1019 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/examples/first-overview.rst
+-rw-r--r--   0 till      (1000) adm          (4)     2333 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/examples/index.rst
+-rw-r--r--   0 till      (1000) adm          (4)      409 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/examples/list.rst
+-rw-r--r--   0 till      (1000) adm          (4)     1024 2021-11-28 13:51:52.000000 cwepr-0.4.0/docs/examples/power-sweep-analysis.rst
+-rw-r--r--   0 till      (1000) adm          (4)     8235 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/index.rst
+-rw-r--r--   0 till      (1000) adm          (4)     3007 2021-11-28 13:51:53.000000 cwepr-0.4.0/docs/installing.rst
+-rw-r--r--   0 till      (1000) adm          (4)     4859 2021-01-31 18:04:25.000000 cwepr-0.4.0/docs/introduction.rst
+-rw-r--r--   0 till      (1000) adm          (4)     3166 2021-11-28 13:51:53.000000 cwepr-0.4.0/docs/literature.bib
+-rw-r--r--   0 till      (1000) adm          (4)      787 2020-05-31 10:15:55.000000 cwepr-0.4.0/docs/make.bat
+-rw-r--r--   0 till      (1000) adm          (4)      807 2021-11-28 13:51:53.000000 cwepr-0.4.0/docs/people.rst
+-rw-r--r--   0 till      (1000) adm          (4)     2016 2023-07-15 15:22:21.000000 cwepr-0.4.0/docs/roadmap.rst
+-rw-r--r--   0 till      (1000) adm          (4)    11755 2022-07-24 08:26:25.000000 cwepr-0.4.0/docs/usecases.rst
+-rw-r--r--   0 till      (1000) adm          (4)       63 2023-07-15 15:22:21.000000 cwepr-0.4.0/requirements.txt
+-rw-r--r--   0 till      (1000) adm          (4)       38 2023-07-15 15:23:20.000000 cwepr-0.4.0/setup.cfg
+-rw-r--r--   0 till      (1000) adm          (4)     1838 2023-07-15 15:22:21.000000 cwepr-0.4.0/setup.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/tests/
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/tests/io/
+-rw-r--r--   0 till      (1000) adm          (4)     4788 2022-06-12 19:25:46.000000 cwepr-0.4.0/tests/io/test_bes3t.py
+-rw-r--r--   0 till      (1000) adm          (4)     4408 2022-06-12 19:25:46.000000 cwepr-0.4.0/tests/io/test_esp_winepr.py
+-rw-r--r--   0 till      (1000) adm          (4)     1879 2021-05-28 19:26:44.000000 cwepr-0.4.0/tests/io/test_exporter.py
+-rw-r--r--   0 till      (1000) adm          (4)     3222 2023-07-15 15:22:21.000000 cwepr-0.4.0/tests/io/test_factory.py
+-rw-r--r--   0 till      (1000) adm          (4)    18871 2023-07-15 15:22:21.000000 cwepr-0.4.0/tests/io/test_magnettech.py
+-rw-r--r--   0 till      (1000) adm          (4)      401 2021-05-28 19:26:44.000000 cwepr-0.4.0/tests/io/test_txt_file.py
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/tests/io/testdata/
+-rwxr-xr-x   0 till      (1000) adm          (4)     2933 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)    24000 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)     2055 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.info
+-rwxr-xr-x   0 till      (1000) adm          (4)     2759 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)    96000 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)     2081 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.info
+-rwxr-xr-x   0 till      (1000) adm          (4)     3075 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)   239920 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)       80 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.YGF
+-rwxr-xr-x   0 till      (1000) adm          (4)     2099 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.info
+-rwxr-xr-x   0 till      (1000) adm          (4)     3286 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)   335888 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)      112 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.YGF
+-rwxr-xr-x   0 till      (1000) adm          (4)     2093 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.info
+-rwxr-xr-x   0 till      (1000) adm          (4)     2962 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)   320000 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)      160 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.YGF
+-rwxr-xr-x   0 till      (1000) adm          (4)     2134 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.info
+-rw-r--r--   0 till      (1000) adm          (4)     2110 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/EMX-winEPR.info
+-rwxr-xr-x   0 till      (1000) adm          (4)      327 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/EMX-winEPR.par
+-rwxr-xr-x   0 till      (1000) adm          (4)     4096 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/EMX-winEPR.spc
+-rw-r--r--   0 till      (1000) adm          (4)     2270 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/ESP.info
+-rw-r--r--   0 till      (1000) adm          (4)      267 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/ESP.par
+-rw-r--r--   0 till      (1000) adm          (4)     4096 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/ESP.spc
+drwxr-xr-x   0 till      (1000) adm          (4)        0 2023-07-15 15:23:20.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/
+-rwxr-xr-x   0 till      (1000) adm          (4)   221427 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120018656_goniometersweep-testdata_F_gon_0dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221869 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120054089_goniometersweep-testdata_F_gon_10dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221437 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120129135_goniometersweep-testdata_F_gon_20dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221798 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120204063_goniometersweep-testdata_F_gon_30dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221738 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120238999_goniometersweep-testdata_F_gon_40dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221870 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120314263_goniometersweep-testdata_F_gon_50dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222003 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120349297_goniometersweep-testdata_F_gon_60dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221882 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120424603_goniometersweep-testdata_F_gon_70dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221748 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120500130_goniometersweep-testdata_F_gon_80dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   221750 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120536148_goniometersweep-testdata_F_gon_90dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222485 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120611356_goniometersweep-testdata_F_gon_100dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222293 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120646202_goniometersweep-testdata_F_gon_110dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222209 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120721430_goniometersweep-testdata_F_gon_120dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222087 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120756411_goniometersweep-testdata_F_gon_130dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222219 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120831365_goniometersweep-testdata_F_gon_140dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222505 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120906619_goniometersweep-testdata_F_gon_150dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222460 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120941813_goniometersweep-testdata_F_gon_160dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222149 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_121017977_goniometersweep-testdata_F_gon_170dg.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)   222425 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_121054028_goniometersweep-testdata_F_gon_180dg.xml
+-rw-r--r--   0 till      (1000) adm          (4)     1981 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/magnettech-goniometer.info
+-rw-r--r--   0 till      (1000) adm          (4)     1450 2022-07-24 08:26:25.000000 cwepr-0.4.0/tests/io/testdata/modulation-amplitude-analysis.yaml
+-rw-r--r--   0 till      (1000) adm          (4)    35398 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/noisy_data.txt
+-rw-r--r--   0 till      (1000) adm          (4)    38314 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/not_noisy_data.txt
+-rw-r--r--   0 till      (1000) adm          (4)   208494 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/phase-45_noise0.000.txt
+-rw-r--r--   0 till      (1000) adm          (4)    50859 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/phase-45_noise0.000_small.txt
+-rw-r--r--   0 till      (1000) adm          (4)    50554 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/phase-45_noise0.100.txt
+-rw-r--r--   0 till      (1000) adm          (4)    35381 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/phase_shift.txt
+-rw-r--r--   0 till      (1000) adm          (4)     1308 2022-07-24 08:26:25.000000 cwepr-0.4.0/tests/io/testdata/power-sweep-analysis.yaml
+-rw-r--r--   0 till      (1000) adm          (4)    35511 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/sinus_baseline.txt
+-rwxr-xr-x   0 till      (1000) adm          (4)     2947 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DSC
+-rwxr-xr-x   0 till      (1000) adm          (4)     8000 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DTA
+-rwxr-xr-x   0 till      (1000) adm          (4)     2057 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.info
+-rw-r--r--   0 till      (1000) adm          (4)     2254 2023-07-15 15:22:21.000000 cwepr-0.4.0/tests/io/testdata/test-magnettech.info
+-rwxr-xr-x   0 till      (1000) adm          (4)   220079 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/io/testdata/test-magnettech.xml
+-rwxr-xr-x   0 till      (1000) adm          (4)      432 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/winepr.par
+-rwxr-xr-x   0 till      (1000) adm          (4)     8192 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/io/testdata/winepr.spc
+-rw-r--r--   0 till      (1000) adm          (4)    11879 2023-07-15 15:22:21.000000 cwepr-0.4.0/tests/test_analysis.py
+-rw-r--r--   0 till      (1000) adm          (4)      695 2021-01-31 18:04:25.000000 cwepr-0.4.0/tests/test_dataset.py
+-rw-r--r--   0 till      (1000) adm          (4)     8044 2022-06-12 19:25:46.000000 cwepr-0.4.0/tests/test_plotting.py
+-rw-r--r--   0 till      (1000) adm          (4)    11822 2023-07-15 15:22:21.000000 cwepr-0.4.0/tests/test_processing.py
+-rw-r--r--   0 till      (1000) adm          (4)     7454 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/test_report.py
+-rw-r--r--   0 till      (1000) adm          (4)     1734 2021-11-28 13:51:53.000000 cwepr-0.4.0/tests/test_utils.py
+-rw-r--r--   0 till      (1000) adm          (4)      582 2021-06-03 10:26:42.000000 cwepr-0.4.0/tox.ini
```

### Comparing `cwepr-0.3.0/CITATION.cff` & `cwepr-0.4.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/LICENSE` & `cwepr-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/PKG-INFO` & `cwepr-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwepr
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for handling cw-EPR data.
 Home-page: https://www.cwepr.de/
 Author: Mirjam Schröder, Pascal Kirchner, Till Biskup
 Author-email: till@till-biskup.de
 License: BSD
 Project-URL: Documentation, https://docs.cwepr.de/
 Project-URL: Source, https://github.com/tillbiskup/cwepr
```

### Comparing `cwepr-0.3.0/README.rst` & `cwepr-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/bin/incrementVersion.sh` & `cwepr-0.4.0/bin/incrementVersion.sh`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/analysis.py` & `cwepr-0.4.0/cwepr/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module containing the analysis steps of the cwEPR package.
+"""Module containing the analysis steps of the cwepr package.
 
 .. sidebar::
     processing *vs.* analysis
 
     For more details on the difference between processing and analysis,
     see the `ASpecD documentation <https://docs.aspecd.de/>`_.
 
@@ -13,14 +13,55 @@
 *e.g.*, in case of the signal-to-noise figure of a data trace, but as
 complicated as a (calculated) dataset on its own containing some measure as
 function of some parameter, such as the microwave frequency for each of a
 series of recordings, allowing to visualise drifts that may or may not
 impact data analysis.
 
 
+Concrete analysis steps
+=======================
+
+* :class:`FieldCalibration`
+
+  Determine offset value for a magnetic field calibration.
+
+* :class:`LinewidthPeakToPeak`
+
+  Peak to peak linewidth in derivative spectrum.
+
+* :class:`LinewidthFWHM`
+
+  Full linewidth at half maximum (FWHM).
+
+* :class:`SignalToNoiseRatio`
+
+  Get a spectrum's signal-to-noise ratio.
+
+* :class:`Amplitude`
+
+  Determine amplitude of dataset.
+
+* :class:`AmplitudeVsPower`
+
+  Return a calculated dataset to further analyse a power-sweep experiment.
+
+* :class:`FitOnData`
+
+  Perform polynomial fit on data and return its parameters or a dataset.
+
+* :class:`PtpVsModAmp`
+
+  Create calculated dataset for modulation sweep analysis.
+
+* :class:`AreaUnderCurve`
+
+  Make definite integration, i.e. calculate the area under the curve.
+
+
+
 Note to developers
 ==================
 
 Processing steps can be based on analysis steps, but not inverse! Otherwise,
 we get cyclic dependencies what should obviously be avoided in order to keep
 code working.
 
@@ -45,16 +86,16 @@
     the magnetic field values recorded are usually measured by a Hall probe
     or NMR teslameter away from the actual sample position. Hence,
     calibrating the recorded magnetic field value is necessary in case you
     are interested in quantitative *g*-value measurements or accurate
     comparisons between measurements.
 
     While spectrometers without removable probeheads (typically benchtop
-    devices) come often calibrated by the manufacturer, in the typical research
-    setup with probeheads and cryostats changing more frequent,
+    devices) come often calibrated by the manufacturer, in the typical
+    research setup with probeheads and cryostats changing more frequent,
     field calibration is typically performed by the individual researcher
     recording the EPR spectrum of a standard sample with known *g* value.
 
     Correcting the magnetic field axis of a recorded EPR spectrum is in such
     cases actually a two-step process:
 
     #. Obtain the magnetic field offset value from the EPR spectrum of a
@@ -109,15 +150,15 @@
             For valid values, see the table above.
 
         g_value : :class:`float`
             *g* value of the standard sample.
 
             If you provide a standard by name using the ``standard``
             parameter above, this is not necessary. Providing a value here
-            overrides the value for the standard. Hence use with care not to
+            overrides the value for the standard. Hence, use with care not to
             confuse you afterwards, when standard name and *g* value are
             inconsistent.
 
         mw_frequency : :class:`float`
             Microwave frequency to be corrected for.
 
             In general, this value is taken from the dataset and should
@@ -139,30 +180,31 @@
     Examples
     --------
     For convenience, a series of examples in recipe style (for details of
     the recipe-driven data analysis, see :mod:`aspecd.tasks`) is given below
     for how to make use of this class. The examples focus each on a single
     aspect.
 
-    Suppose you have recorded the spectrum of a Li:LiF field standard and
+    Suppose you have recorded the spectrum of a Li:LiF field standard, and
     now you would like to obtain the field offset to correct your other
     spectra:
 
     .. code-block:: yaml
 
         - kind: singleanalysis
           type: FieldCalibration
           properties:
             parameters:
               standard: LiLiF
           result: deltaB0
 
 
     This result can now be used within the same recipe to perform a field
-    correction of your other data. A more detailed example may look as follows:
+    correction of your other data. A more detailed example may look as
+    follows:
 
     .. code-block:: yaml
 
         datasets:
           - /path/to/LiLiF/dataset
             label: lilif
           - /path/to/my/first/dataset
@@ -270,17 +312,17 @@
             self.parameters['g_value'] = \
                 self.g_values[self.parameters['standard'].lower()]
 
     def _get_field_offset(self):
         """Calculates a field correction value.
 
         Finds the zero-crossing of a (derivative) spectrum of a field
-        standard by using the difference between minimum and maximum part of the
-        signal. This value is then subtracted from the the expected field
-        value for the MW frequency provided.
+        standard by using the difference between minimum and maximum part
+        of the signal. This value is then subtracted from the expected
+        field value for the MW frequency provided.
 
         Returns
         -------
         delta_b0: :class:`float`
             Field offset to be added to magnetic field axis of dataset(s)
 
         """
@@ -382,15 +424,16 @@
           result: linewidth
 
 
     """
 
     def __init__(self):
         super().__init__()
-        self.description = "Determine linewidth (full width at half max; FWHM)"
+        self.description = \
+            "Determine linewidth (full width at half max; FWHM)"
 
     @staticmethod
     def applicable(dataset):
         """
         Check whether analysis step is applicable to the given dataset.
 
         Line width detection can only be applied to 1D datasets.
@@ -430,27 +473,32 @@
         right_zero_cross_index = np.argmin(spectral_data[index_max:])
         b_field_left = self.dataset.data.axes[0].values[left_zero_cross_index]
         b_field_right = self.dataset.data.axes[0].values[right_zero_cross_index]
         return b_field_right - b_field_left
 
 
 class SignalToNoiseRatio(aspecd.analysis.SingleAnalysisStep):
-    """Get a spectrum's signal to noise ratio.
+    # noinspection PyUnresolvedReferences
+    """Get a spectrum's signal-to-noise ratio.
 
     This is done by comparing the absolute maximum of the spectrum to the
-    maximum of the edge part of the spectrum (i.e. a part which is considered
-    to not contain any signal.
+    maximum of the edge part of the spectrum (i.e. a part which is
+    considered to not contain any signal).
+
 
     Attributes
     ----------
-    parameters['percentage']: :class:`int`
-        percentage of the spectrum to be considered edge part on any side
-        (i.e. 10 % means 10 % on each side).
+    parameters : :class:`dict`
+        All parameters necessary for this step.
+
+        percentage : :class:`int`
+            percentage of the spectrum to be considered edge part on any
+            side  (i.e. 10 % means 10 % on each side).
 
-        Default: 10 %
+            Default: 10 %
 
     Examples
     --------
     The analysis can be applied either with or without the additional
     parameter "percentage":
 
     .. code-block:: yaml
@@ -466,15 +514,15 @@
 
     def __init__(self):
         super().__init__()
         self.parameters["percentage"] = 10
         self.description = "Determine signal to noise ratio."
 
     def _perform_task(self):
-        """Determine signal to noise ratio.
+        """Determine signal-to-noise ratio.
 
         Call method to get the amplitude of the noise, compare it to the
         absolute amplitude and set a result.
         """
         signal = self.dataset.data.data
         noise = self._get_noise()
 
@@ -494,15 +542,15 @@
                                self.dataset.data.data[-number_of_points:])
         return noise_data
 
 
 class Amplitude(aspecd.analysis.SingleAnalysisStep):
     """Determine amplitude of dataset.
 
-    Depending of the dimension of the dataset, the returned value is either
+    Depending on the dimension of the dataset, the returned value is either
     a scalar (1D dataset) or a vector (2D dataset) containing the amplitude of
     each row respectively.
 
     Returns
     -------
     result
         amplitude(s) row-wise, thus scalar or vector.
@@ -544,16 +592,16 @@
     -------
     result: :class:`aspecd.dataset.CalculatedDataset`
        Calculated Dataset where the data is the amplitude and the axis
        values is the root of the mw-power (in ascending order).
 
     Examples
     --------
-    For analysing a power sweep, extracting the amplitude and taking the root of
-    the microwave power is the first step to success (see
+    For analysing a power sweep, extracting the amplitude and taking the
+    root of the microwave power is the first step to success (see
     :ref:`power_sweep_analysis` for further details) and can be done as
     follows without additional parameters:
 
     .. code-block:: yaml
 
         - kind: singleanalysis
           type: AmplitudeVsPower
@@ -605,15 +653,16 @@
     function of the square root of the microwave power, the latter usually
     in mW), and a linear fit covering in this case the first five data points.
 
     """
 
     def __init__(self):
         super().__init__()
-        self.description = "Return calculated dataset for power sweep analysis."
+        self.description = \
+            "Return calculated dataset for power sweep analysis."
         self.result = aspecd.dataset.CalculatedDataset()
         # private properties
         self._analysis = None
         self._roots_of_mw_power = np.ndarray([])
 
     @staticmethod
     def applicable(dataset):
@@ -666,68 +715,79 @@
         elif self.dataset.data.axes[1].unit == 'W':
             self.result.data.axes[0].unit = 'sqrt(W)'
         self.result.data.axes[0].quantity = 'square root of mw power'
         self.result.data.axes[1].quantity = 'EPR amplitude'
 
 
 class FitOnData(aspecd.analysis.SingleAnalysisStep):
+    # noinspection PyUnresolvedReferences
     """Perform polynomial fit on data and return its parameters or a dataset.
 
     Developed tests first.
 
     Attributes
     ----------
     parameters : :class:`dict`
         All parameters necessary for this step.
 
-        points
-            first n points that should taken into account
+        points : :class:`int`
+            first n points that should be taken into account
 
             Default: 3
 
-        order
+        order : :class:`int`
             order of the fit.
 
             Default: 1
 
-        return_type : :class: `str`
+        return_type : :class:`str`
             Choose to returning the coefficients of the fit in order
-            of increasing degree or a calculated dataset containing the curve to
-            plot.
+            of increasing degree or a calculated dataset containing
+            the curve to plot.
 
             Default: coefficients.
 
             Valid values: 'coefficients', 'dataset'
 
-        add_origin : :class: `bool`
-            Adds the point (0,0) to the data and axes, but  does not guarantee
-            the fit really passes the origin.
+        fixed_intercept : :class:`bool`
+            Perform linear regression with fixed intercept, *i.e.*,
+            only fitting the slope.
+
+            To change the intercept from the origin, use the parameter
+            `offset`.
 
             Default: False.
 
+        offset : :class:`float`
+            Vertical offset of the data, *i.e.* f(0)
+
+            Useful in cases where the model defines an intercept f(0) != 0.
+
+            Default: 0
+
     Examples
     --------
-    Some Parameters can be chosen here, depending on the purpose and the
+    Some parameters can be chosen here, depending on the purpose and the
     following analysis and processing steps.
 
     .. code-block:: yaml
 
         - kind: singleanalysis
           type: FitOnData
           properties:
             parameters:
                 points: 5
                 order: 2
                 return_type: dataset
-                add_origin: True
+                fixed_intercept: True
           result: fit
 
     .. versionchanged:: 0.3
         Rewrite to perform fits with fixed intercept, remove parameter
-        "add_origin", introduced "fixed_intercerpt".
+        "add_origin", introduced "fixed_intercept".
         Return coefficients in order of increasing degree
 
     """
 
     def __init__(self):
         super().__init__()
         self.description = "Perform fit and return parameters."
@@ -787,20 +847,24 @@
     def _assign_result(self):
         if self.parameters['return_type'].lower() == 'dataset':
             self.result = self._curve
         else:
             self.result = self.parameters['coefficients']
 
     def _linear_regression_with_fixed_intercept(self):
+        _help = self.create_dataset()
+        _help.data.axes[0].values = \
+            self.dataset.data.axes[0].values[:self.parameters['points']]
+        _help.data.data = self.dataset.data.data[:self.parameters['points']]
         analysis = aspecd.analysis.LinearRegressionWithFixedIntercept()
         aspecd.utils.copy_values_between_dicts(source=self.parameters,
                                                target=analysis.parameters)
         analysis.parameters['polynomial_coefficients'] = True
-        analysis.dataset = self.dataset
-        result = self.dataset.analyse(analysis)
+        analysis.dataset = _help
+        result = _help.analyse(analysis)
         self.parameters['coefficients'] = result.result
 
 
 class PtpVsModAmp(aspecd.analysis.SingleAnalysisStep):
     """Create calculated dataset for modulation sweep analysis.
 
     For a modulation sweep analysis, the first step is to get the peak to
@@ -817,16 +881,16 @@
           type: PtpVsModAmp
           result: calc_dataset
 
     """
 
     def __init__(self):
         super().__init__()
-        self.description = 'Create dataset with ptp-linewidth vs modulation ' \
-                           'Amplitude.'
+        self.description = \
+            'Create dataset with ptp-linewidth vs modulation Amplitude.'
         self.result = aspecd.dataset.CalculatedDataset()
         self.linewidths = np.ndarray([])
 
     def _perform_task(self):
         self._get_linewidths()
         self._fill_dataset()
```

### Comparing `cwepr-0.3.0/cwepr/dataset.py` & `cwepr-0.4.0/cwepr/dataset.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/exceptions.py` & `cwepr-0.4.0/cwepr/exceptions.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/io/__init__.py` & `cwepr-0.4.0/cwepr/io/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,13 +30,14 @@
   Exporters, currently only an ASCII exporter
 
 
 """
 
 # The import statements below should *only* import the respective classes.
 from .factory import DatasetImporterFactory
-from .magnettech import MagnettechXMLImporter, GoniometerSweepImporter
-from .txt_file import TxtImporter
+from .magnettech import MagnettechXMLImporter, GoniometerSweepImporter, \
+    AmplitudeSweepImporter, PowerSweepImporter
+from .txt_file import TxtImporter, CsvImporter
 from .bes3t import BES3TImporter
 from .esp_winepr import ESPWinEPRImporter
 from .niehs import NIEHSDatImporter, NIEHSLmbImporter, NIEHSExpImporter
 from .exporter import ASCIIExporter, MetadataExporter
```

### Comparing `cwepr-0.3.0/cwepr/io/bes3t.py` & `cwepr-0.4.0/cwepr/io/bes3t.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     def __init__(self, source=None):
         super().__init__(source=source)
         self._metadata_dict = OrderedDict()
         self.load_infofile = True
         # private properties
         self._infofile = aspecd.infofile.Infofile()
-        self._dsc_dict = dict()
+        self._dsc_dict = {}
         self._mapper_filename = 'dsc_keys.yaml'
         self._is_two_dimensional = False
         self._dimensions = []
         self._file_encoding = ''
 
     def _import(self):
         self._clean_filenames()
```

### Comparing `cwepr-0.3.0/cwepr/io/dsc_keys.yaml` & `cwepr-0.4.0/cwepr/io/dsc_keys.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/io/esp_winepr.py` & `cwepr-0.4.0/cwepr/io/esp_winepr.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,18 +167,18 @@
         aspecd.utils.copy_values_between_dicts(metadata_dict,
                                                self._metadata_dict)
         self._extract_datetime()
 
     # TODO: Implement handling of "RT" in temperature value
     @staticmethod
     def _check_if_temperature_empty(metadata_dict):
-        print(metadata_dict['temperature_control'])
         if 'value'not in metadata_dict['temperature_control'][
-            'temperature'].keys() or metadata_dict['temperature_control'][
-                                     'temperature']['value'] == 0:
+            'temperature'].keys() or \
+                metadata_dict['temperature_control']['temperature']['value'] \
+                == 0:
             metadata_dict.pop('temperature_control')
         return metadata_dict
 
     def _extract_datetime(self):
         start_date = self._try_parsing_date()
         if 'measurement' not in self._metadata_dict.keys():
             self._metadata_dict['measurement'] = {}
@@ -225,20 +225,15 @@
             self.dataset.metadata.bridge.power.value *= 1e3
         self.dataset.metadata.bridge.power.unit = 'mW'
         # magnetic field objects
         objects_ = ('start', 'stop', 'sweep_width')
         for object_ in objects_:
             magnetic_field_object = getattr(
                 self.dataset.metadata.magnetic_field, object_)
-            if object_ in ('start', 'stop'):
-                if magnetic_field_object.value > 1500:
-                    magnetic_field_object.unit = 'G'
-                else:
-                    magnetic_field_object.unit = 'mT'
-            if magnetic_field_object.unit == 'G':
+            if magnetic_field_object.unit in ('G', ''):
                 magnetic_field_object.value /= 10
                 magnetic_field_object.unit = 'mT'
             setattr(
                 self.dataset.metadata.magnetic_field, object_,
                 magnetic_field_object)
         if not self.dataset.metadata.temperature_control.temperature.unit:
             self.dataset.metadata.temperature_control.temperature.unit = 'K'
@@ -262,12 +257,15 @@
         magnetic_field_axis = np.linspace(start, stop, points)
         assert len(magnetic_field_axis) == points, \
             'Length of magnetic field and number of points differ'
         assert len(magnetic_field_axis) == self.dataset.data.data.shape[0], \
             'Length of magnetic field and size of data differ'
         # set more values in dataset
         self.dataset.metadata.magnetic_field.stop.value = stop
+        self.dataset.metadata.magnetic_field.stop.unit = \
+            self.dataset.metadata.magnetic_field.start.unit
+
         self.dataset.data.axes[0].values = magnetic_field_axis
 
     def _get_number_of_points(self):
         self.dataset.metadata.magnetic_field.points = len(
             self.dataset.data.data)
```

### Comparing `cwepr-0.3.0/cwepr/io/exporter.py` & `cwepr-0.4.0/cwepr/io/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Exporters for both, whole datasets as well as data alone.
+"""Exporters for both, whole datasets and data alone.
 
 Exporters
 =========
 
 There are two different general types of exporters provided: Exporters for
 whole datasets i.e. data with their according metadata and exporters for data
 only.
```

### Comparing `cwepr-0.3.0/cwepr/io/factory.py` & `cwepr-0.4.0/cwepr/io/factory.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,20 +27,25 @@
     module, the standard importers from the ASpecD framework are checked.
     See the documentation of the :class:`aspecd.io.DatasetImporterFactory`
     base class for details.
 
     Attributes
     ----------
     supported_formats : :class:`dict`
-        Dictionary who's keys correspond to the base name of the respective
-        importer (*i.e.*, without the suffix "Importer") and who's values are a
+        Dictionary whose keys correspond to the base name of the respective
+        importer (*i.e.*, without the suffix "Importer") and whose values are a
         list of file extensions to detect the correct importer.
 
     data_format : :class:`str`
-        Name of the format that has been detected.
+        Name of the format that has been given or detected.
+
+    .. versionchanged:: 0.4
+        File extension is taken into account, so that two files with the same
+        name and different extension can reside next to each other and the
+        correct one is taken into account.
 
     """
 
     def __init__(self):
         super().__init__()
         self.supported_formats = {"BES3T": [".DTA", ".DSC"],
                                   "ESPWinEPR": [".spc", ".par"],
@@ -68,58 +73,89 @@
         Raises
         ------
         UnsupportedDataFormatError
             Raised if a format is set but does not match any of the supported
             formats
 
         """
-        self._cut_file_extension_if_necessary()
-        if os.path.isdir(self.source) and self._directory_contains_gon_data():
-            self.data_format = 'GoniometerSweep'
-            importer = \
-                object_from_class_name('cwepr.io.GoniometerSweepImporter')
-            importer.source = self.source
-            return importer
+        if os.path.isdir(self.source):
+            if self._directory_contains_gon_data():
+                self.data_format = 'GoniometerSweep'
+                importer = \
+                    object_from_class_name('cwepr.io.GoniometerSweepImporter')
+                importer.source = self.source
+                return importer
+            if self._directory_contains_amplitude_sweep_data():
+                self.data_format = 'AmplitudeSweep'
+                importer = \
+                    object_from_class_name('cwepr.io.AmplitudeSweepImporter')
+                importer.source = self.source
+                return importer
+            if self._directory_contains_power_sweep_data():
+                self.data_format = 'PowerSweep'
+                importer = \
+                    object_from_class_name('cwepr.io.PowerSweepImporter')
+                importer.source = self.source
+                return importer
         self.data_format = self._find_format()
-        importer = None
         if self.data_format:
             importer = object_from_class_name(
                 ".".join(["cwepr", "io", self.data_format + "Importer"]))
             importer.source = self.source
-        return importer
-
-    def _cut_file_extension_if_necessary(self):
-        for end_ in [extension for sublist in self.supported_formats.values()
-                     for extension in sublist]:
-            if self.source.endswith(end_):
-                self.source = self.source[:-len(end_)]
+            return importer
 
     def _find_format(self):
-        """Find out the format of the given file.
-
-        Determine the format of the given filename by checking if a data and
-        metadata file matching any supported format are present.
-
-        Determination is performed by checking if files with the correct name
-        and extension are present.
-        """
+        # detect extension
         detected_format = None
+        root, file_extension = os.path.splitext(self.source)
         for file_format, extensions in self.supported_formats.items():
             file_exists = []
-            for extension in extensions:
-                file_exists.append(os.path.isfile(self.source + extension))
-            if all(file_exists):
-                detected_format = file_format
+            if file_extension in extensions:
+                for extension in extensions:
+                    file_exists.append(os.path.isfile(root + extension))
+                if all(file_exists):
+                    detected_format = file_format
+            elif not file_extension:
+                for extension in extensions:
+                    file_exists.append(os.path.isfile(self.source + extension))
+                if all(file_exists):
+                    detected_format = file_format
         return detected_format
 
     def _directory_contains_gon_data(self):
         check_gon_filenames = []
         if not os.listdir(self.source):
             return False
         for element in os.listdir(self.source):
             if 'gon' in element:
                 check_gon_filenames.append(True)
             else:
                 check_gon_filenames.append(False)
         if all(check_gon_filenames):
             return True
         return False
+
+    def _directory_contains_amplitude_sweep_data(self):
+        check_modamp_filenames = []
+        if not os.listdir(self.source):
+            return False
+        for element in os.listdir(self.source):
+            if 'mod' in element:
+                check_modamp_filenames.append(True)
+            else:
+                check_modamp_filenames.append(False)
+        if all(check_modamp_filenames):
+            return True
+        return False
+
+    def _directory_contains_power_sweep_data(self):
+        check_powersweep_filenames = []
+        if not os.listdir(self.source):
+            return False
+        for element in os.listdir(self.source):
+            if 'pow' in element:
+                check_powersweep_filenames.append(True)
+            else:
+                check_powersweep_filenames.append(False)
+        if all(check_powersweep_filenames):
+            return True
+        return False
```

### Comparing `cwepr-0.3.0/cwepr/io/niehs.py` & `cwepr-0.4.0/cwepr/io/niehs.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,15 @@
         self._raw_metadata['sweep_width_mT'] = sweep_width = \
             self._raw_data[0] / 10
         self._raw_metadata['start'] = center_field - sweep_width / 2
         self._raw_metadata['stop'] = center_field + sweep_width / 2
         axis = np.linspace(center_field - sweep_width / 2,
                            center_field + sweep_width / 2,
                            num=number_points)
-        assert (axis[0] == center_field - sweep_width / 2)
+        assert axis[0] == center_field - sweep_width / 2
         self.dataset.data.axes[0].values = axis
 
     def _assign_units(self):
         self.dataset.data.axes[0].unit = 'mT'
 
     def _assign_some_metadata(self):
         self.dataset.metadata.magnetic_field.start.value = \
```

### Comparing `cwepr-0.3.0/cwepr/io/par_defaults.yaml` & `cwepr-0.4.0/cwepr/io/par_defaults.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/io/par_keys.yaml` & `cwepr-0.4.0/cwepr/io/par_keys.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/io/txt_file.py` & `cwepr-0.4.0/cwepr/io/txt_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 formats, as nearly every software to record data allows to export these data
 as simple text or CSV files.
 
 You may have a look as well at the importers provided by the ASpecD package
 for similar situations, particularly :class:`aspecd.io.TxtImporter`.
 
 """
+import io
 import numpy as np
 
 import aspecd.io
 
 
 class TxtImporter(aspecd.io.DatasetImporter):
     """Simple importer for txt files containing data.
@@ -30,38 +31,54 @@
         self.extension = '.txt'
 
     def _import(self):
         self._get_data()
         self._create_metadata()
 
     def _get_data(self):
+        if self.source.endswith('.txt'):
+            self.source = self.source[:-4]
+
         self.source = self.source + self.extension
         raw_data = np.loadtxt(self.source, delimiter='\t')
         self.dataset.data.data = raw_data[:, 1]
         self.dataset.data.axes[0].values = raw_data[:, 0]
 
     def _create_metadata(self):
         self.dataset.data.axes[0].unit = 'mT'
         self.dataset.data.axes[1].quantity = 'intensity'
 
 
 class CsvImporter(aspecd.io.DatasetImporter):
     """Importer for simple csv imports with different delimiters."""
 
     def __init__(self, source=''):
+        if source.endswith('.csv'):
+            source = source[:-4]
         super().__init__(source=source)
         # public properties
         self.extension = '.csv'
+        self.parameters["skiprows"] = 1
+        self.parameters["delimiter"] = None
+        self.parameters["comments"] = "#"
+        self.parameters["separator"] = None
 
     def _import(self):
         self._read_data()
 
     def _read_data(self):
-        with open(self.source + self.extension) as csv_file:
+        if "separator" in self.parameters:
+            separator = self.parameters.pop("separator")
+        else:
+            separator = None
+        if separator:
+            with open(self.source + self.extension, encoding="utf8") as file:
+                contents = file.read()
+            contents = contents.replace(separator, '.')
             # noinspection PyTypeChecker
-            raw_data = np.loadtxt(csv_file, delimiter=';', skiprows=3)
-            self.dataset.data.data = raw_data[:, 1]
-            self.dataset.data.axes[0].values = raw_data[:, 0]
+            data = np.loadtxt(io.StringIO(contents), **self.parameters)
+            self.dataset.data.data = data[:, 1]
+            self.dataset.data.axes[0].values = data[:, 0]
 
     def _create_metadata(self):
         self.dataset.data.axes[0].unit = 'mT'
         self.dataset.data.axes[1].quantity = 'intensity'
```

### Comparing `cwepr-0.3.0/cwepr/metadata.py` & `cwepr-0.4.0/cwepr/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 
 
 class ExperimentalDatasetMetadata(aspecd.metadata.ExperimentalDatasetMetadata):
     """Set of all metadata for a dataset object.
 
     Metadata as a unified structure of information coupled to the dataset are
     necessary for the understanding, analysis and processing of data,
-    especially in cwepr. Too many parameters have an direct influence to the
+    especially in cwepr. Too many parameters have a direct influence to the
     spectral shape of the spectrum that anything other than saving them in an
     appropriate place and accessing them automatised in the respective tasks
     is no option. Some parameters are written automatically by the
     spectrometer's software, others, depending also on the actual setup (that
-    may change over time!) are omitted and it is highly recommended those
-    should be noted by hand, for example in an *.info-file.*
+    may change over time!) are omitted. It is highly recommended those
+    parameters should be noted by hand, for example in an *.info-file.*
 
     Attributes
     ----------
     measurement: :class:`cwepr.metadata.Measurement`
         Metadata corresponding to the measurement.
 
     sample : :class:`cwepr.metadata.Sample`
@@ -86,14 +86,15 @@
         self.measurement = Measurement()
         self.experiment = Experiment()
         self.sample = Sample()
         self.spectrometer = Spectrometer()
         self.magnetic_field = MagneticField()
         self.bridge = Bridge()
         self.signal_channel = SignalChannel()
+        self.digital_filter = DigitalFilter()
         self.probehead = Probehead()
         self.temperature_control = TemperatureControl()
         self.metadata_modifications = []
 
 
 class CalculatedDatasetMetadata(aspecd.metadata.CalculatedDatasetMetadata):
     """Metadata for a calculated dataset.
@@ -468,15 +469,15 @@
         self.frequency_counter = ""
         self.mw_frequency = aspecd.metadata.PhysicalQuantity()
         self.q_value = 0
         super().__init__(dict_=dict_)
 
 
 class SignalChannel(aspecd.metadata.Metadata):
-    """Metadata information information on the signal channel employed.
+    """Metadata information on the signal channel employed.
 
     Parameters
     ----------
     dict_ : dict
         Dictionary containing fields corresponding to attributes of the class
 
     Attributes
@@ -523,14 +524,53 @@
         self.conversion_time = aspecd.metadata.PhysicalQuantity()
         self.time_constant = aspecd.metadata.PhysicalQuantity()
         self.phase = aspecd.metadata.PhysicalQuantity()
         self.offset = float()
         super().__init__(dict_=dict_)
 
 
+class DigitalFilter(aspecd.metadata.Metadata):
+    """Metadata about the digital filter applied to the data.
+
+    Especially in Magnettech data, by default, a digital filter is applied on
+    the data.
+
+    Parameters
+    ----------
+    dict_ : :class:`dict`
+        Dictionary containing properties to set.
+
+
+    Attributes
+    ----------
+    mode : :class:`str`
+        Mode of the digital filter. In Magnettech files, this is one of
+        "DIG" or "DIGRC".
+
+    points : :class:`int`
+        Number of points taken into account. Not used in Magnettech data.
+
+    parameter : :class:`aspecd.metadata.PhysicalQuantity`
+         In Magnettech data files, there are two different types of
+         parameters: In ``DIG`` mode the parameter is named "Smoothing
+         Filter width" and given in mT` whereas in ``DIGRC`` mode, it is the
+         "Time Constant" and given in `s`.
+
+
+    .. versionadded:: 0.4
+
+    """
+
+    def __init__(self, dict_=None):
+        self.mode = ""
+        self.points = ""
+        self.parameter = aspecd.metadata.PhysicalQuantity()
+        super().__init__(dict_=dict_)
+
+
 class Probehead(aspecd.metadata.Metadata):
     """Metadata corresponding to the probehead.
 
     Often, resonating structures get used in EPR spectroscopy, but as this
     is not always the case, the term "probehead" is more generic.
 
     In all except of fully integrated benchtop spectrometers, the probehead
@@ -547,15 +587,15 @@
 
 
     Attributes
     ----------
     type : :class:`str`
         Type of the probehead used.
 
-        There are several different types of probeheads regularly used. For
+        There are several types of probeheads regularly used. For
         resonators, there are, *e.g.*, dielectic and split-ring resonators,
         cylindrical and rectangular cavities. More special would be
         Fabry-Perot and stripline resonators. Sometimes, even resonator-free
         designs are used as probeheads.
 
     model : :class:`str`
         Model of the probehead used.
```

### Comparing `cwepr-0.3.0/cwepr/plotting.py` & `cwepr-0.4.0/cwepr/plotting.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/processing.py` & `cwepr-0.4.0/cwepr/processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 * :class:`Projection`
 
   Project data, *i.e.* reduce dimensions along one axis.
 
 * :class:`SliceExtraction`
 
-  Extract slice along one ore more dimensions from dataset.
+  Extract slice along one or more dimensions from dataset.
 
 * :class:`BaselineCorrection`
 
   Correct baseline of dataset.
 
 * :class:`Averaging`
 
@@ -151,15 +151,15 @@
     Usually, cwEPR spectra are not recorded with quadrature detection,
     *i.e.*, with both, absorptive and dispersive signal components. However,
     using the Hilbert transform, one can reconstruct the dispersive signal (
     imaginary component) and correct the phase of the microwave source this way.
 
   * Baseline correction
 
-    However careful measurements are performed, baselines are quite often
+    However, careful measurements are performed, baselines are quite often
     encountered. There are two different kinds of baseline that need to be
     corrected in different ways. Drifts of some kind can usually be handled
     by fitting and afterwards subtracting a (low-order) polynomial to the data.
 
     Particularly for low-temperature data, weak signals, and large magnetic
     field sweep ranges, resonator background can become quite dramatic.
     Here, usually the only viable way is to record the empty resonator
@@ -249,15 +249,15 @@
     intensity should be proportional to the number of spins in the active
     volume of the resonator/probehead. Therefore, with all crucial
     experimental parameters directly affecting the signal strength being
     equal (microwave power, modulation amplitude), normalising to same area
     should be the most straight-forward way of comparing two spectra in a
     meaningful way.
 
-    Bare in mind, however, that spectra with strongly different overall line
+    Bear in mind, however, that spectra with strongly different overall line
     width will have dramatically different minima and maxima, making
     comparison of this kind sometimes less meaningful.
 
 
 Besides these rather general ways of normalising spectra (although described
 above particularly with cwEPR data in mind), there are some other
 normalisations more particular to cwEPR spectroscopy:
@@ -279,15 +279,15 @@
     spectrometers is usually called) have usually a gain that can be
     adjusted to the signal strength of the actual sample. Of course,
     this setting will have a direct impact on the intensity values recorded (
     usually something like mV).
 
     Comparing spectra recorded with different receiver gain settings
     therefore requires the user to *first* normalise the data to the same
-    receiver gain setting. Otherwise, (semi-)quantiative comparison is not
+    receiver gain setting. Otherwise, (semi-)quantitative comparison is not
     possible and will lead to wrong conclusions.
 
     Note on the side: Adjusting the receiver gain for each measurement is
     highly recommended, as setting it too high will make the signal clip and
     distort the signal shape, and setting it too low will result in data
     with (unnecessary) poor signal-to-noise ratio.
 
@@ -303,15 +303,15 @@
 
 There are, however, other types of 2D datasets that are quite useful in
 cwEPR spectroscopy. Some vendors of EPR spectrometers offer no simple way of
 saving each individual scan in a series of accumulations. However, this may
 sometimes be of interest, particularly as a single "spike" due to some
 external event or other malfunctioning may otherwise ruin your entire
 dataset, however long it might have taken to record it. Therefore, one way
-around this limitations is to perform a 2D experiment with repeated field
+around this limitation is to perform a 2D experiment with repeated field
 scans, but saving each scan as a row in a 2D dataset.
 
 Generally, there are at least two different processing steps of interest for
 2D datasets:
 
   * Projection along one axis
 
@@ -425,16 +425,17 @@
    :keyprefix: proc-
 
 
 Module documentation
 ====================
 
 What  follows is the API documentation of each class implemented in this module.
-
 """
+import warnings
+
 import numpy as np
 import scipy.integrate
 import scipy.interpolate
 import scipy.signal
 
 import aspecd.processing
 from cwepr import utils
@@ -445,15 +446,16 @@
 
     Perform a linear field correction of the data with a correction value
     previously determined.
 
     Attributes
     ----------
     parameters['offset']: :class:`float`
-        Offset to be added to the field axis values.
+        Offset to be added to the field axis values. Should be given in the
+        unit of the axis.
 
 
     See Also
     --------
     cwepr.analysis.FieldCalibration :
         Determine offset value for a magnetic field calibration
 
@@ -471,51 +473,113 @@
     def _perform_task(self):
         """Shift all field axis data points by the correction value."""
         for axis in self.dataset.data.axes:
             # TODO: Question: Better check for quantity rather than unit?
             #       (Difficult if not filled)
             # if axis.quantity == 'magnetic field'
             if axis.unit in ('mT', 'G'):
-                self.dataset.data.axes[0].values += \
-                    self.parameters["offset"]
+                axis.values += self.parameters["offset"]
+                self.dataset.metadata.magnetic_field.start.value = \
+                    axis.values[0]
+                self.dataset.metadata.magnetic_field.stop.value = \
+                    axis.values[-1]
 
 
 class FrequencyCorrection(aspecd.processing.SingleProcessingStep):
     """Convert data of a given frequency to another given frequency.
 
     This is used to make spectra comparable.
+    There are two methods for frequency correction which has to be given
+    in the parameter section.
+
+    * calculation via the Zeeman splitting (proportional)
+
+      All magnetic field points will be recalculated to keep their g-value.
+      This preserves field-dependent interactions such as *g* anisotropy,
+      but artificially scales all field-independent shifts. HFI or ZFS
+      constants are not preserved.
+
+    * Addition of an offset value (offset)
+
+      As the EPR spectrum should be somewhat centered to the signal of
+      interest, the central point will be corrected for the new frequency.
+      The difference between the old and the new magnetic field will be added
+      onto all other magnetic field points. Preserves constant energy shifts
+      such as (first order) HFI or ZFS, but artificially scales
+      field-dependent interactions such as *g* anisotropy. *g* factors besides
+      the reference point are not preserved. (Thanks to B. Corzilius for the
+      input)
+
+    Examples
+    --------
+    .. code-block:: yaml
+
+       - kind: processing
+         type: FrequencyCorrection
+         properties:
+           parameters:
+             kind: proportional
+             frequency: 9.63
+
 
     Attributes
     ----------
     self.parameters['frequency']
         Frequency to correct for.
 
         Default: 9.5
 
+    self.parameters['kind']
+        Method used for frequency correction. Can be ``offset`` or
+        ``proportional``.
+
+        Default: proportional
+
+
+    .. versionchanged:: 0.4
+        Choice between the two methods of  frequency correction
+
     """
 
     def __init__(self):
         super().__init__()
         self.parameters["frequency"] = 9.5
+        self.parameters['kind'] = 'proportional'
         self.description = "Correct magnetic field axis for given frequency"
 
+    @staticmethod
+    def applicable(dataset):
+        """Check applicability."""
+        if not dataset.metadata.bridge.mw_frequency.value:
+            message = 'No frequency given in dataset'
+            warnings.warn(message=message)
+            return False
+        return True
+
+    def _sanitise_parameters(self):
+        if isinstance(self.parameters['frequency'], int):
+            self.parameters['frequency'] = float(self.parameters['frequency'])
+
     def _perform_task(self):
         """Perform the actual transformation / correction."""
         nu_target = self.parameters['frequency']
         for axis in self.dataset.data.axes:
             # TODO: Question: Better check for quantity rather than unit?
             #       (Difficult if not filled)
             # if axis.quantity == 'magnetic field'
             if axis.unit in ('mT', 'G'):
-                axis.values = self._correct_field_for_frequency(nu_target,
-                                                                axis.values)
+                if 'proportional' in self.parameters['kind'].lower():
+                    axis.values = self._correct_proportionally(nu_target,
+                                                               axis.values)
+                elif 'offset' in self.parameters['kind'].lower():
+                    axis.values = self._correct_with_offset(nu_target,
+                                                            axis.values)
                 self._write_new_frequency()
 
-    def _correct_field_for_frequency(self, nu_target=None,
-                                     b_initial=None):
+    def _correct_proportionally(self, nu_target=None, b_initial=None):
         """
         Calculate new field axis for given frequency.
 
         Parameters
         ----------
         nu_target : :class:`float`
             Frequency the magnetic field should be computed for
@@ -529,14 +593,21 @@
             Computed field axis
 
         """
         nu_initial = self.dataset.metadata.bridge.mw_frequency.value
         b_target = (nu_target / nu_initial) * b_initial
         return b_target
 
+    def _correct_with_offset(self, nu_target=None, axis=None):
+        point_to_correct = axis[round(len(axis) / 2)]
+        nu_initial = self.dataset.metadata.bridge.mw_frequency.value
+        offset = point_to_correct - (nu_target / nu_initial) * point_to_correct
+        b_target = axis + offset
+        return b_target
+
     def _write_new_frequency(self):
         self.dataset.metadata.bridge.mw_frequency.value = \
             self.parameters['frequency']
 
 
 class GAxisCreation(aspecd.processing.SingleProcessingStep):
     """Change magnetic field axis to *g* axis.
@@ -644,15 +715,15 @@
 
     def _find_best_phase(self):
         min_angle = -np.pi / 2
         max_angle = np.pi / 2
         # TODO: introduce parameter step width/number of points.
         angles = np.linspace(min_angle, max_angle, num=181)
         for angle in angles:
-            rotated_signal = (np.exp(1j * angle) * self._analytic_signal)
+            rotated_signal = np.exp(1j * angle) * self._analytic_signal
             if self.parameters['order'] > 0:
                 # pylint: disable=unused-variable
                 for j in range(self.parameters['order']):
                     rotated_signal = scipy.integrate.cumtrapz(rotated_signal,
                                                               initial=0)
             rotated_signal = self._baseline_correction(signal=np.real(
                 rotated_signal))
@@ -985,15 +1056,15 @@
     This will project the data along the second axis (index 1), yielding a 1D
     dataset.
 
     """
 
 
 class SliceExtraction(aspecd.processing.SliceExtraction):
-    """Extract slice along one ore more dimensions from dataset.
+    """Extract slice along one or more dimensions from dataset.
 
     As the class is fully inherited from ASpecD for simple usage, see the
     ASpecD documentation of the :class:`aspecd.processing.SliceExtraction`
     class for details.
 
     Examples
     --------
@@ -1092,15 +1163,15 @@
          type: BaselineCorrection
 
     In this case, a zeroth-order polynomial baseline will be subtracted from
     your dataset using ten percent to the left and right, and in case of a
     2D dataset, the baseline correction will be performed along the first
     axis (index zero) for all indices of the second axis (index 1).
 
-    Of course, often you want to control a little bit more how the baseline
+    Of course, often you want to control a little more how the baseline
     will be corrected. This can be done by explicitly setting some parameters.
 
     Suppose you want to perform a baseline correction with a polynomial of
     first order:
 
     .. code-block:: yaml
```

### Comparing `cwepr-0.3.0/cwepr/report.py` & `cwepr-0.4.0/cwepr/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,17 @@
 class ExperimentalDatasetLaTeXReporter(aspecd.report.LaTeXReporter):
     """Report implementation for cwepr module."""
 
     def __init__(self, template='', filename=''):
         super().__init__(template=template, filename=filename)
         self.dataset = cwepr.dataset.ExperimentalDataset()
         # private properties
-        self._metadata = dict()
+        self._metadata = {}
         self._tasks = collections.OrderedDict()
-        self._figure_name = dict()
+        self._figure_name = {}
         self._exclude_from_to_dict.extend(['dataset'])
 
     def create(self):
         """Perform all methods to generate a report."""
         self._prepare_metadata()
         self._get_tasks()
         self._get_figure_names()
@@ -167,15 +167,15 @@
             elif not value:
                 tmp_dict.pop(key)
         dict_ = tmp_dict
         return dict_
 
     def _get_figure_names(self):
         """Get the names of the figures used for the report."""
-        for i in range(len(self.dataset.representations)):
+        for i, _ in enumerate(self.dataset.representations):
             if self.dataset.representations[i].plot.description \
                     == '2D plot as scaled image.':
                 self._figure_name['Figure2D'] = \
                     self.dataset.representations[i].plot.filename
             elif self.dataset.representations[i].plot.description \
                     == '1D line plot.':
                 self._figure_name['Figure1D'] = \
@@ -187,16 +187,16 @@
 class PowerSweepAnalysisReporter(aspecd.report.LaTeXReporter):
     """Create report for power sweep analysis."""
 
     def __init__(self, template='', filename=''):
         super().__init__(template=template, filename=filename)
         self.dataset = cwepr.dataset.ExperimentalDataset()
         # private properties
-        self._metadata = dict()
-        self._tasks = dict()
+        self._metadata = {}
+        self._tasks = {}
         self._exclude_from_to_dict.extend(['dataset'])
 
     def create(self):
         """Perform all methods to generate a report.
 
         .. todo::
             Do not rely on dataset from recipe properties but use the dataset
@@ -272,16 +272,16 @@
     def __init__(self, template='', filename=''):
         self.filename = filename
         self.language = 'de'
         self.template = template if template else self._get_template()
         super().__init__(template=self.template, filename=self.filename)
         self.dataset = cwepr.dataset.ExperimentalDataset()
         # private properties
-        self._metadata = dict()
-        self._figure_name = dict()
+        self._metadata = {}
+        self._figure_name = {}
         self._exclude_from_to_dict.extend(['dataset'])
 
     def create(self):
         """Perform all methods to create captions."""
         self._prepare_metadata()
         self._create_context()
         super().create()
```

### Comparing `cwepr-0.3.0/cwepr/templates/de/DokuwikiCaption.txt.jinja` & `cwepr-0.4.0/cwepr/templates/de/DokuwikiCaption.txt.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/de/modulation_sweep_analysis_report.tex.jinja` & `cwepr-0.4.0/cwepr/templates/de/modulation_sweep_analysis_report.tex.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/de/power_sweep_report.tex.jinja` & `cwepr-0.4.0/cwepr/templates/de/power_sweep_report.tex.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/de/report.tex.jinja` & `cwepr-0.4.0/cwepr/templates/de/report.tex.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/en/DokuwikiCaption.txt.jinja` & `cwepr-0.4.0/cwepr/templates/en/DokuwikiCaption.txt.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/en/Infofile.info.jinja` & `cwepr-0.4.0/cwepr/templates/en/Infofile.info.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/en/power_sweep_report_generic.tex.jinja` & `cwepr-0.4.0/cwepr/templates/en/power_sweep_report_generic.tex.jinja`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/report/latex/de/kolophon.tex` & `cwepr-0.4.0/cwepr/templates/report/latex/de/kolophon.tex`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/report/latex/de/metadaten_experimentell.tex` & `cwepr-0.4.0/cwepr/templates/report/latex/de/metadaten_experimentell.tex`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/report/latex/en/colophon.tex` & `cwepr-0.4.0/cwepr/templates/report/latex/en/colophon.tex`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/templates/report/latex/en/metadata_experimental.tex` & `cwepr-0.4.0/cwepr/templates/report/latex/en/metadata_experimental.tex`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr/utils.py` & `cwepr-0.4.0/cwepr/utils.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/cwepr.egg-info/PKG-INFO` & `cwepr-0.4.0/cwepr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwepr
-Version: 0.3.0
+Version: 0.4.0
 Summary: Package for handling cw-EPR data.
 Home-page: https://www.cwepr.de/
 Author: Mirjam Schröder, Pascal Kirchner, Till Biskup
 Author-email: till@till-biskup.de
 License: BSD
 Project-URL: Documentation, https://docs.cwepr.de/
 Project-URL: Source, https://github.com/tillbiskup/cwepr
```

### Comparing `cwepr-0.3.0/cwepr.egg-info/SOURCES.txt` & `cwepr-0.4.0/cwepr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 cwepr/io/__init__.py
 cwepr/io/bes3t.py
 cwepr/io/dsc_keys.yaml
 cwepr/io/esp_winepr.py
 cwepr/io/exporter.py
 cwepr/io/factory.py
 cwepr/io/magnettech.py
+cwepr/io/magnettech_keys.yaml
 cwepr/io/niehs.py
 cwepr/io/par_defaults.yaml
 cwepr/io/par_keys.yaml
 cwepr/io/txt_file.py
 cwepr/templates/de/DokuwikiCaption.txt.jinja
 cwepr/templates/de/modulation_sweep_analysis_report.tex.jinja
 cwepr/templates/de/power_sweep_report.tex.jinja
```

### Comparing `cwepr-0.3.0/docs/CalculatedDataset.yaml` & `cwepr-0.4.0/docs/CalculatedDataset.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/ExperimentalDataset.yaml` & `cwepr-0.4.0/docs/ExperimentalDataset.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/Makefile` & `cwepr-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/_templates/page.html` & `cwepr-0.4.0/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/_templates/versions.html` & `cwepr-0.4.0/docs/_templates/versions.html`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/api/index.rst` & `cwepr-0.4.0/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/audience.rst` & `cwepr-0.4.0/docs/audience.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/changelog.rst` & `cwepr-0.4.0/docs/changelog.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,66 @@
 =========
 Changelog
 =========
 
 This page contains a summary of changes between the official cwepr releases. Only the biggest changes are listed here. A complete and detailed log of all changes is available through the `GitHub Repository Browser <https://github.com/tillbiskup/cwepr/commits/master>`_.
 
-Version 0.3
+Version 0.4.0
+=============
+
+Released 2023-07-15
+
+**Note:** Starting with this version, cwepr requires **ASpecD >= 0.8.0**.
+
+New features
+------------
+
+* Add Frequency Correction with offset: This keeps the hyperfine splitting values.
+
+* Amplitude sweep importer for Magnettech. Averaging of temperature and Q-Values of the single measurements. A warning is issued if the values vary too much.
+
+* Implement Digital Filter into metadata.
+
+* Data is imported according to its file extension specified in the recipe.
+
+* Added support for cwepr-infofile version 0.1.5
+
+* Handling of data from Magnettech-Files: The filtered first derivative spectrum is taken by its name by default. The parameter can be set to also import other data curves such as the second derivative or the sinus part.
+
+
+Changes
+-------
+
+* Extend cw-EPR primer: additional notes on recording spectra
+
+
+Fixes
+-----
+
+* Fix bug in analysis.FitOnData by using a helper dataset.
+
+* Fix some metadata in magnettech importer (experiment.runs -> signal_channel.accumulations, correctly import spectrometer metadata, bring time stamp to same timezone.)
+
+* Do range extraction and interpolation (instead of interpolation only) in GoniometerSweepImporter.
+
+* Fix FieldCorrection to update correct axis and update metadata.
+
+* Win-EPR importer makes less mistakes in guessing the unit of the field axis.
+
+
+
+Version 0.3.0
 =============
 
 Released 2022-07-24
 
 New features
 ------------
 
-* Add linear fit with fixed intercept to FitOnData, renamed function accordingly. (0719809a22)
+* Add linear fit with fixed intercept to FitOnData, renamed function accordingly.
 * Importer for NIEHS dat, lmb, and exp files
 
 
 Version 0.2.1
 =============
 
 Released 2022-06-12
```

### Comparing `cwepr-0.3.0/docs/concepts.rst` & `cwepr-0.4.0/docs/concepts.rst`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
 *Information on cw-EPR data(sets), can exist separately from datasets.*
 
 Metadata are stored outside the cwepr package in simple yet structured text files that focus on human readability and writability, while retaining machine readability.
 
 The simplest incarnation of metadata is all necessary information obtained during data acquisition that usually gets stored in a file and read upon data import. A `dataset`_ contains these metadata together with the numerical data.
 
+For more details, see the separate page on :doc:`metadata during data acquisition <metadata>`.
+
 
 History
 =======
 
 *Complete list of all processing steps, allows for reproducibility.*
 
 Reproducibility is an essential aspect of good scientific practice. In the context of data processing and analysis, this means that each processing step performed on data (of a dataset) should be stored in an reproducible way and preferably in a consistent format.
```

### Comparing `cwepr-0.3.0/docs/conf.py` & `cwepr-0.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     'python': ('https://docs.python.org/3', None),
     'numpy': ('https://numpy.org/doc/stable/', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference/', None),
+    'scipy': ('https://docs.scipy.org/doc/scipy/', None),
     'matplotlib': ('https://matplotlib.org/stable/', None),
     'aspecd': ('https://docs.aspecd.de/', None),
 }
 
 # -- Options for todo extension ----------------------------------------------
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
```

### Comparing `cwepr-0.3.0/docs/cwepr/analysis.rst` & `cwepr-0.4.0/docs/cwepr/analysis.rst`

 * *Files 1% similar despite different names*

```diff
@@ -45,16 +45,16 @@
 
 Comparing cw-EPR spectra
 ========================
 
 What is normally considered a simple task, comparing two or more recorded cw-EPR spectra, is much more tricky than one might think at first. Of course, the procedure taken depends dramatically on the ultimate goal of comparing as well. If you would like to do a semi-quantitative comparison of a series of spectra, you need to take different things into account as if you are interested in comparing spectral shapes.
 
 
-Semi-quantiative analysis
--------------------------
+Semi-quantitative analysis
+--------------------------
 
 Suppose you have recorded a series of cw-EPR spectra of different samples and would like to compare them in a semi-quantitative way, *i.e.* only with respect to their relative intensities. Note that this is different from spin quantification. For details of the latter, see below.
 
 There are a number of experimental parameters that influence the signal intensity as recorded by your spectrometer, and that need to be known for any meaningful comparison:
 
   * Microwave power
   * Modulation amplitude
@@ -62,15 +62,15 @@
   * Time constant/conversion time
   * Q value
 
 While you can numerically account for microwave power, receiver gain, and Q value, the other parameters better be set identical during recording. And of course, microwave power and receiver gain need to be in a range that does not saturate your signal or clip the detector, respectively.
 
 The absolute intensity values are usually arbitrary units and thus not comparable at all between different setups. The same is true for different resonators within the same spectrometer. Positioning of the resonator between the pole tips of your magnet influences the signal intensity as well, although probably to a smaller extent. Measuring with and without cryostat, however, will certainly make a more dramatic difference.
 
-Suppose you have recorded all samples with identical experimental settings, and you are reasonably confident that the resulting spectra are neither saturated nor over-modulated nor clipped nor otherwise distorted. If you forgot to record the Q value, you cannot reliably do a semi-quantiative analysis, at least not if you would like to do better than an order-of-magnitude estimation.
+Suppose you have recorded all samples with identical experimental settings, and you are reasonably confident that the resulting spectra are neither saturated nor over-modulated nor clipped nor otherwise distorted. If you forgot to record the Q value, you cannot reliably do a semi-quantitative analysis, at least not if you would like to do better than an order-of-magnitude estimation.
 
 If all requirements are reasonably fulfilled, the next step is to doubly integrate your spectra recorded with the usual lock-in detection scheme. Sounds simple, is mathematically well-defined, but in reality often rather tricky. These steps usually need to be carried out:
 
   * Baseline correction (at least 0th order)
   * 1st integration
   * Visual inspection of the resulting absorptive spectrum
   * Baseline correction (1st order)
@@ -96,14 +96,16 @@
   * Area under curve
 
     (Note: For first-derivative spectra, the area under the curve is *not* identical to the number of spins contributing to the signal!)
 
 You should, however, never simply plot the spectra "as is" and start interpreting some overlapping parts in some way. This would mean that you implicitly perform a semi-quantitative analysis, and this is in this way most certainly wrong. For details why this is the case and how to do better, see above.
 
 
+.. _spin_quantification:
+
 Spin quantification
 ===================
 
 Quantitative EPR is a field on its own. There is an excellent book on the topic authored by the Eatons that is highly recommended for everybody interested in performing quantitative EPR of any kind (not only spin quantification, but as well accurate measurements of *g* values).
 
 If you happen to have access to a calibrated commercial spectrometer, spin counting of samples at room temperature that consist of only one species may be quite straight-forward, given that you managed to record your data accurately, with minimum phase error and baseline. The latter points are highly important, as spin counting involves integrating the spectra. If all these conditions are met, it may be as simple as running some built-in routine of the measurement control software.
```

### Comparing `cwepr-0.3.0/docs/cwepr/index.rst` & `cwepr-0.4.0/docs/cwepr/index.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/cwepr/processing.rst` & `cwepr-0.4.0/docs/cwepr/processing.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/cwepr/recording.rst` & `cwepr-0.4.0/docs/cwepr/recording.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 ========================
 Recording cw-EPR spectra
 ========================
 
 What is the usual way of recording cw-EPR spectra of an unknown sample?
 
-To obtain data that can be properly post-processed and analysed, the signal should not be distorted by either saturation or overmodulation, and it should be as good as possible in terms of its signal-to-noise ratio.
+To obtain data that can be properly post-processed and analysed, the signal should not be distorted by either saturation or overmodulation, and it should be as good as possible in terms of its signal-to-noise ratio. Unfortunately, this means that **you generally need to optimise parameters for each individual sample**, or at least for each individual series of similar samples (in terms of paramagnetic species, solvent, tube dimensions, and temperature). Of course, there are some "informed guesses" for parameters to start from, but don't fool yourself using these parameters without checking whether you accidentally distort your EPR signal.
 
 Furthermore, if you would like to compare spectra among each other, you will need to ensure that you calibrate your field, usually by recording the spectrum of a sample with known *g* factor (commonly referred to as "field standard") or have it properly calibrated (*e.g.*, once by a technician upon setting up the spectrometer in your lab).
 
 
 .. note::
     Basic familiarity with operating an EPR spectrometer is tacitly assumed. You will find no information how to couple your resonator and similar things, as this strongly depends on the setup you're using.
 
 
+Metadata
+========
+
+Before delving into how to optimise the parameters of a cw-EPR experiment, we need to briefly mention an important but too often overlooked or ignored aspect: **recording all relevant metadata during data acquisition**. In short: no spectrometer will record all relevant metadata for you automatically, and some will sometimes even record wrong parameters. Hence, make it a habit to *always* record all relevant metadata *during data acquisition* in a format that can be directly read by the cwepr package. This is both, a matter of convenience for you when later processing and analysing the data, and a prerequisite for reproducible research and hence integral part of the scientific method.
+
+.. important::
+
+    Note that most commercial **EPR spectrometers do not record sufficient metadata** for full reproducibility. What is even worse: some tend to write **wrong parameter values**, as they do not read the parameter values from the devices when the measurement starts/finishes, but only when the operator manually triggers the saving. Hence, you better record crucial metadata by hand in an *external* file -- and understand which values to trust and why.
+
+
+For further details, see the section on :doc:`metadata during data acquisition <../metadata>` in the user manual.
+
+
 Field range
 ===========
 
-How to know over which field range to sweep? The answer strongly depends on the kind of sample you're measuring. Organic radicals usually show rather narrow signals of 5-10 mT centred about a *g* value of *g* = 2. Metals are a completely different thing. They have often quite broad spectra and can easily have g values in the range of 1.9-4 and beyond.
+How to know over which field range to sweep? The answer strongly depends on the kind of sample you're measuring. Organic radicals usually show rather narrow signals of 5-10 mT centred about a *g* value of *g* = 2. Metals are a completely different thing. They have often quite broad spectra and can easily have g values in the range of 1.9--4 and beyond.
 
 In any case, make sure to record enough "baseline" left and right of your actual signal. Beware of your signal having Lorentzian shape. In this case, you will have very broad "wings" with very little intensity, hence need to record quite a bit of "baseline" not to truncate your spectrum. Furthermore, if you plan to correct the phase of your spectra afterwards, having the spectra recorded rather broad is particularly important, as the dispersive component is quite broad as well.
 
-From own experience, people usually tend to record data over a far too narrow field range.
+From own experience, people usually tend to record data over a far too narrow field range. For example: if your signal appears to be 5--10 mT wide, as typical for an organic radical, you better record a range of 15--20 mT, assuming a finite Lorentzian contribution to your linewidth.
 
 
 Microwave power: power sweep
 ============================
 
-What microwave power to use? Obviously, more is not always better, as you may easily saturate your signals, resulting in broadening that you cannot easily correct for afterwards. Besides that, it strongly depends on your setup what microwave power will yield reasonable results.
+What microwave power to use? Obviously, more is not always better, as you may easily saturate your signals, resulting in broadening that you cannot easily correct for afterwards. Besides that, it strongly depends on your setup what microwave power will yield reasonable results. For organic radicals at ambient temperatures, microwave powers of 1--2 mW will usually be a good first guess.
+
+From a physical point of view, the spin relaxation times determine the microwave power required to saturate your sample. These spin relaxation times or rates are generally temperature-dependent: the lower the temperature, the longer the spin-relaxation time. Furthermore, high-spin systems with *S*>1/2 generally have shorter spin relaxation times due to spin-spin interactions, resulting in higher microwave power required to saturate your signal. Organic radicals usually have *S*\ =1/2 and hence have rather long relaxation times. This means that it is rather simple to saturate the signal of an organic radical, particularly at lower temperatures (*i.e.* in solid state/frozen solution).
 
 The only way to really know what setting to use to not distort your signal shape is to perform a series of measurements with different microwave power settings. This is colloquially known as "power sweep".
 
 As 3 dB change in attenuation translates to a factor of 2 in microwave power, 3-dB steps for a power sweep are quite common.
 
 How such power sweep is analysed will be described in more detail later. For now just one important comment:
 
@@ -75,15 +90,15 @@
 Signal channel settings
 =======================
 
 Depending on the type of setup you use, you will usually have to deal with two parameters: conversion time and time constant.
 
 The conversion time is the time the digitizer in the signal channel spends on acquiring signal on every magnetic field point, and is therefore directly connected to the total sweep time for one scan and the number of field points to record. Generally, the longer you set your conversion time, the better your signal-to-noise ratio will become. However, this has some intrinsic limitations. One is the overall stability of your setup that might make it favourable to use shorter conversion times and more individual scans. Another is the lifetime of the paramagnetic species you are interested in. If you are measuring transient species with a limited lifetime, your conversion time should be short compared to the signal change, and if you would like to not only record the signal change on a single magnetic field position, but acquire complete spectra, it should even be much shorter, at least by the factor of field points you record for a single spectrum.
 
-The time constant, on the other hand, acts as a filter to reduce the noise on the acquired signal. Therefore, larger time constants will generally lead to less noisy spectra. However, this filtering comes to a price, and you need to ensure not to accidentially filter your signal and hence distort its line shape. Usually, you will find advice in the literature to set the time constant at least a factor of four smaller than the conversion time, and at least a factor of ten smaller than it takes to pass through the narrowest line of your spectrum. In any case, the value for the time constant should be *smaller* than that of the conversion time. If in doubt, your best bet will usually be to try it out using a sample with decent signal strength, and make sure the signal shape does not change at all when increasing the time constant, at least not beyond available spectrometer accuracy and repeatability.
+The time constant, on the other hand, acts as a filter to reduce the noise on the acquired signal. Therefore, larger time constants will generally lead to less noisy spectra. However, this filtering comes to a price, and you need to ensure not to accidentally filter your signal and hence distort its line shape. Usually, you will find advice in the literature to set the time constant at least a factor of four smaller than the conversion time, and at least a factor of ten smaller than it takes to pass through the narrowest line of your spectrum. In any case, the value for the time constant should be *smaller* than that of the conversion time. If in doubt, your best bet will usually be to try it out using a sample with decent signal strength, and make sure the signal shape does not change at all when increasing the time constant, at least not beyond available spectrometer accuracy and repeatability.
 
 
 Digital filters
 ===============
 
 Modern spectrometers come equipped with digital signal processing capabilities that are often switched on by default. While generally, there is nothing wrong with digital signal processing, and the EPR community can probably learn a lot from the concepts developed in this (engineering) field decades ago and applied in probably more devices we're using daily than we can imagine, scientists should usually strive for signals that are as much unprocessed as possible.
 
@@ -105,12 +120,32 @@
 
 
 Recording each scan independently
 =================================
 
 Usually, you will need to record more than one scan to obtain a sufficient signal-to-noise ratio of your signal. The exception proves the rule.
 
-One problem with recording multiple scans can be that many spectrometers average the scans immediately, not saving the individual scans. This is fine as long as everything goes smooth. However, having personal experience with an environment where you frequently obtain random noise from unknown sources resulting in narrow spikes in your spectra, we strongly recommend saving each scan individually wherever possible.
+One problem with recording multiple scans can be that many spectrometers average the scans immediately, not saving the individual scans. This is fine as long as everything goes smoothly. However, having personal experience with an environment where you frequently obtain random noise from unknown sources resulting in narrow spikes in your spectra, we strongly recommend saving each scan individually wherever possible.
 
-Some spectrometers do this *per se*, with others, such as Bruker spectrometers, you can usually perform "field delay" measurements and set the delay to a very short time. A "field delay" measurement is kind of a kinetic experiment where you repeatedly perform a convential field sweep experiment and save the results as individual rows of a two-dimensional dataset. In this case, all information regarding other parameters of the setup, such as the microwave frequency, that may change during the measurement, are nevertheless lost.
+Some spectrometers do this *per se*, with others, such as Bruker spectrometers, you can usually perform "field delay" measurements and set the delay to a very short time. A "field delay" measurement is kind of a kinetic experiment where you repeatedly perform a conventional field sweep experiment and save the results as individual rows of a two-dimensional dataset. In this case, all information regarding other parameters of the setup, such as the microwave frequency, that may change during the measurement, are nevertheless lost.
 
 Of course, having recorded 2D datasets instead of the usual 1D datasets makes it less convenient to look at the data, as you first need to average over the second dimension. However, given a software package like cwepr, this can pretty easily be dealt with.
+
+
+Sample concentration and number of spins
+========================================
+
+A last factor that definitely determines the quality of the signals you can record is the number of spins present in your sample. Generally, you may be tempted to think that more is better. However, beware of the fact that at higher concentrations, paramagnetic centres are such densely packed that the spins start to "see" each other and couple via both, dipolar and exchange interactions. This generally leads to distortions of your lines.
+
+As a rule of thumb, a 100 uM solution of TEMPO or similar nitroxide spin probe is perfectly fine, and a TEMPO solution of > 1 mM will be inappropriate due to strong spin-spin interactions visible as strongly broadened signals.
+
+On the other end of the scale, the question often arises how many spins you can detect using a conventional cw-EPR spectrometer. Again, the fair answer would be: it depends on the resonator you use and the overall setup and its sensitivity. Furthermore, keep in mind that sensitivity is usually given as spins per field unit (G or mT). The reason for this is obvious: Sensitivity depends on the absolute signal height, but the height of the signal of a paramagnetic species strongly depends on the spectral width, as the integral and not the amplitude is proportional to the number of spins. Typical figures for commercial EPR spectrometers are in the range of 10^10 to 10^11 spins per Gauss. If you are interested in performing quantitative EPR measurements to obtain the absolute number of spins in your sample, have a look at the section on :ref:`spin quantification <spin_quantification>` in the data analysis section.
+
+
+I don't see a signal: what now?
+===============================
+
+More often than not, you will not see an EPR signal of your unknown sample on first try. However, this does not necessarily mean that there is no EPR signal. Make sure that your spectrometer works and that you did not accidentally made a mistake or set a parameter to a wrong value. You can easily check that your spectrometer works and that you operate it correctly by measuring a sample that you know will give a signal.
+
+EPR standards are a good choice for checking the spectrometer to work correctly, but if you happen to not have access to such a standard sample, coal (from a burned match) or even coffee powder may do well. A freshly prepared solution of TEMPO or some similar nitroxide spin probe will do fine as well. Just make sure to *not* dissolve it in water or some other solvent with high relative permittivity (dielectric constant), as this will make your dip disappear. Hint: If you dissolve TEMPO or similar in DMSO, you need to use a thin tube, as with a 4 mm tube, you won't manage to tune your resonator.
+
+If the spectrometer works and the standard sample you measured does show its known signal, there still might be the chance that the other conditions are just not right. If you have high-spin systems, you will usually need to go to rather low temperatures to see an EPR signal at all. As a rule of thumb, Fe-S clusters frequently found in proteins do show up only below 80 K, typically at about 10--20 K.
```

### Comparing `cwepr-0.3.0/docs/cwepr-favicon.ico` & `cwepr-0.4.0/docs/cwepr-favicon.ico`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/cwepr-logo.png` & `cwepr-0.4.0/docs/cwepr-logo.png`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/dataset-structure.rst` & `cwepr-0.4.0/docs/dataset-structure.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/developers.rst` & `cwepr-0.4.0/docs/developers.rst`

 * *Files 6% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 To install the necessary Python dependencies, create a virtual environment, e.g., with ``virtualenv <environment>``, and activate it afterwards with ``<environment>/bin/activate``. Then install the dependencies using ``pip``:
 
 
 .. code-block:: bash
 
     pip install sphinx
-    pip install sphinx-rtd-theme
+    pip install sphinx-rtd-theme sphinxcontrib-bibtex sphinx-multiversion
 
 
 To build the documentation:
 
     * Activate the virtual environment where the necessary dependencies are installed in.
     * ``cd`` to ``docs/``, then run ``make html``. (To clean previously built documentation, run ``make clean`` first).
 
@@ -121,14 +121,20 @@
 
 
 .. code-block:: bash
 
     pip install prospector[all]
     pip install prospector[with_pyroma]
 
+Some shells (such as Zsh, the default shell of macOS Catalina) require brackets to be escaped:
+
+.. code-block:: bash
+
+    pip install prospector\[with_pyroma\]
+
 
 The optional arguments ensure that all necessary dependencies are installed as well.
 
 Afterwards, simply run Prospector from a terminal from within your project root:
 
 
 .. code-block:: bash
```

### Comparing `cwepr-0.3.0/docs/examples/first-overview.rst` & `cwepr-0.4.0/docs/examples/first-overview.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/examples/index.rst` & `cwepr-0.4.0/docs/examples/index.rst`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,33 @@
 
 Here, we present a (growing) series of working examples of how to use the cwepr package to perform both, day-to-day routine tasks in a laboratory working with cw-EPR spectroscopy as well as more complex processing and analysis tasks.
 
 For each of the examples, a full recipe is provided ready to be copied and pasted and run on your local computer.
 
 .. note::
 
-    There are plans to provide a series of real example data as well, to make it easy to get first-hand experience with the cwepr package.
+    For each of the recipes provided so far, the cwepr package (at least its `repository on GitHub <https://github.com/tillbiskup/cwepr>`_) contains the real example data as well. Therefore, you can download the data and recipe to get first-hand experience with the cwepr package.
 
 
 Prerequisites
 =============
 
 To be able to run the example recipes locally, you need to have a working installation of the cwepr package and its dependencies. Have a look at the :doc:`installation instructions <../installing>` for details.
 
 Furthermore, to be able to run ("cook") the recipes and get ("serve") the results, you need to have access to a command line, as running recipes (still) is command-line based using the command :samp:`serve {recipe.yaml}`.
 
-For some recipes, you will need to have a working LaTeX installation in case you would like to get your reports not only created, but compiled into a well-formatted PDF document as well.
+**Optional:** For some recipes, you will need to have a working LaTeX installation in case you would like to get your reports not only created, but compiled into a well-formatted PDF document as well.
 
+
+.. note::
+
+    The path to the data in the recipes assumes the directory layout of the cwepr package. Hence, the easiest way is to clone or download the repository from `GitHub <https://github.com/tillbiskup/cwepr>`_, change into the ``examples`` directory and there into the respective subdirectory and run the corresponding recipe.
+
+
+Further examples
+================
+
+If you are interested in more examples, the :ref:`publication describing the cwepr package <sec-how_to_cite>` contains a number of examples of different complexity. The complete recipes are provided in the supporting information (SI). What is even better: You can download the entire set of data and corresponding recipes from GitHub:
+
+* `EPR data and analysis for Schröder and Biskup, J. Magn. Reson. 335:107140, 2022 <https://github.com/tillbiskup/2022-jmr-data>`_
+
+  GitHub repository containing both, data and recipes for all the examples shown in the :ref:`publication describing the cwepr package <sec-how_to_cite>`.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cwepr-0.3.0/docs/examples/power-sweep-analysis.rst` & `cwepr-0.4.0/docs/examples/power-sweep-analysis.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/index.rst` & `cwepr-0.4.0/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    :target: https://doi.org/10.5281/zenodo.4896687
    :align: right
 
 ===================
 cwepr documentation
 ===================
 
-Welcome! This is the documentation for cwepr, a Python package for **processing and analysis of continuous-wave electron paramagnetic resonance (cw-EPR) spectra** based on the `ASpecD framework <https://www.aspecd.de/>`_. For general information see its `Homepage <https://www.cwepr.de/>`_. Due to the inheritance from the ASpecD framework, all data generated with the cwepr package are completely reproducible and have a complete history.
+Welcome! This is the documentation for cwepr, a Python package for **processing and analysis of continuous-wave electron paramagnetic resonance (cw-EPR) spectra** based on the `ASpecD framework <https://www.aspecd.de/>`_. For general information see its `Homepage <https://www.cwepr.de/>`_. Due to the inheritance from the ASpecD framework, all data generated with the cwepr package are **completely reproducible** and have a complete history.
 
 What is even better: Actual data processing and analysis **no longer requires programming skills**, but is as simple as writing a text file summarising all the steps you want to have been performed on your dataset(s) in an organised way. Curious? Have a look at the following example:
 
 
 .. code-block:: yaml
     :linenos:
 
@@ -77,22 +77,33 @@
 * Extensive user and API documentation
 
 
 .. warning::
   The cwepr package is currently under active development and still considered in Beta development state. Therefore, expect frequent changes in features and public APIs that may break your own code. Nevertheless, feedback as well as feature requests are highly welcome.
 
 
+Requirements
+============
+
+The cwepr package comes with a rather minimal set of requirements:
+
+* Python >= 3.7 with aspecd, numpy, scipy and matplotlib packages
+* command-line access for :doc:`recipe-driven data analysis <usecases>`
+* :doc:`metadata <metadata>` (in addition to the usual parameter files)
+* EPR data in readable formats (details in the :mod:`cwepr.io` (sub)package)
+
+
 .. _sec-how_to_cite:
 
 How to cite
 ===========
 
 cwepr is free software. However, if you use cwepr for your own research, please cite both, the article describing it and the software itself:
 
-  * Mirjam Schröder, Till Biskup. cwepr -- a Python package for analysing cw-EPR data focussing on reproducibility and simple usage. *Journal of Magnetic Resonance* **335**:107140, 2022. `doi:10.1016/j.jmr.2021.107140 <https://doi.org/10.1016/j.jmr.2021.107140>`_
+  * Mirjam Schröder, Till Biskup. cwepr -- a Python package for analysing cw-EPR data focussing on reproducibility and simple usage. *Journal of Magnetic Resonance* **335**:107140, 2022. `doi:10.1016/j.jmr.2021.107140 <https://doi.org/10.1016/j.jmr.2021.107140>`_ | `PDF <https://www.till-biskup.de/_media/de/person/schr-jmr-335-107140-accepted.pdf>`_ | `SI <https://www.till-biskup.de/_media/de/person/schr-jmr-335-107140-si.pdf>`_
 
   * Mirjam Schröder, Till Biskup. cwepr (2021). `doi:10.5281/zenodo.4896687 <https://doi.org/10.5281/zenodo.4896687>`_
 
 To make things easier, cwepr has a `DOI <https://doi.org/10.5281/zenodo.4896687>`_ provided by `Zenodo <https://zenodo.org/>`_, and you may click on the badge below to directly access the record associated with it. Note that this DOI refers to the package as such and always forwards to the most current version.
 
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4896687.svg
    :target: https://doi.org/10.5281/zenodo.4896687
@@ -116,14 +127,20 @@
 .. code-block:: bash
 
     pip install cwepr
 
 Have a look at the more detailed :doc:`installation instructions <installing>` as well.
 
 
+Actual use cases
+================
+
+The cwepr Python package has been used already for analysing published cwepr data, and for some, the data and recipes have been published as "data publications". See the list of :doc:`data publications <examples/data-publications>` for further details.
+
+
 Related projects
 ================
 
 There is a number of related packages users of the cwepr package may well be interested in, as they have a similar scope, focussing on spectroscopy and reproducible research.
 
 * `ASpecD <https://docs.aspecd.de/>`_
 
@@ -147,14 +164,15 @@
    :maxdepth: 2
    :caption: User Manual:
    :hidden:
 
    audience
    introduction
    concepts
+   metadata
    usecases
    installing
 
 
 .. toctree::
    :maxdepth: 2
    :caption: cw-EPR Primer:
@@ -169,14 +187,15 @@
 .. toctree::
    :maxdepth: 2
    :caption: Examples:
    :hidden:
 
    examples/index
    examples/list
+   examples/data-publications
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Developers:
    :hidden:
```

### Comparing `cwepr-0.3.0/docs/installing.rst` & `cwepr-0.4.0/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/introduction.rst` & `cwepr-0.4.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/literature.bib` & `cwepr-0.4.0/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/make.bat` & `cwepr-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/people.rst` & `cwepr-0.4.0/docs/people.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/docs/usecases.rst` & `cwepr-0.4.0/docs/usecases.rst`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/setup.py` & `cwepr-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Development Status :: 4 - Beta",
         "Topic :: Scientific/Engineering",
     ],
     install_requires=[
-        'aspecd>=0.6.3',
+        'aspecd>=0.8.0',
         'numpy',
         'scipy',
         'matplotlib',
     ],
     extras_require={
         'dev': ['prospector'],
         'docs': ['sphinx', 'sphinx-rtd-theme', 'sphinxcontrib-bibtex'],
```

### Comparing `cwepr-0.3.0/tests/io/test_bes3t.py` & `cwepr-0.4.0/tests/io/test_bes3t.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/test_esp_winepr.py` & `cwepr-0.4.0/tests/io/test_esp_winepr.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/test_exporter.py` & `cwepr-0.4.0/tests/io/test_exporter.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/test_factory.py` & `cwepr-0.4.0/tests/io/test_factory.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,34 +21,43 @@
 
     def test_goniometer_importer_gets_correct_files(self):
         source = os.path.join(ROOTPATH, 'testdata', 'magnettech-goniometer/')
         importer = cwepr.dataset.DatasetFactory().importer_factory
         importer.get_importer(source=source)
         self.assertEqual('GoniometerSweep', importer.data_format)
 
+    def test_powersweep_importer_gets_correct_files(self):
+        source = os.path.join(ROOTPATH, 'testdata', 'magnettech-power/')
+        importer = cwepr.dataset.DatasetFactory().importer_factory
+        importer.get_importer(source=source)
+        self.assertEqual('PowerSweep', importer.data_format)
+
     def test_goniometer_importer_does_not_import_inconsistent_data(self):
         source = os.path.join(ROOTPATH, 'testdata', 'magnettech-goniometer/')
         with tempfile.TemporaryDirectory() as tmpdir:
             new_source = os.path.join(tmpdir, 'new')
-            shutil.copytree(source, new_source)
-            list_element = os.listdir(new_source)[2]
-            source_name = os.path.join(new_source, list_element)
-            target_name = os.path.join(new_source, 'fake_name')
-            os.rename(source_name, target_name)
             importer = cwepr.dataset.DatasetFactory().importer_factory
             importer.get_importer(source=new_source)
             self.assertNotEqual('MagnettechXML', importer.data_format)
 
-    def test_factory_cuts_filename(self):
+    def test_factory_detects_extension(self):
         source = os.path.join(ROOTPATH, 'testdata', 'test-magnettech.xml')
         factory = cwepr.dataset.DatasetFactory()
         importer_factory = factory.importer_factory
         importer_factory.get_importer(source=source)
         root_source, _ = os.path.splitext(source)
-        self.assertEqual(root_source, importer_factory.source)
+        self.assertEqual(importer_factory.data_format, 'MagnettechXML')
+
+    def test_factory_without_extension_returns(self):
+        source = os.path.join(ROOTPATH, 'testdata', 'test-magnettech')
+        factory = cwepr.dataset.DatasetFactory()
+        importer_factory = factory.importer_factory
+        importer_factory.get_importer(source=source)
+        root_source, _ = os.path.splitext(source)
+        self.assertEqual(importer_factory.data_format, 'MagnettechXML')
 
     def test_with_adf_extension_returns_adf_importer(self):
         source = 'test.adf'
         importer = self.factory.get_importer(source=source)
         self.assertIsInstance(importer, aspecd.io.AdfImporter)
 
     def test_niehsdat_file_returns_correct_importer(self):
```

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.DSC` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.DTA` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DFieldSweep.info` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DFieldSweep.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.DSC` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.DTA` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-1DTimeSweep.info` & `cwepr-0.4.0/tests/io/testdata/BDPA-1DTimeSweep.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.DSC` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.DTA` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldDelay.info` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldDelay.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.DSC` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.DTA` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DFieldPower.info` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DFieldPower.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.DSC` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.DTA` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/BDPA-2DTimeField.info` & `cwepr-0.4.0/tests/io/testdata/BDPA-2DTimeField.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/EMX-winEPR.info` & `cwepr-0.4.0/tests/io/testdata/EMX-winEPR.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/EMX-winEPR.spc` & `cwepr-0.4.0/tests/io/testdata/EMX-winEPR.spc`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/ESP.info` & `cwepr-0.4.0/tests/io/testdata/ESP.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/ESP.spc` & `cwepr-0.4.0/tests/io/testdata/ESP.spc`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120018656_goniometersweep-testdata_F_gon_0dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120018656_goniometersweep-testdata_F_gon_0dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120054089_goniometersweep-testdata_F_gon_10dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120054089_goniometersweep-testdata_F_gon_10dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120129135_goniometersweep-testdata_F_gon_20dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120129135_goniometersweep-testdata_F_gon_20dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120204063_goniometersweep-testdata_F_gon_30dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120204063_goniometersweep-testdata_F_gon_30dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120238999_goniometersweep-testdata_F_gon_40dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120238999_goniometersweep-testdata_F_gon_40dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120314263_goniometersweep-testdata_F_gon_50dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120314263_goniometersweep-testdata_F_gon_50dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120349297_goniometersweep-testdata_F_gon_60dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120349297_goniometersweep-testdata_F_gon_60dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120424603_goniometersweep-testdata_F_gon_70dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120424603_goniometersweep-testdata_F_gon_70dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120500130_goniometersweep-testdata_F_gon_80dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120500130_goniometersweep-testdata_F_gon_80dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120536148_goniometersweep-testdata_F_gon_90dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120536148_goniometersweep-testdata_F_gon_90dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120611356_goniometersweep-testdata_F_gon_100dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120611356_goniometersweep-testdata_F_gon_100dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120646202_goniometersweep-testdata_F_gon_110dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120646202_goniometersweep-testdata_F_gon_110dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120721430_goniometersweep-testdata_F_gon_120dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120721430_goniometersweep-testdata_F_gon_120dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120756411_goniometersweep-testdata_F_gon_130dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120756411_goniometersweep-testdata_F_gon_130dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120831365_goniometersweep-testdata_F_gon_140dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120831365_goniometersweep-testdata_F_gon_140dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120906619_goniometersweep-testdata_F_gon_150dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120906619_goniometersweep-testdata_F_gon_150dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_120941813_goniometersweep-testdata_F_gon_160dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_120941813_goniometersweep-testdata_F_gon_160dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_121017977_goniometersweep-testdata_F_gon_170dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_121017977_goniometersweep-testdata_F_gon_170dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer/20201216_121054028_goniometersweep-testdata_F_gon_180dg.xml` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer/20201216_121054028_goniometersweep-testdata_F_gon_180dg.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/magnettech-goniometer.info` & `cwepr-0.4.0/tests/io/testdata/magnettech-goniometer.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/modulation-amplitude-analysis.yaml` & `cwepr-0.4.0/tests/io/testdata/modulation-amplitude-analysis.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/noisy_data.txt` & `cwepr-0.4.0/tests/io/testdata/noisy_data.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/not_noisy_data.txt` & `cwepr-0.4.0/tests/io/testdata/not_noisy_data.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/phase-45_noise0.000.txt` & `cwepr-0.4.0/tests/io/testdata/phase-45_noise0.000.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/phase-45_noise0.000_small.txt` & `cwepr-0.4.0/tests/io/testdata/phase-45_noise0.000_small.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/phase-45_noise0.100.txt` & `cwepr-0.4.0/tests/io/testdata/phase-45_noise0.100.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/phase_shift.txt` & `cwepr-0.4.0/tests/io/testdata/phase_shift.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/power-sweep-analysis.yaml` & `cwepr-0.4.0/tests/io/testdata/power-sweep-analysis.yaml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/sinus_baseline.txt` & `cwepr-0.4.0/tests/io/testdata/sinus_baseline.txt`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DSC` & `cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DSC`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DTA` & `cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.DTA`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/test-bes3t-1D-fieldsweep.info` & `cwepr-0.4.0/tests/io/testdata/test-bes3t-1D-fieldsweep.info`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/test-magnettech.info` & `cwepr-0.4.0/tests/io/testdata/test-magnettech.info`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cwEPR Info file - v. 0.1.3 (2016-01-18)
+cwEPR Info file - v. 0.1.5 (2023-03-24)
 
 GENERAL
 Filename:               test-magnettech
 Date start:             2020-11-12
 Date end:               2020-11-12
 Time start:             9:50:00
 Time end:               10:20:00
@@ -51,24 +51,36 @@
 SIGNAL CHANNEL
 Model:                  Magnettech built-in
 Modulation amplifier:   Magnettech built-in
 Accumulations:          1
 Modulation frequency:   10 kHz
 Modulation amplitude:   0.001 mT
 Receiver gain:          N/A
+Offset:                 N/A
 Conversion time:        N/A
 Time constant:          N/A
 Phase:                  0 deg
 
+DIGITAL FILTER
+Mode:                   DIG
+Number of Points:       N/A
+Parameter:              0.01 mT
+
+GONIOMETER
+Start:                  0 deg
+Increment:              10 deg
+Number of Points:       19
+Fine Tuning per Slice:  off
+
 PROBEHEAD
 Type:                   rectangular TE102
 Model:                  Magnettech built-in
 Coupling:               critical
 
 TEMPERATURE
 Temperature:            293 K
 Controller:             N/A
 Cryostat:               N/A
 Cryogen:                N/A
 
 COMMENT
-Booh!
+Booh!
```

### Comparing `cwepr-0.3.0/tests/io/testdata/test-magnettech.xml` & `cwepr-0.4.0/tests/io/testdata/test-magnettech.xml`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/io/testdata/winepr.spc` & `cwepr-0.4.0/tests/io/testdata/winepr.spc`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/test_analysis.py` & `cwepr-0.4.0/tests/test_analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
     def test_fixed_offset_with_offset_non_zero(self):
         self.dataset.data.data = np.asarray([1.4, 2, 3, 4, 5, 6])
         self.dataset.data.axes[0].values = np.asarray([0.5, 1, 2, 3, 4, 5])
         self.analysator.parameters['fixed_intercept'] = True
         self.analysator.parameters['offset'] = 1
         res = self.dataset.analyse(self.analysator)
-        self.assertAlmostEqual(res.result[1], 1, 2)
+        self.assertAlmostEqual(res.result[1], 1, 1)
         self.assertEqual(res.result[0], 1)
 
     def test_fixed_offset_with_offset_zero_return_pol_coeffs(self):
         self.dataset.data.data = np.asarray([0.45, 1, 2, 3, 4, 5])
         self.dataset.data.axes[0].values = np.asarray([0.5, 1, 2, 3, 4, 5])
         self.analysator.parameters['fixed_intercept'] = True
         self.analysator.parameters['polynomial_coefficients'] = True
```

### Comparing `cwepr-0.3.0/tests/test_dataset.py` & `cwepr-0.4.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/test_plotting.py` & `cwepr-0.4.0/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/test_processing.py` & `cwepr-0.4.0/tests/test_processing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,51 @@
 import copy
 import os
 import unittest
 
+import aspecd.metadata
 import aspecd.exceptions
 import numpy as np
+import numpy.testing as testing
 
 import cwepr.exceptions
 import cwepr.processing
 import cwepr.dataset
 import cwepr.io.magnettech
 
 ROOTPATH = os.path.split(os.path.abspath(__file__))[0]
 
 
+class TestFieldCorrection(unittest.TestCase):
+    def setUp(self):
+        source = os.path.join(ROOTPATH, 'io/testdata/test-magnettech')
+        importer = cwepr.io.magnettech.MagnettechXMLImporter(source=source)
+        self.dataset = cwepr.dataset.ExperimentalDataset()
+        self.dataset.import_from(importer)
+
+    def test_axis_is_updated(self):
+        fc = cwepr.processing.FieldCorrection()
+        fc.parameters['offset'] = 10
+        axis_before = copy.deepcopy(self.dataset.data.axes[0].values)
+        self.dataset.process(fc)
+        axis_after = self.dataset.data.axes[0].values
+        testing.assert_equal(axis_before + 10, axis_after)
+
+    def test_metadata_is_updated(self):
+        fc = cwepr.processing.FieldCorrection()
+        fc.parameters['offset'] = 10
+        start = copy.deepcopy(self.dataset.metadata.magnetic_field.start.value)
+        stop = copy.deepcopy(self.dataset.metadata.magnetic_field.stop.value)
+        self.dataset.process(fc)
+        self.assertGreater(self.dataset.metadata.magnetic_field.start.value,
+                           start)
+        self.assertGreater(self.dataset.metadata.magnetic_field.stop.value,
+                           stop)
+
+
 class TestAutomaticPhaseCorrection(unittest.TestCase):
     def setUp(self):
         source = os.path.join(ROOTPATH, 'io/testdata/phase-45_noise0.000')
         importer = cwepr.io.txt_file.TxtImporter(source=source)
         self.dataset = cwepr.dataset.ExperimentalDataset()
         self.dataset.import_from(importer)
 
@@ -55,24 +84,87 @@
     def test_frequency_before_is_different_from_after(self):
         old_freq = copy.deepcopy(self.dataset.metadata.bridge.mw_frequency)
         self.corrector.parameters['frequency'] = 9.5
         self.dataset.process(self.corrector)
         new_freq = self.dataset.metadata.bridge.mw_frequency
         self.assertNotEqual(new_freq.value, old_freq.value)
 
+    def test_frequency_given_as_int(self):
+        old_freq = copy.deepcopy(self.dataset.metadata.bridge.mw_frequency)
+        self.corrector.parameters['frequency'] = 9
+        self.dataset.process(self.corrector)
+        new_freq = self.dataset.metadata.bridge.mw_frequency
+        self.assertNotEqual(new_freq.value, old_freq.value)
+
+    def test_no_frequency_given(self):
+        self.dataset.metadata.bridge.mw_frequency = \
+            aspecd.metadata.PhysicalQuantity()
+        with self.assertRaises(aspecd.exceptions.NotApplicableToDatasetError):
+            self.dataset.process(self.corrector)
+
     def test_magnetic_field_axis_is_different(self):
         old_field_axis = copy.deepcopy(
             self.dataset.data.axes[0].values)
         self.corrector.parameters['frequency'] = 8.
         self.dataset.process(self.corrector)
         new_field_axis = self.dataset.data.axes[0].values
         diffs = old_field_axis - new_field_axis
         conditions = (diff == 0 for diff in diffs)
         self.assertFalse(all(conditions))
 
+    def test_magnetic_field_points_have_non_constant_offset(self):
+        old_field_axis = copy.deepcopy(
+            self.dataset.data.axes[0].values)
+        self.corrector.parameters['frequency'] = 8.
+        self.dataset.process(self.corrector)
+        new_field_axis = self.dataset.data.axes[0].values
+        diffs = old_field_axis - new_field_axis
+        self.assertTrue(diffs[0] != diffs[-1])
+
+    def test_correct_with_offset_writes_new_magnetic_field_values(self):
+        old_field_axis = copy.deepcopy(
+            self.dataset.data.axes[0].values)
+        self.corrector.parameters['frequency'] = 8.5
+        self.corrector.parameters['kind'] = 'offset'
+        self.dataset.process(self.corrector)
+        new_field_axis = self.dataset.data.axes[0].values
+        diffs = old_field_axis - new_field_axis
+        conditions = (diff == 0 for diff in diffs)
+        self.assertFalse(all(conditions))
+
+    def test_correct_with_offset_center_point_is_lower_than_before(self):
+        old_field_axis = copy.deepcopy(
+            self.dataset.data.axes[0].values)
+        self.corrector.parameters['frequency'] = 8.5
+        self.corrector.parameters['kind'] = 'offset'
+        self.dataset.process(self.corrector)
+        new_field_axis = self.dataset.data.axes[0].values
+        idx = round(len(old_field_axis) / 2)
+        old_point = old_field_axis[idx]
+        new_point = new_field_axis[idx]
+        self.assertTrue(old_point < new_point)
+
+    def test_correct_with_offset_writes_new_frequency(self):
+        old_freq = copy.deepcopy(self.dataset.metadata.bridge.mw_frequency)
+        self.corrector.parameters['kind'] = 'offset'
+        self.corrector.parameters['frequency'] = 8.5
+        self.dataset.process(self.corrector)
+        new_freq = self.dataset.metadata.bridge.mw_frequency
+        self.assertNotEqual(new_freq.value, old_freq.value)
+
+    def test_correct_with_offset_field_points_have_constant_offset(self):
+        old_field_axis = copy.deepcopy(
+            self.dataset.data.axes[0].values)
+        self.corrector.parameters['kind'] = 'offset'
+        self.corrector.parameters['frequency'] = 8.5
+        self.dataset.process(self.corrector)
+        new_field_axis = self.dataset.data.axes[0].values
+        diffs = old_field_axis - new_field_axis
+        self.assertTrue(len(np.unique(diffs)) == 1)
+
 
 class GAxisCreation(unittest.TestCase):
     def setUp(self):
         self.proc = cwepr.processing.GAxisCreation()
         self.dataset = cwepr.dataset.ExperimentalDataset()
         self.dataset.data.data = np.random.random(100)
         self.dataset.data.axes[0].values = np.linspace(300, 400, num=100)
@@ -153,38 +245,39 @@
         importer = cwepr.dataset.DatasetFactory()
         self.dataset = importer.get_dataset(source=source)
 
     def test_normalisation_to_receiver_gain(self):
         correction = cwepr.processing.Normalisation()
         correction.parameters['kind'] = 'receiver_gain'
         before = max(self.dataset.data.data)
-        rg = 10**(self.dataset.metadata.signal_channel.receiver_gain.value /20)
+        rg = 10 ** (
+                self.dataset.metadata.signal_channel.receiver_gain.value / 20)
         self.dataset.process(correction)
         after = max(self.dataset.data.data)
-        self.assertEqual(before/rg, after)
+        self.assertEqual(before / rg, after)
 
     def test_normalisation_to_scan_number(self):
         correction = cwepr.processing.Normalisation()
         correction.parameters['kind'] = 'scan_number'
         before = max(self.dataset.data.data)
         scans = self.dataset.metadata.signal_channel.accumulations
         self.dataset.process(correction)
         after = max(self.dataset.data.data)
-        self.assertEqual(before/scans, after)
+        self.assertEqual(before / scans, after)
 
     def test_normalisation_to_maximum(self):
         correction = cwepr.processing.Normalisation()
         correction.parameters['kind'] = 'max'
         before = np.max(self.dataset.data.data)
         max_ = max(self.dataset.data.data)
         self.dataset.process(correction)
         after = max(self.dataset.data.data)
-        self.assertEqual(before/max_, after)
+        self.assertEqual(before / max_, after)
 
     def test_normalisation_to_minimum(self):
         correction = cwepr.processing.Normalisation()
         correction.parameters['kind'] = 'min'
         before = min(self.dataset.data.data)
         min_ = min(self.dataset.data.data)
         self.dataset.process(correction)
         after = min(self.dataset.data.data)
-        self.assertEqual(before/abs(min_), after)
+        self.assertEqual(before / abs(min_), after)
```

### Comparing `cwepr-0.3.0/tests/test_report.py` & `cwepr-0.4.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tests/test_utils.py` & `cwepr-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cwepr-0.3.0/tox.ini` & `cwepr-0.4.0/tox.ini`

 * *Files identical despite different names*

