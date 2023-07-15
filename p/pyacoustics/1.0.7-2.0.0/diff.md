# Comparing `tmp/pyacoustics-1.0.7.tar.gz` & `tmp/pyacoustics-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyacoustics-1.0.7.tar", last modified: Sun Aug  8 11:44:06 2021, max compression
+gzip compressed data, was "pyacoustics-2.0.0.tar", last modified: Sat Jul 15 16:22:52 2023, max compression
```

## Comparing `pyacoustics-1.0.7.tar` & `pyacoustics-2.0.0.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.746020 pyacoustics-1.0.7/
--rw-r--r--   0 tmahrt     (501) staff       (20)       28 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/MANIFEST.in
--rw-r--r--   0 tmahrt     (501) staff       (20)     6286 2021-08-08 11:44:06.745652 pyacoustics-1.0.7/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     4687 2019-12-08 15:31:04.000000 pyacoustics-1.0.7/README.rst
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.725566 pyacoustics-1.0.7/praatScripts/
--rw-r--r--   0 tmahrt     (501) staff       (20)     1589 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/praatScripts/get_pitch_and_intensity.praat
--rw-r--r--   0 tmahrt     (501) staff       (20)      727 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/praatScripts/psolaPitch.praat
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.726525 pyacoustics-1.0.7/pyacoustics/
--rw-r--r--   0 tmahrt     (501) staff       (20)       49 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1962 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/aggregate_features.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.730457 pyacoustics-1.0.7/pyacoustics/intensity_and_pitch/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/intensity_and_pitch/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1654 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/intensity_and_pitch/get_f0.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.733102 pyacoustics-1.0.7/pyacoustics/signals/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/signals/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     6986 2020-10-28 13:19:51.000000 pyacoustics-1.0.7/pyacoustics/signals/audio_scripts.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1834 2021-01-28 00:26:47.000000 pyacoustics-1.0.7/pyacoustics/signals/data_fitting.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1166 2021-01-28 00:35:37.000000 pyacoustics-1.0.7/pyacoustics/signals/filters.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.738092 pyacoustics-1.0.7/pyacoustics/speech_detection/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3492 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/common.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2880 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/naive_vad.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2118 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/naive_vad_efficient.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     6925 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/segment_stereo_speech.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     7385 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/segment_stereo_speech_efficient.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2460 2021-01-22 12:30:38.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/split_on_tone.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1807 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_detection/textgrids.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.739116 pyacoustics-1.0.7/pyacoustics/speech_rate/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_rate/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3916 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_rate/dictionary_estimate.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2529 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/speech_rate/uwe_sr.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.739986 pyacoustics-1.0.7/pyacoustics/text/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/text/__init__.py
--rwxr-xr-x   0 tmahrt     (501) staff       (20)     5935 2021-08-08 11:39:51.000000 pyacoustics-1.0.7/pyacoustics/text/frequency.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      609 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/text/transcript.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.740850 pyacoustics-1.0.7/pyacoustics/textgrids/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/textgrids/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2911 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/textgrids/syllabify_textgrids.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     2517 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/textgrids/textgrids.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.745173 pyacoustics-1.0.7/pyacoustics/utilities/
--rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/__init__.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      475 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/error_utils.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1807 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/filters.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      781 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/matlab.py
--rw-r--r--   0 tmahrt     (501) staff       (20)      464 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/my_math.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     3468 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/normalize.py
--rw-r--r--   0 tmahrt     (501) staff       (20)    10607 2021-01-22 12:21:12.000000 pyacoustics-1.0.7/pyacoustics/utilities/sequences.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     1802 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/statistics.py
--rw-r--r--   0 tmahrt     (501) staff       (20)     5438 2019-04-30 15:47:25.000000 pyacoustics-1.0.7/pyacoustics/utilities/utils.py
-drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2021-08-08 11:44:06.728663 pyacoustics-1.0.7/pyacoustics.egg-info/
--rw-r--r--   0 tmahrt     (501) staff       (20)     6286 2021-08-08 11:44:06.000000 pyacoustics-1.0.7/pyacoustics.egg-info/PKG-INFO
--rw-r--r--   0 tmahrt     (501) staff       (20)     1565 2021-08-08 11:44:06.000000 pyacoustics-1.0.7/pyacoustics.egg-info/SOURCES.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)        1 2021-08-08 11:44:06.000000 pyacoustics-1.0.7/pyacoustics.egg-info/dependency_links.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       13 2021-08-08 11:44:06.000000 pyacoustics-1.0.7/pyacoustics.egg-info/requires.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       12 2021-08-08 11:44:06.000000 pyacoustics-1.0.7/pyacoustics.egg-info/top_level.txt
--rw-r--r--   0 tmahrt     (501) staff       (20)       38 2021-08-08 11:44:06.746145 pyacoustics-1.0.7/setup.cfg
--rw-r--r--   0 tmahrt     (501) staff       (20)      993 2021-08-08 11:33:33.000000 pyacoustics-1.0.7/setup.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.056873 pyacoustics-2.0.0/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3266 2020-11-26 00:42:38.000000 pyacoustics-2.0.0/LICENSE
+-rw-r--r--   0 tmahrt     (501) staff       (20)       28 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/MANIFEST.in
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4896 2023-07-15 16:22:52.056366 pyacoustics-2.0.0/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4518 2023-07-15 16:22:01.000000 pyacoustics-2.0.0/README.md
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.020176 pyacoustics-2.0.0/praatScripts/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1589 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/praatScripts/get_pitch_and_intensity.praat
+-rw-r--r--   0 tmahrt     (501) staff       (20)      727 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/praatScripts/psolaPitch.praat
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.022055 pyacoustics-2.0.0/pyacoustics/
+-rw-r--r--   0 tmahrt     (501) staff       (20)       49 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1844 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/aggregate_features.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.026208 pyacoustics-2.0.0/pyacoustics/intensity_and_pitch/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/intensity_and_pitch/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1569 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/intensity_and_pitch/get_f0.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.029706 pyacoustics-2.0.0/pyacoustics/signals/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/signals/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6741 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/signals/audio_scripts.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1867 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/signals/data_fitting.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1170 2023-07-15 16:03:54.000000 pyacoustics-2.0.0/pyacoustics/signals/filters.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.036321 pyacoustics-2.0.0/pyacoustics/speech_detection/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3386 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/common.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2876 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/naive_vad.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1992 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/naive_vad_efficient.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6250 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/segment_stereo_speech.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     6889 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/segment_stereo_speech_efficient.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2265 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/split_on_tone.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1783 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_detection/textgrids.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.038995 pyacoustics-2.0.0/pyacoustics/speech_rate/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/speech_rate/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3419 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_rate/dictionary_estimate.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2338 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/speech_rate/uwe_sr.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.041682 pyacoustics-2.0.0/pyacoustics/text/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/text/__init__.py
+-rwxr-xr-x   0 tmahrt     (501) staff       (20)     5922 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/text/frequency.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      596 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/text/transcript.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.047870 pyacoustics-2.0.0/pyacoustics/textgrids/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/textgrids/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2873 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/textgrids/syllabify_textgrids.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     2401 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/textgrids/textgrids.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.055395 pyacoustics-2.0.0/pyacoustics/utilities/
+-rw-r--r--   0 tmahrt     (501) staff       (20)        0 2019-04-30 15:47:25.000000 pyacoustics-2.0.0/pyacoustics/utilities/__init__.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      462 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/error_utils.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1713 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/filters.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      744 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/matlab.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)      483 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/my_math.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     3309 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/normalize.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)    10141 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/sequences.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1691 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/statistics.py
+-rw-r--r--   0 tmahrt     (501) staff       (20)     5539 2023-07-15 16:12:04.000000 pyacoustics-2.0.0/pyacoustics/utilities/utils.py
+drwxr-xr-x   0 tmahrt     (501) staff       (20)        0 2023-07-15 16:22:52.025407 pyacoustics-2.0.0/pyacoustics.egg-info/
+-rw-r--r--   0 tmahrt     (501) staff       (20)     4896 2023-07-15 16:22:51.000000 pyacoustics-2.0.0/pyacoustics.egg-info/PKG-INFO
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1572 2023-07-15 16:22:51.000000 pyacoustics-2.0.0/pyacoustics.egg-info/SOURCES.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)        1 2023-07-15 16:22:51.000000 pyacoustics-2.0.0/pyacoustics.egg-info/dependency_links.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       31 2023-07-15 16:22:51.000000 pyacoustics-2.0.0/pyacoustics.egg-info/requires.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       12 2023-07-15 16:22:51.000000 pyacoustics-2.0.0/pyacoustics.egg-info/top_level.txt
+-rw-r--r--   0 tmahrt     (501) staff       (20)       38 2023-07-15 16:22:52.057040 pyacoustics-2.0.0/setup.cfg
+-rw-r--r--   0 tmahrt     (501) staff       (20)     1117 2023-07-15 16:22:11.000000 pyacoustics-2.0.0/setup.py
```

### Comparing `pyacoustics-1.0.7/README.rst` & `pyacoustics-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 
--------------
-pyAcoustics
--------------
+# pyAcoustics
 
-.. image:: https://img.shields.io/badge/license-MIT-blue.svg?
-   :target: http://opensource.org/licenses/MIT
+[![](https://img.shields.io/badge/license-MIT-blue.svg?)](http://opensource.org/licenses/MIT)
 
 A collection of python scripts for extracting and analyzing acoustics from audio files.
 
-.. sectnum::
-.. contents::
+# Table of contents
+1. [Common use cases](#common-use-cases)
+2. [Version history](#version-history)
+3. [Requirements](#requirements)
+4. [Installation](#installation)
+5. [Example usage](#example-usage)
+6. [Citing pyAcoustics](#citing-pyacoustics)
+7. [Acknowledgements](#acknowledgements)
 
-Common Use Cases
-================
+## Common Use Cases
 
 What can you do with this library?
 
 - Extract pitch and intensity::
 
     pyacoustics.intensity_and_pitch.praat_pi.getPraatPitchAndIntensity()
 
@@ -41,79 +43,61 @@
 - Mask speech with speech shaped noise::
 
     pyacoustics.speech_filters.speech_shaped_noise.batchMaskSpeakerData()
 
 - And more!
 
 
-Major revisions
-================
+## Version history
 
-Ver 1.0 (June 7, 2015)
+*Praatio uses semantic versioning (Major.Minor.Patch)*
 
-- first public release.
+Please view [CHANGELOG.md](<https://github.com/timmahrt/pyAcoustics/blob/main/CHANGELOG.md>) for version history.
 
 
-Features as they are added
-===========================
-
-Mask speech with speech shaped noise
-(March 21, 2016)
-
-Find syllable nuclei/estimate speech rate using Uwe Reichel's matlab code
-(July 29, 2015) 
-
-Find the valley bottom between peaks (July 7th, 2015)
-
-Requirements
-================
+## Requirements
 
 Many of the individual features require different packages.  If you aren't using those
 packages then you don't need to install the dependencies.
 
 pyacoustics.intensity_and_pitch.praat_pi requires 
-`praat <http://www.fon.hum.uva.nl/praat/>`_
+[praat](<http://www.fon.hum.uva.nl/praat/>)
 
 pyacoustics.intensity_and_pitch.get_f0 requires the ESPS getF0 function as implemented 
-by `Snack <http://www.speech.kth.se/snack/>`_ although I recall having difficulty 
+by [Snack](<http://www.speech.kth.se/snack/>) although I recall having difficulty 
 installing it.
 
 pyacoustics.speech_rate/dictionary_estimate.py requires my library 
-`psyle <https://github.com/timmahrt/pysle>`_
+[psyle](<https://github.com/timmahrt/pysle>)
 
 pyacoustics.signals.data_fitting.py requires
-`SciPy <http://www.scipy.org/>`_,
-`NumPy <http://www.numpy.org/>`_, and
-`scikit-learn <http://scikit-learn.org/>`_
+[SciPy](<http://www.scipy.org/>),
+[NumPy](<http://www.numpy.org/>), and
+[scikit-learn](<http://scikit-learn.org/>)
 
 My praatIO library is used extensively and can be downloaded 
-`here <https://github.com/timmahrt/praatIO>`_
-
+[here](<https://github.com/timmahrt/praatIO>)
 
-Installation
-================
 
-If you on Windows, you can use the installer found here (check that it is up to date though)
-`Windows installer <http://www.timmahrt.com/python_installers>`_
+## Installation
 
 PyAcoustics is on pypi and can be installed or upgraded from the command-line shell with pip like so::
 
     python -m pip install pyacoustics --upgrade
 
 Otherwise, to manually install, after downloading the source from github, from a command-line shell, navigate to the directory containing setup.py and type::
 
     python setup.py install
 
 If python is not in your path, you'll need to enter the full path e.g.::
 
 	C:\Python36\python.exe setup.py install
 
     
-Example usage
-================
+## Example usage
 
 See the example folders for a few real-world examples using this library.
 
 - examples/split_audio_on_silence.py
 
     Detects the presence of speech in a recording based on acoustic 
     intensity.  Everything louder than some threshold specified by
@@ -131,29 +115,26 @@
     contain some voicing, so a stream of modulating pitch values
     suggests that someone is speaking.  This aspect is not extensively
     tested but it works well for the example files.
 
 - examples/estimate_speech_rate.py
 
     Calculates the speech rate through a matlab script written by
-    `Uwe Reichel <http://www.phonetik.uni-muenchen.de/~reichelu/>`_
+    [Uwe Reichel](<http://www.phonetik.uni-muenchen.de/~reichelu/>)
     that estimates the location of syllable boundaries.
 
-
-Citing LMEDS
-===============
+## Citing PyAcoustics
 
 PyAcoustics is general purpose coding and doesn't need to be cited
 but if you would like to, it can be cited like so:
 
 Tim Mahrt. PyAcoustics. https://github.com/timmahrt/pyAcoustics, 2016.
 
 
-Acknowledgements
-=================
+## Acknowledgements
 
 PyAcoustics is an ongoing collection of code with contributions from a
 number of projects worked on over several years.  Development of various
 aspects of PyAcoustics was possible thanks to
 NSF grant **IIS 07-03624**
 to Jennifer Cole and Mark Hasegawa-Johnson,
 NSF grant BCS **12-51343**
```

### Comparing `pyacoustics-1.0.7/praatScripts/get_pitch_and_intensity.praat` & `pyacoustics-2.0.0/praatScripts/get_pitch_and_intensity.praat`

 * *Files identical despite different names*

### Comparing `pyacoustics-1.0.7/praatScripts/psolaPitch.praat` & `pyacoustics-2.0.0/praatScripts/psolaPitch.praat`

 * *Files identical despite different names*

### Comparing `pyacoustics-1.0.7/pyacoustics/aggregate_features.py` & `pyacoustics-2.0.0/pyacoustics/aggregate_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-'''
+"""
 Created on Oct 20, 2014
 
 @author: tmahrt
-'''
+"""
 
 import os
 from os.path import join
 import io
 
 from pyacoustics.utilities import utils
 
 
 def aggregateFeatures(featurePath, featureList, headerStr=None):
-    
+
     outputDir = join(featurePath, "aggr")
     utils.makeDir(outputDir)
-    
+
     fnList = []
     dataList = []
-    
+
     # Find the files that exist in all features
     for feature in featureList:
-        fnSubList = utils.findFiles(join(featurePath, feature),
-                                    filterExt=".txt")
+        fnSubList = utils.findFiles(join(featurePath, feature), filterExt=".txt")
         fnList.append(fnSubList)
-        
+
     actualFNList = []
     for featureFN in fnList[0]:
         if all([featureFN in subList for subList in fnList]):
             actualFNList.append(featureFN)
-    
+
     for featureFN in actualFNList:
         dataList = []
         for feature in featureList:
-            featureDataList = utils.openCSV(join(featurePath, feature),
-                                            featureFN, encoding="utf-8")
+            featureDataList = utils.openCSV(
+                join(featurePath, feature), featureFN, encoding="utf-8"
+            )
             dataList.append([",".join(row) for row in featureDataList])
-        
+
         name = os.path.splitext(featureFN)[0]
-        
+
         dataList.insert(0, [name for _ in range(len(dataList[0]))])
         tDataList = utils.safeZip(dataList, enforceLength=True)
         outputList = [",".join(row) for row in tDataList]
         outputTxt = "\n".join(outputList)
-        
+
         outputFN = join(outputDir, name + ".csv")
         with io.open(outputFN, "w", encoding="utf-8") as fd:
             fd.write(outputTxt)
-        
+
     # Cat all files together
     aggrOutput = []
-    
+
     if headerStr is not None:
         aggrOutput.append(headerStr)
-    
+
     for fn in utils.findFiles(outputDir, filterExt=".csv"):
         if fn == "all.csv":
             continue
-        with io.open(join(outputDir, fn), "r", encoding='utf-8') as fd:
+        with io.open(join(outputDir, fn), "r", encoding="utf-8") as fd:
             aggrOutput.append(fd.read())
-    
-    with io.open(join(outputDir, "all.csv"), "w", encoding='utf-8') as fd:
+
+    with io.open(join(outputDir, "all.csv"), "w", encoding="utf-8") as fd:
         fd.write("\n".join(aggrOutput))
```

### Comparing `pyacoustics-1.0.7/pyacoustics/intensity_and_pitch/get_f0.py` & `pyacoustics-2.0.0/pyacoustics/intensity_and_pitch/get_f0.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,64 @@
-'''
+"""
 A Python implementation of ESPS's getF0 function
 
 The implementation is part of tkSnack.  As I recall, it is a bit
 cumbersome to install, although there are python distributions,
 like ActiveState, which come with it preinstalled.  For more information,
 visit the snack website:
 http://www.speech.kth.se/snack/
-'''
+"""
 import os
 from os.path import join
 
 import Tkinter
+
 root = Tkinter.Tk()
 import tkSnack
+
 tkSnack.initializeSnack(root)
 
 
 from rpt_feature_suite.utilities import utils
 
 MALE = "male"
 FEMALE = "female"
 
 SAMPLE_FREQ = 100
 
 
 def extractPitch(fnFullPath, minPitch, maxPitch):
-    '''
-    
+    """
+
     Former default pitch values: male (50, 350); female (75, 450)
-    '''
-        
+    """
+
     soundObj = tkSnack.Sound(load=fnFullPath)
 
-    output = soundObj.pitch(method="ESPS",
-                            minpitch=minPitch,
-                            maxpitch=maxPitch)
+    output = soundObj.pitch(method="ESPS", minpitch=minPitch, maxpitch=maxPitch)
 
     pitchList = []
     for value in output:
-
         value = value[0]
 
         if value == 0:
             value = int(value)
         pitchList.append(value)
-    
+
     return pitchList, SAMPLE_FREQ
 
 
 def getPitchAtTime(pitchList, startTime, endTime):
-    
     startIndex = int(startTime * SAMPLE_FREQ)
     endIndex = int(endTime * SAMPLE_FREQ)
 
     return pitchList[startIndex:endIndex]
 
 
 if __name__ == "__main__":
-
     path = "/Users/tmahrt/Desktop/fire_new_audio_test"
     for name in utils.findFiles(path, filterExt=".wav", stripExt=True):
         tmpPitchList = extractPitch(join(path, name + ".wav"), 75, 450)
         tmpPitchList = [str(val) for val in tmpPitchList]
-        
+
         with open(join(path, name + "_f0.csv"), "w") as fd:
             fd.write("\n".join(tmpPitchList))
```

### Comparing `pyacoustics-1.0.7/pyacoustics/signals/audio_scripts.py` & `pyacoustics-2.0.0/pyacoustics/signals/audio_scripts.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-'''
+"""
 Created on Aug 23, 2014
 
 @author: tmahrt
-'''
+"""
 
 import os
 from os.path import join
 
 import struct
 import wave
 import audioop
 
 from pyacoustics.utilities import utils
 
 
 def loadWavFile(wavFN):
-    
-    sampWidthDict = {1: 'b', 2: 'h', 4: 'i', 8: 'q'}
+    sampWidthDict = {1: "b", 2: "h", 4: "i", 8: "q"}
     audiofile = wave.open(wavFN, "r")
-    
+
     params = audiofile.getparams()
     sampwidth = params[1]
     nframes = params[3]
-    
+
     byteCode = sampWidthDict[sampwidth]
     waveData = audiofile.readframes(nframes)
     audioFrameList = struct.unpack("<" + byteCode * nframes, waveData)
-    
+
     return audioFrameList, params
 
 
 def resampleAudio(soxEXE, newSampleRate, inputPath, fn, outputPath=None):
-    '''
-    
+    """
+
     Mac: "/opt/local/bin/sox"
     Windows: "C:\Program Files (x86)\sox-14-4-2\sox.exe"
-    '''
+    """
     if outputPath is None:
         outputPath = join(inputPath, "resampled_wavs")
     utils.makeDir(outputPath)
-    
-    soxCmd = "%s %s -r %f %s rate -v 96k" % (soxEXE,
-                                             join(inputPath, fn),
-                                             newSampleRate,
-                                             join(outputPath, fn))
+
+    soxCmd = "%s %s -r %f %s rate -v 96k" % (
+        soxEXE,
+        join(inputPath, fn),
+        newSampleRate,
+        join(outputPath, fn),
+    )
     os.system(soxCmd)
 
 
 def getSerializedFileDuration(fn):
     name = os.path.splitext(fn)[0]
     durationFN = name + "_duration.txt"
     if not os.path.exists(durationFN):
@@ -58,185 +59,196 @@
         except IOError:
             # If we don't have write permissions, there isn't anything we can
             # do, the user should still be able to get their data
             pass
     else:
         with open(durationFN, "r") as fd:
             duration = float(fd.read())
-        
+
     return duration
 
 
 def getSoundFileDuration(fn):
-    '''
+    """
     Returns the duration of a wav file (in seconds)
-    '''
+    """
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
     framerate = params[2]
     nframes = params[3]
-    
+
     duration = float(nframes) / framerate
     return duration
-    
+
 
 def getParams(fn):
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
-    
+
     return params
 
 
 def reduceToSingleChannel(fn, outputFN, leftFactor=1, rightFactor=0):
-    
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
     sampwidth = params[1]
     nframes = params[3]
     audioFrames = audiofile.readframes(nframes)
-    
-    monoAudioFrames = audioop.tomono(audioFrames, sampwidth,
-                                     leftFactor, rightFactor)
-    params = tuple([1, ] + list(params[1:]))
-    
+
+    monoAudioFrames = audioop.tomono(audioFrames, sampwidth, leftFactor, rightFactor)
+    params = tuple(
+        [
+            1,
+        ]
+        + list(params[1:])
+    )
+
     outputAudiofile = wave.open(outputFN, "w")
     outputAudiofile.setparams(params)
     outputAudiofile.writeframes(monoAudioFrames)
 
 
 def modifySampleWidth(fn, outputFN, newSampleWidth):
-    
-    sampWidthDict = {1: 'b', 2: 'h', 4: 'i', 8: 'q'}
-    
+    sampWidthDict = {1: "b", 2: "h", 4: "i", 8: "q"}
+
     audiofile = wave.open(fn, "r")
     params = audiofile.getparams()
     sampwidth = params[1]
     nframes = params[3]
     waveData = audiofile.readframes(nframes)
-    
+
     sampleCode = sampWidthDict[sampwidth]
     newSampleCode = sampWidthDict[newSampleWidth]
-    
+
     audioFrameList = struct.unpack("<" + sampleCode * nframes, waveData)
     outputByteStr = struct.pack("<" + newSampleCode * nframes, *audioFrameList)
-    
+
     if newSampleWidth is not None:
-        params = list(params[:2]) + [newSampleWidth, ] + list(params[3:])
+        params = (
+            list(params[:2])
+            + [
+                newSampleWidth,
+            ]
+            + list(params[3:])
+        )
         params = tuple(params)
-    
+
     outputAudiofile = wave.open(outputFN, "w")
     outputAudiofile.setparams(params)
     outputAudiofile.writeframes(outputByteStr)
 
 
 def monoToStereo(fnL, fnR, outputFN, lfactor=1.0, rfactor=1.0):
-    '''
+    """
     Given two audio files, combines them into a stereo audio file
-    
+
     Derived mostly from the official python documentation
     https://docs.python.org/2/library/audioop.html
-    '''
-    
+    """
+
     def _monoToStereo(fn, leftBalance, rightBalance):
         audiofile = wave.open(fn, "r")
         params = audiofile.getparams()
         sampwidth = params[1]
         nframes = params[3]
-        
+
         waveData = audiofile.readframes(nframes)
-        sample = audioop.tostereo(waveData, sampwidth,
-                                  leftBalance, rightBalance)
-    
+        sample = audioop.tostereo(waveData, sampwidth, leftBalance, rightBalance)
+
         return sample, params
-    
+
     lsample, params = _monoToStereo(fnL, lfactor, 1 - lfactor)
     rsample = _monoToStereo(fnR, 1 - rfactor, rfactor)[0]
 
     sampwidth, framerate, nframes, comptype, compname = params[1:]
-    
+
     stereoSamples = audioop.add(lsample, rsample, sampwidth)
-    
+
     outputAudiofile = wave.open(outputFN, "w")
 
     params = [2, sampwidth, framerate, nframes, comptype, compname]
     outputAudiofile.setparams(params)
     outputAudiofile.writeframes(stereoSamples)
 
 
 def splitStereoAudio(path, fn, outputPath=None):
-    
     if outputPath is None:
         outputPath = join(path, "split_audio")
 
     if not os.path.exists(outputPath):
         os.mkdir(outputPath)
-    
+
     name = os.path.splitext(fn)[0]
-    
+
     fnFullPath = join(path, fn)
     leftOutputFN = join(outputPath, "%s_L.wav" % name)
     rightOutputFN = join(outputPath, "%s_R.wav" % name)
-    
+
     audiofile = wave.open(fnFullPath, "r")
 
     params = audiofile.getparams()
     sampwidth = params[1]
     nframes = params[3]
     audioFrames = audiofile.readframes(nframes)
-    
-    for leftFactor, rightFactor, outputFN in ((1, 0, leftOutputFN),
-                                              (0, 1, rightOutputFN)):
-        
-        monoAudioFrames = audioop.tomono(audioFrames, sampwidth,
-                                         leftFactor, rightFactor)
-        params = tuple([1, ] + list(params[1:]))
-        
+
+    for leftFactor, rightFactor, outputFN in (
+        (1, 0, leftOutputFN),
+        (0, 1, rightOutputFN),
+    ):
+        monoAudioFrames = audioop.tomono(
+            audioFrames, sampwidth, leftFactor, rightFactor
+        )
+        params = tuple(
+            [
+                1,
+            ]
+            + list(params[1:])
+        )
+
         outputAudiofile = wave.open(outputFN, "w")
         outputAudiofile.setparams(params)
         outputAudiofile.writeframes(monoAudioFrames)
 
 
 def getSubwav(fn, startT, endT, singleChannelFlag):
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
     nchannels = params[0]
     sampwidth = params[1]
     framerate = params[2]
 
     # Extract the audio frames
     audiofile.setpos(int(framerate * startT))
     audioFrames = audiofile.readframes(int(framerate * (endT - startT)))
-    
+
     # Convert to single channel if needed
     if singleChannelFlag is True and nchannels > 1:
         audioFrames = audioop.tomono(audioFrames, sampwidth, 1, 0)
         nchannels = 1
-    
+
     return audioFrames
-    
-    
+
+
 def extractSubwav(fn, outputFN, startT, endT, singleChannelFlag):
-    
     audiofile = wave.open(fn, "r")
     params = audiofile.getparams()
     nchannels = params[0]
     sampwidth = params[1]
     framerate = params[2]
     comptype = params[4]
     compname = params[5]
 
     print([fn, startT, endT])
     audioFrames = getSubwav(fn, startT, endT, singleChannelFlag)
-    
+
     if singleChannelFlag is True and nchannels > 1:
         nchannels = 1
-    
-    outParams = [nchannels, sampwidth, framerate,
-                 len(audioFrames), comptype, compname]
-    
+
+    outParams = [nchannels, sampwidth, framerate, len(audioFrames), comptype, compname]
+
     outWave = wave.open(outputFN, "w")
     outWave.setparams(outParams)
     outWave.writeframes(audioFrames)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/signals/data_fitting.py` & `pyacoustics-2.0.0/pyacoustics/signals/data_fitting.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,76 @@
-'''
+"""
 Created on Jul 6, 2015
 
 @author: tmahrt
-'''
+"""
 
 from sklearn import mixture
 
 from scipy import stats
+from scipy.stats import norm
 import matplotlib.pyplot as plot
 import matplotlib.mlab
 import numpy as np
 
 
 def getPDF(ddata, numSamples=50, minV=None, maxV=None):
-    
     pdf = stats.gaussian_kde(ddata)
-    
+
     if minV is None:
         minV = min(ddata)
     if maxV is None:
         maxV = max(ddata)
-    
+
     xValues = np.linspace(minV, maxV, numSamples)
-    
+
     yValues = pdf(xValues)
-    
+
     return xValues, yValues
 
 
 def getBimodalValley(data, numSamples=100, doplot=True):
-    '''
+    """
     Returns the smallest value between the peaks of a bimodal distribution
-    '''
+    """
 
     # Build GMM, fit it to the data, and get GMM parameters
     # The two means are used as the start and end point of a our search
     # for the smallest value between the two distributions.
-    
+
     ncomp = 2  # Could be parameterized later if needed
-    
-    clf = mixture.GaussianMixture(n_components=ncomp, covariance_type='full')
-    clf.fit([[item, ] for item in data])
+
+    clf = mixture.GaussianMixture(n_components=ncomp, covariance_type="full")
+    clf.fit(
+        [
+            [
+                item,
+            ]
+            for item in data
+        ]
+    )
     ml = clf.means_
     wl = clf.weights_
     cl = clf.covariances_
     ms = [m[0] for m in ml]
     cs = [np.sqrt(c[0][0]) for c in cl]
     ws = [w for w in wl]
-    
+
     # Find the smallest point in the pdf between the means
     startV = int(min(ms))
     endV = int(max(ms))
-    
+
     pdfX, pdfY = getPDF(data, numSamples, startV, endV)
     minY = min(pdfY)
     minX = pdfX[[float(x) for x in pdfY].index(minY)]
-    
+
     # Plot result if requested
     if doplot is True:
-        histo = plot.hist(data, numSamples, normed=True)
+        histo = plot.hist(data, numSamples)
         for w, m, c in zip(ws, ms, cs):
-            normedPDF = matplotlib.mlab.normpdf(histo[1], m, np.sqrt(c))
+            normedPDF = norm.pdf(histo[1], m, np.sqrt(c))
             plot.plot(histo[1], w * normedPDF, linewidth=3)
         plot.plot(pdfX, pdfY, linewidth=2)
         plot.axvline(minX)
         plot.show()
-    
+
     return minX
```

### Comparing `pyacoustics-1.0.7/pyacoustics/signals/filters.py` & `pyacoustics-2.0.0/pyacoustics/signals/filters.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 
 def _butter(cutoff, fs, btype, order=5):
     nyq = 0.5 * fs
     normal_cutoff = cutoff / nyq
     b, a = butter(order, normal_cutoff, btype=btype, analog=False)
     return b, a
 
+
 def filterData(data, cutoff, fs, btype, order=5):
     b, a = _butter(cutoff, fs, btype, order=order)
     y = lfilter(b, a, data)
     return y
 
+
 def filterFile(inputFn, outputFn, cutoff, btype, order=5):
-    '''
+    """
     Highpass or lowpass a file
 
     Highpass -- frequencies above the cutoff are kept, others removed
     Lowpass -- frequenices below the cutoff are kept, others removed
 
     cutoff - integer: the cutoff frequency
     btype - string: one of 'lowpass' or 'highpass'
     order - the order of the filter
-    '''
-    assert(btype in ['lowpass', 'highpass'])
-    fs,data=wavfile.read(inputFn)
+    """
+    assert btype in ["lowpass", "highpass"]
+    fs, data = wavfile.read(inputFn)
     filteredData = filterData(data, cutoff, fs, btype, order)
     wavfile.write(outputFn, fs, filteredData)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_detection/common.py` & `pyacoustics-2.0.0/pyacoustics/speech_detection/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-'''
+"""
 Created on Jun 7, 2015
 
 @author: tmahrt
-'''
+"""
 
 import struct
 import wave
 import math
 
 from pyacoustics.signals import audio_scripts
 
 
 class EndOfAudioData(Exception):
     pass
 
 
 def getSoundFileDuration(fn):
-    '''
+    """
     Returns the duration of a wav file (in seconds)
-    '''
+    """
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
     framerate = params[2]
     nframes = params[3]
-    
+
     duration = float(nframes) / framerate
     return duration
 
 
 def openAudioFile(fn):
     audiofile = wave.open(fn, "r")
-    
+
     params = audiofile.getparams()
     sampwidth = params[1]
     framerate = params[2]
-    
+
     return audiofile, sampwidth, framerate
 
 
 def rms(audioFrameList):
-    audioFrameList = [val ** 2 for val in audioFrameList]
+    audioFrameList = [val**2 for val in audioFrameList]
     meanVal = sum(audioFrameList) / len(audioFrameList)
     return math.sqrt(meanVal)
 
 
 def overlapCheck(interval, cmprInterval, percentThreshold=0):
-    '''Checks whether two intervals overlap'''
-    
+    """Checks whether two intervals overlap"""
+
     startTime, endTime = interval[0], interval[1]
     cmprStartTime, cmprEndTime = cmprInterval[0], cmprInterval[1]
-    
+
     overlapTime = min(endTime, cmprEndTime) - max(startTime, cmprStartTime)
     overlapTime = max(0, overlapTime)
     overlapFlag = overlapTime > 0
-    
+
     if percentThreshold > 0 and overlapFlag:
         totalTime = max(endTime, cmprEndTime) - min(startTime, cmprStartTime)
         percentOverlap = overlapTime / float(totalTime)
-        
+
         overlapFlag = percentOverlap >= percentThreshold
-    
+
     return overlapFlag
 
 
 def getMinMaxAmplitude(wavFN, stepSize, entryList=None):
-    
     audiofile = openAudioFile(wavFN)[0]
-    
+
     # By default, find the min and max amplitude for the whole file
     if entryList is None:
         stop = audio_scripts.getSoundFileDuration(wavFN)
-        entryList = [(0, stop), ]
-    
+        entryList = [
+            (0, stop),
+        ]
+
     # Accumulate relevant energy values
     rmsList = []
     for entry in entryList:
         start, stop = entry[0], entry[1]
         currentTime = start
         while currentTime < stop:
             rmsList.append(rmsNextFrames(audiofile, stepSize))
             currentTime += stepSize
-    
+
     # Return the min and max values
     minValue = min(rmsList)
     maxValue = max(rmsList)
-    
+
     return minValue, maxValue
 
 
 def rmsNextFrames(audiofile, stepSize, normMinVal=None, normMaxVal=None):
-    
     params = audiofile.getparams()
     sampwidth, framerate = params[1], params[2]
 
     numFrames = int(framerate * stepSize)
     waveData = audiofile.readframes(numFrames)
 
     if len(waveData) == 0:
         raise EndOfAudioData()
 
     actualNumFrames = int(len(waveData) / float(sampwidth))
     audioFrameList = struct.unpack("<" + "h" * actualNumFrames, waveData)
-    
+
     rmsEnergy = rms(audioFrameList)
 
     if normMinVal is not None and normMaxVal is not None:
         rmsEnergy = (rmsEnergy - normMinVal) / (normMaxVal - normMinVal)
 
     return rmsEnergy
 
 
 def mergeAdjacentEntries(entryList):
-    
     i = 0
     while i < len(entryList) - 1:
-        
         if entryList[i][1] == entryList[i + 1][0]:
             startEntry = entryList.pop(i)
             nextEntry = entryList.pop(i)
-            
+
             entryList.insert(i, (startEntry[0], nextEntry[1]))
         else:
             i += 1
-            
+
     return entryList
 
 
 def cropUnusedPortion(entry, start, stop):
-    
     retEntryList = []
-    
+
     if entry[0] < start:
         retEntryList.append((entry[0], start))
-    
+
     if entry[1] > stop:
         retEntryList.append((stop, entry[1]))
-    
+
     return retEntryList
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_detection/segment_stereo_speech.py` & `pyacoustics-2.0.0/pyacoustics/speech_detection/segment_stereo_speech.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,189 +1,221 @@
-'''
+"""
 Created on Nov 4, 2014
 
 @author: tmahrt
-'''
+"""
 
 from pyacoustics.speech_detection import common
 
 
-def findNextSpeaker(leftSamples, rightSamples, samplingFreq,
-                    startTime, analyzeStop, stepSize,
-                    numSteps, findLeft=True):
-    '''
-    
-    '''
-    
+def findNextSpeaker(
+    leftSamples,
+    rightSamples,
+    samplingFreq,
+    startTime,
+    analyzeStop,
+    stepSize,
+    numSteps,
+    findLeft=True,
+):
+    """"""
+
     # Extract the audio frames
     i = 0
     currentSequenceNum = 0
     while currentSequenceNum < numSteps:
-
         # Stop analyzing once we've reached the end of this interval
         currentTime = startTime + i * stepSize
         nextTime = startTime + ((i + 1) * stepSize)
 
         if nextTime > analyzeStop:
             raise common.EndOfAudioData()
 
-        leftRMSEnergy = common.rms(leftSamples[int(currentTime *
-                                                   samplingFreq):
-                                               int(nextTime *
-                                                   samplingFreq)])
-        rightRMSEnergy = common.rms(rightSamples[int(currentTime *
-                                                     samplingFreq):
-                                                 int(nextTime *
-                                                     samplingFreq)])
-        
-        if ((findLeft is True and leftRMSEnergy >= rightRMSEnergy) or
-           (findLeft is False and leftRMSEnergy <= rightRMSEnergy)):
+        leftRMSEnergy = common.rms(
+            leftSamples[int(currentTime * samplingFreq) : int(nextTime * samplingFreq)]
+        )
+        rightRMSEnergy = common.rms(
+            rightSamples[int(currentTime * samplingFreq) : int(nextTime * samplingFreq)]
+        )
+
+        if (findLeft is True and leftRMSEnergy >= rightRMSEnergy) or (
+            findLeft is False and leftRMSEnergy <= rightRMSEnergy
+        ):
             currentSequenceNum += 1
         else:
             currentSequenceNum = 0
         i += 1
-    
+
     endTime = startTime + (i - numSteps) * stepSize
-    
+
     return endTime
 
 
-def assignAudioEventsForEntries(leftSamples, rightSamples, samplingFreq,
-                                leftEntry, rightEntry, stepSize,
-                                speakerNumSteps):
-    '''
+def assignAudioEventsForEntries(
+    leftSamples,
+    rightSamples,
+    samplingFreq,
+    leftEntry,
+    rightEntry,
+    stepSize,
+    speakerNumSteps,
+):
+    """
     Start up and tear down function for assignAudioEvents()
-    '''
-    
+    """
+
     # Find the overlap interval and preserve the non-overlapped portions
     start = max(leftEntry[0], rightEntry[0])
     stop = min(leftEntry[1], rightEntry[1])
-    
+
     leftEntryList = common.cropUnusedPortion(leftEntry, start, stop)
     rightEntryList = common.cropUnusedPortion(rightEntry, start, stop)
-    
+
     # Determine who is speaking in overlapped portions
-    tmpEntries = assignAudioEvents(leftSamples, rightSamples, samplingFreq,
-                                   start, stop, stepSize, speakerNumSteps)
-    
+    tmpEntries = assignAudioEvents(
+        leftSamples, rightSamples, samplingFreq, start, stop, stepSize, speakerNumSteps
+    )
+
     leftEntryList.extend(tmpEntries[0])
     rightEntryList.extend(tmpEntries[1])
-    
+
     # Merge adjacent regions sharing a boundary, if any
     leftEntryList.sort()
     rightEntryList.sort()
-    
+
     leftEntryList = common.mergeAdjacentEntries(leftEntryList)
     rightEntryList = common.mergeAdjacentEntries(rightEntryList)
-    
-    return leftEntryList, rightEntryList
 
+    return leftEntryList, rightEntryList
 
-def assignAudioEvents(leftSamples, rightSamples, samplingFreq, startTime,
-                      analyzeStop, stepSize, speakerNumSteps):
 
+def assignAudioEvents(
+    leftSamples,
+    rightSamples,
+    samplingFreq,
+    startTime,
+    analyzeStop,
+    stepSize,
+    speakerNumSteps,
+):
     findLeft = True
     leftEntryList = []
     rightEntryList = []
     try:
         while True:
-            endTime = findNextSpeaker(leftSamples, rightSamples,
-                                      samplingFreq, startTime,
-                                      analyzeStop, stepSize,
-                                      speakerNumSteps, findLeft)
-            
+            endTime = findNextSpeaker(
+                leftSamples,
+                rightSamples,
+                samplingFreq,
+                startTime,
+                analyzeStop,
+                stepSize,
+                speakerNumSteps,
+                findLeft,
+            )
+
             if endTime > analyzeStop:
                 endTime = analyzeStop
-            
+
             if startTime != endTime:
                 entry = (startTime, endTime)
                 if findLeft:
                     leftEntryList.append(entry)
                 else:
                     rightEntryList.append(entry)
-            
+
             print("%f, %f, %f" % (startTime, endTime, analyzeStop))
             startTime = endTime
             findLeft = not findLeft
-        
+
     except common.EndOfAudioData:  # Stop processing
-    
         if analyzeStop - startTime > stepSize * speakerNumSteps:
             finalEntry = (startTime, analyzeStop)
             if findLeft:
                 leftEntryList.append(finalEntry)
             else:
                 rightEntryList.append(finalEntry)
-    
-    return leftEntryList, rightEntryList
 
+    return leftEntryList, rightEntryList
 
-def autosegmentStereoAudio(leftSamples, rightSamples, samplingFreq,
-                           leftEntryList, rightEntryList,
-                           stepSize, speakerNumSteps):
 
+def autosegmentStereoAudio(
+    leftSamples,
+    rightSamples,
+    samplingFreq,
+    leftEntryList,
+    rightEntryList,
+    stepSize,
+    speakerNumSteps,
+):
     overlapThreshold = 0
-    overlapCheck = (lambda entry, entryList:
-                    [not common.overlapCheck(entry,
-                                             cmprEntry,
-                                             overlapThreshold)
-                     for cmprEntry in entryList]
-                    )
-    
+    overlapCheck = lambda entry, entryList: [
+        not common.overlapCheck(entry, cmprEntry, overlapThreshold)
+        for cmprEntry in entryList
+    ]
+
     # First add all of the entries with no overlap
     newLeftEntryList = []
     for leftEntry in leftEntryList:
-        
         if all(overlapCheck(leftEntry, rightEntryList)):
             newLeftEntryList.append(leftEntry)
-            
+
     newRightEntryList = []
     for rightEntry in rightEntryList:
-        
         if all(overlapCheck(rightEntry, leftEntryList)):
             newRightEntryList.append(rightEntry)
-        
+
     # For all entries with overlap, split them by speaker
     # Utilizing the left channel as a base, this chunks through all overlapping
     # in a single pass of the left channel, until there are no more overlapping
     # segments between the right and left channels.
     i = 0
     while i < len(leftEntryList):
-        
         # Check if there are any segments in the right channel that overlap
         # with the current segment in the left channel.  If not, move to
         # the next segment.
         leftEntry = leftEntryList[i]
         overlapCheckList = overlapCheck(leftEntry, rightEntryList)
         if all(overlapCheckList):
             i += 1
             continue
-        
+
         # Otherwise, resolve the first segment in the right channel that
         # overlaps with the current segment
         leftEntry = leftEntryList.pop(i)
-        
+
         j = overlapCheckList.index(False)  # Find the first overlap
         rightEntry = rightEntryList.pop(j)
-        
-        entryTuple = assignAudioEventsForEntries(leftSamples, rightSamples,
-                                                 samplingFreq,
-                                                 leftEntry, rightEntry,
-                                                 stepSize, speakerNumSteps)
+
+        entryTuple = assignAudioEventsForEntries(
+            leftSamples,
+            rightSamples,
+            samplingFreq,
+            leftEntry,
+            rightEntry,
+            stepSize,
+            speakerNumSteps,
+        )
         tmpLeftEntryList, tmpRightEntryList = entryTuple
-        
+
         leftEntryList[i:i] = tmpLeftEntryList
         rightEntryList[j:j] = tmpRightEntryList
 
     # Combine the original non-overlapping segments with the adjusted segments
     newLeftEntryList.extend(leftEntryList)
     newRightEntryList.extend(rightEntryList)
-    
+
     newLeftEntryList.sort()
     newRightEntryList.sort()
-    
-    newLeftEntryList = [entry for entry in newLeftEntryList
-                        if (entry[1] - entry[0] > stepSize * speakerNumSteps)]
-    newRightEntryList = [entry for entry in newRightEntryList
-                         if (entry[1] - entry[0] > stepSize * speakerNumSteps)]
-    
+
+    newLeftEntryList = [
+        entry
+        for entry in newLeftEntryList
+        if (entry[1] - entry[0] > stepSize * speakerNumSteps)
+    ]
+    newRightEntryList = [
+        entry
+        for entry in newRightEntryList
+        if (entry[1] - entry[0] > stepSize * speakerNumSteps)
+    ]
+
     return newLeftEntryList, newRightEntryList
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_detection/segment_stereo_speech_efficient.py` & `pyacoustics-2.0.0/pyacoustics/speech_detection/segment_stereo_speech_efficient.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,198 +1,247 @@
-'''
+"""
 Created on Nov 4, 2014
 
 @author: tmahrt
-'''
+"""
 
 from pyacoustics.speech_detection import common
 
 
-def findNextSpeaker(leftFN, rightFN, startTime, analyzeStop, stepSize,
-                    numSteps, findLeft=True, leftMin=None, leftMax=None,
-                    rightMin=None, rightMax=None):
-    '''
-    
-    '''
-    
+def findNextSpeaker(
+    leftFN,
+    rightFN,
+    startTime,
+    analyzeStop,
+    stepSize,
+    numSteps,
+    findLeft=True,
+    leftMin=None,
+    leftMax=None,
+    rightMin=None,
+    rightMax=None,
+):
+    """"""
+
     audioTuple = common.openAudioFile(leftFN)
     leftAudioFile = audioTuple[0]
     framerate = audioTuple[2]
     rightAudioFile = common.openAudioFile(rightFN)[0]
-    
+
     # Extract the audio frames
     i = 0
     currentSequenceNum = 0
     leftAudioFile.setpos(int(framerate * startTime))
     rightAudioFile.setpos(int(framerate * startTime))
     while currentSequenceNum < numSteps:
-
         # Stop analyzing once we've reached the end of this interval
         currentTime = startTime + i * stepSize
 
         if currentTime >= analyzeStop:
             raise common.EndOfAudioData()
 
-        leftRMSEnergy = common.rmsNextFrames(leftAudioFile, stepSize,
-                                             leftMin, leftMax)
-        rightRMSEnergy = common.rmsNextFrames(rightAudioFile, stepSize,
-                                              rightMin, rightMax)
-        
-        if ((findLeft is True and leftRMSEnergy >= rightRMSEnergy) or
-           (findLeft is False and leftRMSEnergy <= rightRMSEnergy)):
+        leftRMSEnergy = common.rmsNextFrames(leftAudioFile, stepSize, leftMin, leftMax)
+        rightRMSEnergy = common.rmsNextFrames(
+            rightAudioFile, stepSize, rightMin, rightMax
+        )
+
+        if (findLeft is True and leftRMSEnergy >= rightRMSEnergy) or (
+            findLeft is False and leftRMSEnergy <= rightRMSEnergy
+        ):
             currentSequenceNum += 1
         else:
             currentSequenceNum = 0
         i += 1
-    
+
     endTime = startTime + (i - numSteps) * stepSize
-    
+
     return endTime
 
 
-def assignAudioEventsForEntries(leftFN, rightFN, leftEntry, rightEntry,
-                                stepSize, speakerNumSteps, leftMin, leftMax,
-                                rightMin, rightMax):
-    '''
+def assignAudioEventsForEntries(
+    leftFN,
+    rightFN,
+    leftEntry,
+    rightEntry,
+    stepSize,
+    speakerNumSteps,
+    leftMin,
+    leftMax,
+    rightMin,
+    rightMax,
+):
+    """
     Start up and tear down function for assignAudioEvents()
-    '''
-    
+    """
+
     # Find the overlap interval and preserve the non-overlapped portions
     start = max(leftEntry[0], rightEntry[0])
     stop = min(leftEntry[1], rightEntry[1])
-    
+
     leftEntryList = common.cropUnusedPortion(leftEntry, start, stop)
     rightEntryList = common.cropUnusedPortion(rightEntry, start, stop)
-    
+
     # Determine who is speaking in overlapped portions
-    tmpEntries = assignAudioEvents(leftFN, rightFN, start, stop, stepSize,
-                                   speakerNumSteps, leftMin, leftMax, rightMin,
-                                   rightMax)
-    
+    tmpEntries = assignAudioEvents(
+        leftFN,
+        rightFN,
+        start,
+        stop,
+        stepSize,
+        speakerNumSteps,
+        leftMin,
+        leftMax,
+        rightMin,
+        rightMax,
+    )
+
     leftEntryList.extend(tmpEntries[0])
     rightEntryList.extend(tmpEntries[1])
-    
+
     # Merge adjacent regions sharing a boundary, if any
     leftEntryList.sort()
     rightEntryList.sort()
-    
+
     leftEntryList = common.mergeAdjacentEntries(leftEntryList)
     rightEntryList = common.mergeAdjacentEntries(rightEntryList)
-    
-    return leftEntryList, rightEntryList
 
+    return leftEntryList, rightEntryList
 
-def assignAudioEvents(leftFN, rightFN, startTime, analyzeStop, stepSize,
-                      speakerNumSteps, leftMin, leftMax, rightMin, rightMax):
 
+def assignAudioEvents(
+    leftFN,
+    rightFN,
+    startTime,
+    analyzeStop,
+    stepSize,
+    speakerNumSteps,
+    leftMin,
+    leftMax,
+    rightMin,
+    rightMax,
+):
     findLeft = True
     leftEntryList = []
     rightEntryList = []
     try:
         while True:
-            endTime = findNextSpeaker(leftFN, rightFN, startTime, analyzeStop,
-                                      stepSize, speakerNumSteps, findLeft,
-                                      leftMin, leftMax, rightMin, rightMax)
-            
+            endTime = findNextSpeaker(
+                leftFN,
+                rightFN,
+                startTime,
+                analyzeStop,
+                stepSize,
+                speakerNumSteps,
+                findLeft,
+                leftMin,
+                leftMax,
+                rightMin,
+                rightMax,
+            )
+
             if endTime > analyzeStop:
                 endTime = analyzeStop
-            
+
             if startTime != endTime:
                 entry = (startTime, endTime)
                 if findLeft:
                     leftEntryList.append(entry)
                 else:
                     rightEntryList.append(entry)
-            
+
             print("%f, %f, %f" % (startTime, endTime, analyzeStop))
             startTime = endTime
             findLeft = not findLeft
-        
+
     except common.EndOfAudioData:  # Stop processing
-    
         if analyzeStop - startTime > stepSize * speakerNumSteps:
             finalEntry = (startTime, analyzeStop)
             if findLeft:
                 leftEntryList.append(finalEntry)
             else:
                 rightEntryList.append(finalEntry)
-    
-    return leftEntryList, rightEntryList
 
+    return leftEntryList, rightEntryList
 
-def autosegmentStereoAudio(leftFN, rightFN, leftEntryList, rightEntryList,
-                           stepSize, speakerNumSteps):
 
+def autosegmentStereoAudio(
+    leftFN, rightFN, leftEntryList, rightEntryList, stepSize, speakerNumSteps
+):
     overlapThreshold = 0
-    overlapCheck = (lambda entry, entryList:
-                    [not common.overlapCheck(entry,
-                                             cmprEntry,
-                                             overlapThreshold)
-                     for cmprEntry in entryList]
-                    )
-    
+    overlapCheck = lambda entry, entryList: [
+        not common.overlapCheck(entry, cmprEntry, overlapThreshold)
+        for cmprEntry in entryList
+    ]
+
     # Find the min and max intensity levels for normalizing later
-    leftMin, leftMax = common.getMinMaxAmplitude(leftFN,
-                                                 stepSize,
-                                                 leftEntryList)
-    rightMin, rightMax = common.getMinMaxAmplitude(rightFN,
-                                                   stepSize,
-                                                   rightEntryList)
-    
+    leftMin, leftMax = common.getMinMaxAmplitude(leftFN, stepSize, leftEntryList)
+    rightMin, rightMax = common.getMinMaxAmplitude(rightFN, stepSize, rightEntryList)
+
     # First add all of the entries with no overlap
     newLeftEntryList = []
     for leftEntry in leftEntryList:
-        
         if all(overlapCheck(leftEntry, rightEntryList)):
             newLeftEntryList.append(leftEntry)
-            
+
     newRightEntryList = []
     for rightEntry in rightEntryList:
-        
         if all(overlapCheck(rightEntry, leftEntryList)):
             newRightEntryList.append(rightEntry)
-        
+
     # For all entries with overlap, split them by speaker
     # Utilizing the left channel as a base, this chunks through all overlapping
     # in a single pass of the left channel, until there are no more overlapping
     # segments between the right and left channels.
     i = 0
     while i < len(leftEntryList):
-        
         # Check if there are any segments in the right channel that overlap
         # with the current segment in the left channel.  If not, move to
         # the next segment.
         leftEntry = leftEntryList[i]
         overlapCheckList = overlapCheck(leftEntry, rightEntryList)
         if all(overlapCheckList):
             i += 1
             continue
-        
+
         # Otherwise, resolve the first segment in the right channel that
         # overlaps with the current segment
         leftEntry = leftEntryList.pop(i)
-        
+
         j = overlapCheckList.index(False)  # Find the first overlap
         rightEntry = rightEntryList.pop(j)
-        
-        entryTuple = assignAudioEventsForEntries(leftFN, rightFN, leftEntry,
-                                                 rightEntry, stepSize,
-                                                 speakerNumSteps, leftMin,
-                                                 leftMax, rightMin, rightMax)
+
+        entryTuple = assignAudioEventsForEntries(
+            leftFN,
+            rightFN,
+            leftEntry,
+            rightEntry,
+            stepSize,
+            speakerNumSteps,
+            leftMin,
+            leftMax,
+            rightMin,
+            rightMax,
+        )
         tmpLeftEntryList, tmpRightEntryList = entryTuple
-        
+
         leftEntryList[i:i] = tmpLeftEntryList
         rightEntryList[j:j] = tmpRightEntryList
 
     # Combine the original non-overlapping segments with the adjusted segments
     newLeftEntryList.extend(leftEntryList)
     newRightEntryList.extend(rightEntryList)
-    
+
     newLeftEntryList.sort()
     newRightEntryList.sort()
-    
-    newLeftEntryList = [entry for entry in newLeftEntryList
-                        if (entry[1] - entry[0] > stepSize * speakerNumSteps)]
-    newRightEntryList = [entry for entry in newRightEntryList
-                         if (entry[1] - entry[0] > stepSize * speakerNumSteps)]
-    
+
+    newLeftEntryList = [
+        entry
+        for entry in newLeftEntryList
+        if (entry[1] - entry[0] > stepSize * speakerNumSteps)
+    ]
+    newRightEntryList = [
+        entry
+        for entry in newRightEntryList
+        if (entry[1] - entry[0] > stepSize * speakerNumSteps)
+    ]
+
     return newLeftEntryList, newRightEntryList
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_detection/split_on_tone.py` & `pyacoustics-2.0.0/pyacoustics/speech_detection/split_on_tone.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,86 +1,88 @@
-'''
+"""
 Created on Sep 6, 2014
 
 @author: tmahrt
-'''
+"""
 
 import os
 from os.path import join
 import math
 
 from pyacoustics.signals import audio_scripts
 from pyacoustics.utilities import sequences
 
 BEEP = "beep"
 SILENCE = "silence"
 SPEECH = "speech"
 
 
 def _homogenizeList(dataList, toneFrequency):
-    '''
+    """
     Discritizes pitch values into one of three categories
-    '''
-    
+    """
+
     minVal = min(dataList)
-    
+
     retDataList = []
     for val in dataList:
         if val == toneFrequency:
             val = BEEP
         elif val == minVal:
             val = SILENCE
         else:
             val = SPEECH
         retDataList.append(val)
-        
+
     return retDataList
 
 
-def splitFileOnTone(pitchList, timeStep, toneFrequency,
-                    eventDurationThreshold):
-    '''
+def splitFileOnTone(pitchList, timeStep, toneFrequency, eventDurationThreshold):
+    """
     Splits files by pure tones
-    '''
+    """
     toneFrequency = int(round(toneFrequency, -1))
-    
+
     roundedPitchList = [int(round(val, -1)) for val in pitchList]
     codedPitchList = _homogenizeList(roundedPitchList, toneFrequency)
-    
+
     compressedList = sequences.compressList(codedPitchList)
-    timeDict = sequences.compressedListTransform(compressedList,
-                                                 1.0/timeStep,
-                                                 eventDurationThreshold)
-    
+    timeDict = sequences.compressedListTransform(
+        compressedList, 1.0 / timeStep, eventDurationThreshold
+    )
+
     # Fill in with empty lists if it didn't appear in the dataset
     # (eg no beeps were detected or no speech occurred)
     for key in [BEEP, SPEECH, SILENCE]:
         if key not in timeDict:
             timeDict[key] = []
 
     return timeDict
-    
+
 
 def extractSubwavs(timeDict, path, fn, outputPath):
-    '''
+    """
     Extracts segments between tones marked in the output of splitFileOnTone()
-    '''
+    """
     name = os.path.splitext(fn)[0]
-    
+
     duration = audio_scripts.getSoundFileDuration(join(path, fn))
     beepEntryList = timeDict[BEEP]
     segmentEntryList = sequences.invertIntervalList(beepEntryList, 0, duration)
-    
+
     if len(segmentEntryList) > 0:
         numZeroes = int(math.floor(math.log10(len(segmentEntryList)))) + 1
     else:
         numZeroes = 1
-        
+
     strFmt = "%%s_%%0%dd.wav" % numZeroes  # e.g. '%s_%02d.wav'
 
     for i, entry in enumerate(segmentEntryList):
         start, stop = entry[:2]
-        
-        audio_scripts.extractSubwav(join(path, fn),
-                                    join(outputPath, strFmt % (name, i)),
-                                    startT=float(start), endT=float(stop),
-                                    singleChannelFlag=True)
+
+        audio_scripts.extractSubwav(
+            join(path, fn),
+            join(outputPath, strFmt % (name, i)),
+            startT=float(start),
+            endT=float(stop),
+            singleChannelFlag=True,
+        )
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_detection/textgrids.py` & `pyacoustics-2.0.0/pyacoustics/speech_detection/textgrids.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,60 @@
-'''
+"""
 Created on Nov 5, 2014
 
 @author: tmahrt
 
 Textgrid utilities for saving the output of speech detection code into
 praat textgrids.
-'''
+"""
 
-from praatio import tgio
+from praatio import textgrid
 
 
 def outputTextgrid(outputFN, duration, entryList, tierName):
-    
     # Give all entries a label indicating their order of occurrence
     entryList.sort()
-    newEntryList = [(entry[0], entry[1], str(i))
-                    for i, entry in enumerate(entryList)]
-    
+    newEntryList = [(entry[0], entry[1], str(i)) for i, entry in enumerate(entryList)]
+
     # Output textgrid
-    tierSpeech = tgio.IntervalTier(tierName, newEntryList, 0, duration)
+    tierSpeech = textgrid.IntervalTier(tierName, newEntryList, 0, duration)
 
-    tg = tgio.Textgrid()
+    tg = textgrid.Textgrid()
     tg.addTier(tierSpeech)
-    tg.save(outputFN)
-
+    tg.save(outputFN, format="short_textgrid", includeBlankSpaces=True)
 
-def outputStereoTextgrid(outputFN, duration, leftEntryList, rightEntryList,
-                         leftChannelName, rightChannelName):
 
+def outputStereoTextgrid(
+    outputFN, duration, leftEntryList, rightEntryList, leftChannelName, rightChannelName
+):
     # Give all entries a label indicating their order of occurrence
     leftEntryList.sort()
-    newLeftEntryList = [(entry[0], entry[1], str(i))
-                        for i, entry in enumerate(leftEntryList)]
+    newLeftEntryList = [
+        (entry[0], entry[1], str(i)) for i, entry in enumerate(leftEntryList)
+    ]
 
     rightEntryList.sort()
-    newRightEntryList = [(entry[0], entry[1], str(i))
-                         for i, entry in enumerate(rightEntryList)]
-    
+    newRightEntryList = [
+        (entry[0], entry[1], str(i)) for i, entry in enumerate(rightEntryList)
+    ]
+
     # This shouldn't be necessary
-    newLeftEntryList = [entry for entry in newLeftEntryList
-                        if entry[1] <= duration and entry[0] < entry[1]]
-    newRightEntryList = [entry for entry in newRightEntryList
-                         if entry[1] <= duration and entry[0] < entry[1]]
-    
+    newLeftEntryList = [
+        entry
+        for entry in newLeftEntryList
+        if entry[1] <= duration and entry[0] < entry[1]
+    ]
+    newRightEntryList = [
+        entry
+        for entry in newRightEntryList
+        if entry[1] <= duration and entry[0] < entry[1]
+    ]
+
     # Output textgrid
-    leftTier = tgio.IntervalTier(leftChannelName, newLeftEntryList,
-                                    0, duration)
-    rightTier = tgio.IntervalTier(rightChannelName, newRightEntryList,
-                                     0, duration)
-    
-    outputTG = tgio.Textgrid()
+    leftTier = textgrid.IntervalTier(leftChannelName, newLeftEntryList, 0, duration)
+    rightTier = textgrid.IntervalTier(rightChannelName, newRightEntryList, 0, duration)
+
+    outputTG = textgrid.Textgrid()
     outputTG.addTier(leftTier)
     outputTG.addTier(rightTier)
-    
-    outputTG.save(outputFN)
+
+    outputTG.save(outputFN, format="short_textgrid", includeBlankSpaces=True)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_rate/dictionary_estimate.py` & `pyacoustics-2.0.0/pyacoustics/speech_rate/dictionary_estimate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,107 @@
-'''
+"""
 Created on Jan 28, 2015
 
 @author: tmahrt
-'''
+"""
 
 import os
 from os.path import join
 
 from pyacoustics.utilities import utils
 from pysle import isletool
 
 
 def percentInside(startTime, endTime, cmprStartTime, cmprEndTime):
-    
-    if (float(startTime) <= float(cmprEndTime) and
-            float(endTime) >= float(cmprStartTime)):
-
+    if float(startTime) <= float(cmprEndTime) and float(endTime) >= float(
+        cmprStartTime
+    ):
         leftEdge = cmprStartTime - startTime
         rightEdge = endTime - cmprEndTime
-        
+
         if leftEdge < 0:
             leftEdge = 0
         if rightEdge < 0:
             rightEdge = 0
-            
+
         retVal = 1 - ((rightEdge + leftEdge)) / (endTime - startTime)
 
     # No overlap
     else:
         retVal = 0
 
     return retVal
 
 
 def manualPhoneCount(tgInfoPath, isleFN, outputPath, skipList=None):
-    
     if skipList is None:
         skipList = []
-    
+
     utils.makeDir(outputPath)
-    
+
     isleDict = isletool.LexicalTool(isleFN)
-    
-    existFNList = utils.findFiles(outputPath, filterPaths=".txt")
-    for fn in utils.findFiles(tgInfoPath, filterExt=".txt",
-                              skipIfNameInList=existFNList):
 
+    existFNList = utils.findFiles(outputPath, filterPaths=".txt")
+    for fn in utils.findFiles(
+        tgInfoPath, filterExt=".txt", skipIfNameInList=existFNList
+    ):
         if os.path.exists(join(outputPath, fn)):
             continue
         print(fn)
-        
+
         dataList = utils.openCSV(tgInfoPath, fn)
         dataList = [row[2] for row in dataList]  # start, stop, tmpLabel
         outputList = []
         for tmpLabel in dataList:
             if tmpLabel not in skipList:
-                syllableCount, phoneCount = isletool.getNumPhones(isleDict,
-                                                                  tmpLabel,
-                                                                  maxFlag=True)
+                syllableCount, phoneCount = isletool.getNumPhones(
+                    isleDict, tmpLabel, maxFlag=True
+                )
             else:
                 syllableCount, phoneCount = 0, 0
-            
+
             outputList.append("%d,%d" % (syllableCount, phoneCount))
-        
+
         outputTxt = "\n".join(outputList)
-        
+
         with open(join(outputPath, fn), "w") as fd:
             fd.write(outputTxt)
-        
 
-def manualPhoneCountForEpochs(manualCountsPath, tgInfoPath, epochPath,
-                              outputPath):
-    
+
+def manualPhoneCountForEpochs(manualCountsPath, tgInfoPath, epochPath, outputPath):
     utils.makeDir(outputPath)
-    
+
     skipList = utils.findFiles(outputPath, filterExt=".txt")
-    for fn in utils.findFiles(tgInfoPath, filterExt=".txt",
-                              skipIfNameInList=skipList):
-        
+    for fn in utils.findFiles(tgInfoPath, filterExt=".txt", skipIfNameInList=skipList):
         epochList = utils.openCSV(epochPath, fn)
         tgInfo = utils.openCSV(tgInfoPath, fn)
         manualCounts = utils.openCSV(manualCountsPath, fn)
-        
+
         epochOutputList = []
         for epochTuple in epochList:  # Epoch num, start, stop
             epochStart, epochStop = float(epochTuple[1]), float(epochTuple[2])
-            
+
             # Find all of the intervals that are at least partially
             # contained within the current epoch
             epochSyllableCount = 0
             epochPhoneCount = 0
             speechDuration = 0
-            for info, counts in utils.safeZip([tgInfo, manualCounts],
-                                              enforceLength=True):
+            for info, counts in utils.safeZip(
+                [tgInfo, manualCounts], enforceLength=True
+            ):
                 start, stop = float(info[0]), float(info[1])
                 syllableCount, phoneCount = float(counts[0]), float(counts[1])
-            
+
                 # Accounts for intervals that straddle an epoch boundary
-                multiplicationFactor = percentInside(start, stop,
-                                                     epochStart, epochStop)
-                
+                multiplicationFactor = percentInside(start, stop, epochStart, epochStop)
+
                 speechDuration += (stop - start) * multiplicationFactor
-                
+
                 epochSyllableCount += syllableCount * multiplicationFactor
                 epochPhoneCount += phoneCount * multiplicationFactor
-            
-            epochOutputList.append("%f,%f,%f" % (epochSyllableCount,
-                                                 epochPhoneCount,
-                                                 speechDuration))
-        
+
+            epochOutputList.append(
+                "%f,%f,%f" % (epochSyllableCount, epochPhoneCount, speechDuration)
+            )
+
         with open(join(outputPath, fn), "w") as fd:
             fd.write("\n".join(epochOutputList))
```

### Comparing `pyacoustics-1.0.7/pyacoustics/speech_rate/uwe_sr.py` & `pyacoustics-2.0.0/pyacoustics/speech_rate/uwe_sr.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,69 +1,72 @@
-'''
+"""
 Created on July 28, 2015
 
 @author: tmahrt
 
 This code estimates the speech rate of a speaker by using Uwe Reichel's matlab
 script for detecting syllable nuclei over some interval.
-'''
+"""
 
 from os.path import join
 
 from pyacoustics.utilities import utils
 from pyacoustics.utilities import matlab
 
 
-def findSyllableNuclei(inputPath, outputPath, matlabEXE,
-                       matlabScriptsPath, printCmd=False):
-    '''
+def findSyllableNuclei(
+    inputPath, outputPath, matlabEXE, matlabScriptsPath, printCmd=False
+):
+    """
     Makes a file listing the syllable nuclei for each file in inputPath
-    '''
+    """
     utils.makeDir(outputPath)
-    
-    pathList = [matlabScriptsPath,
-                join(matlabScriptsPath, "nucleus_detection_matlab")]
+
+    pathList = [matlabScriptsPath, join(matlabScriptsPath, "nucleus_detection_matlab")]
     cmd = "detect_syllable_nuclei('%s', '%s');" % (inputPath, outputPath)
     matlab.runMatlabFunction(cmd, matlabEXE, pathList, printCmd)
 
 
 def toAbsoluteTime(namePrefix, matlabOutputPath, startTimeList):
-    '''
+    """
     Converts the sampled times from relative to absolute time
-    
+
     The input may be split across a number of files.  This script assumes
     that files of the pattern <<namePrefix>><<nameSuffix>>.txt correspond
     to different parts of the same source file.
-    
+
     namePrefix - name of the original wav file with no suffix
     speechRatePath - the path where the output of the matlab script is placed
     startTimeList - there needs to be one file here for each file in
                     speechRatePath with the pattern namePrefix
-    
+
     Returns a list of lists where each sublist corresponds to the output of
     one file matching <<namePrefix>>
-    '''
+    """
     # Load subset speech rate
-    speechRateFNList = utils.findFiles(matlabOutputPath, filterExt=".txt",
-                                       filterPattern=namePrefix)
-    
+    speechRateFNList = utils.findFiles(
+        matlabOutputPath, filterExt=".txt", filterPattern=namePrefix
+    )
+
     returnList = []
-    for start, speechRateFN in utils.safeZip([startTimeList, speechRateFNList],
-                                             enforceLength=True):
-        speechRateList = utils.openCSV(matlabOutputPath,
-                                       speechRateFN,
-                                       valueIndex=0)
-        speechRateList = [value for value in speechRateList if value != '']
-        speechRateList = [str(float(start) + float(sampNum))
-                          for sampNum in speechRateList]
+    for start, speechRateFN in utils.safeZip(
+        [startTimeList, speechRateFNList], enforceLength=True
+    ):
+        speechRateList = utils.openCSV(matlabOutputPath, speechRateFN, valueIndex=0)
+        speechRateList = [value for value in speechRateList if value != ""]
+        speechRateList = [
+            str(float(start) + float(sampNum)) for sampNum in speechRateList
+        ]
 
         returnList.append(speechRateList)
-    
+
     return returnList
-    
+
 
 def uweSyllableCountForInterval(startTime, stopTime, nucleiCenterList):
+    countList = [
+        timestamp
+        for timestamp in nucleiCenterList
+        if timestamp >= startTime and timestamp <= stopTime
+    ]
 
-    countList = [timestamp for timestamp in nucleiCenterList
-                 if timestamp >= startTime and timestamp <= stopTime]
-    
     return len(countList)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/text/frequency.py` & `pyacoustics-2.0.0/pyacoustics/text/frequency.py`

 * *Files 9% similar despite different names*

```diff
@@ -59,38 +59,34 @@
         for word in self.frequencyDict.keys():
             sumV += self.frequencyDict[word]
 
         return sumV
 
 
 class GoogleUnigram(CountCorpus):
-
     NUM_WORDS = 1024908267229.0
 
     def __init__(self, googleUnigram):
-
         # Load the corpus data
         frequencyDict = {}
         with open(googleUnigram, "r") as fd:
             data = fd.read()
         dataList = data.split()
-        for (word, count) in zip(
+        for word, count in zip(
             islice(dataList, 0, None, 2), islice(dataList, 1, None, 2)
         ):
             frequencyDict[word] = count
 
         super(GoogleUnigram, self).__init__(frequencyDict, GoogleUnigram.NUM_WORDS)
 
 
 class Switchboard(CountCorpus):
-
     NUM_WORDS = 1456224.0
 
     def __init__(self, switchboardCounts):
-
         # Load the corpus
         frequencyDict = {}
         with open(switchboardCounts, "r") as fd:
             data = fd.read()
 
         dataList = data.split("\n")
         dataList = [
@@ -103,66 +99,60 @@
             count = row[-4]
             frequencyDict[word] = int(count)
 
         super(Switchboard, self).__init__(frequencyDict, Switchboard.NUM_WORDS)
 
 
 class SwitchboardTim(CountCorpus):
-
     NUM_WORDS = 1464017.0
 
     def __init__(self, switchboardCounts):
         frequencyDict = loadCountList(switchboardCounts)
         super(SwitchboardTim, self).__init__(frequencyDict, SwitchboardTim.NUM_WORDS)
 
 
 class Buckeye(CountCorpus):
-
     NUM_WORDS = 282575.0  # Not including words that start with '['
 
     def __init__(self, buckeyeCounts):
         frequencyDict = loadCountList(buckeyeCounts)
         super(Buckeye, self).__init__(frequencyDict, Buckeye.NUM_WORDS)
 
 
 class Fischer(CountCorpus):
-
     NUM_WORDS = 21025946.0
 
     def __init__(self, fischerCounts):
         frequencyDict = loadCountList(fischerCounts)
         super(Fischer, self).__init__(frequencyDict, Fischer.NUM_WORDS)
 
 
 class Crea(CountCorpus):
-
     NUM_WORDS = 152554665
 
     def __init__(self, creaCounts):
         frequencyDict = loadCountList(creaCounts)
         super(Crea, self).__init__(frequencyDict, Crea.NUM_WORDS)
 
 
 class FrenchCorpus(CountCorpus):
-
     NUM_WORDS = None
 
     def __init__(self, frenchCounts):
         frequencyDict = loadCountList(frenchCounts)
         super(FrenchCorpus, self).__init__(frequencyDict, 0)
 
 
 def calcWordsPerMillion(count, totalCount):
     million = 1000000
     assert totalCount > million
     return count * million / totalCount
 
 
 def loadFrenchList(fnFullPath, outputFullPath):
-
     with io.open(fnFullPath, "r", encoding="utf-8") as fd:
         data = fd.read()
     frequencyDict = {}
 
     dataList = data.splitlines()
     dataList = [row.rsplit(",") for row in dataList[1:]]
     dataList = [(rowList[0], float(rowList[6])) for rowList in dataList]
@@ -195,15 +185,14 @@
     for word, count in dataList:
         frequencyDict[word] = float(count)
 
     return frequencyDict
 
 
 def findFrequenciesForWordLists(featurePath, countObj, frequencyNormFunc):
-
     frequencyPath = join(featurePath, "frequency")
     utils.makeDir(frequencyPath)
 
     wordsPath = join(featurePath, "words")
 
     for fn in utils.findFiles(wordsPath):
         wordList = utils.openCSV(wordsPath, fn, valueIndex=0, encoding="utf-8")
```

### Comparing `pyacoustics-1.0.7/pyacoustics/text/transcript.py` & `pyacoustics-2.0.0/pyacoustics/text/transcript.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-'''
+"""
 Created on Oct 20, 2014
 
 @author: tmahrt
-'''
+"""
 
 from os.path import join
 
 import io
 
 from pyacoustics.utilities import utils
 
 
 def toWords(featurePath, outputPath):
-    
     utils.makeDir(outputPath)
 
     transcriptPath = join(featurePath, "txt")
 
     for fn in utils.findFiles(transcriptPath, filterExt=".txt"):
         fnFullPath = join(transcriptPath, fn)
         with io.open(fnFullPath, "r", encoding="utf-8") as fd:
             data = fd.read()
         dataList = data.split()
-        
+
         with io.open(join(outputPath, fn), "w", encoding="utf-8") as fd:
             fd.write("\n".join(dataList))
```

### Comparing `pyacoustics-1.0.7/pyacoustics/textgrids/syllabify_textgrids.py` & `pyacoustics-2.0.0/pyacoustics/textgrids/syllabify_textgrids.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,88 @@
-'''
+"""
 Created on Oct 22, 2014
 
 @author: tmahrt
-'''
+"""
 
 import os
 from os.path import join
 
-from praatio import tgio
+from praatio import textgrid
 from pysle import isletool
 from pysle import praattools
 
 
 from pyacoustics.utilities import utils
 
 
 def correctTextgridTimes(tgPath, threshold):
-    
     # Are x and y unique but very very similar
     withinThreshold = lambda x, y: (abs(x - y) < threshold) and (x != y)
-    
+
     outputPath = join(tgPath, "correctsTGs")
     utils.makeDir(outputPath)
-    
+
     for fn in utils.findFiles(tgPath, filterExt=".TextGrid"):
         print(fn)
-        tg = tgio.openTextgrid(join(tgPath, fn))
+        tg = textgrid.openTextgrid(join(tgPath, fn), includeEmptyIntervals=False)
         wordTier = tg.tierDict["words"]
         phoneTier = tg.tierDict["phones"]
-        
+
         for wordEntry in wordTier.entryList:
-            
             for i, phoneEntry in enumerate(phoneTier.entryList):
-                
-                if tgio.intervalOverlapCheck(wordEntry, phoneEntry):
-                    
+                if textgrid.intervalOverlapCheck(wordEntry, phoneEntry):
                     start = phoneEntry[0]
                     end = phoneEntry[1]
                     phone = phoneEntry[2]
-                    
+
                     if withinThreshold(wordEntry[0], start):
                         start = wordEntry[0]
                     elif withinThreshold(wordEntry[1], start):
                         start = wordEntry[1]
                     elif withinThreshold(wordEntry[0], end):
                         end = wordEntry[0]
                     elif withinThreshold(wordEntry[1], end):
                         end = wordEntry[1]
-                    
+
                     phoneTier.entryList[i] = (start, end, phone)
-        
-        tg.save(join(outputPath, fn))
 
+        tg.save(join(outputPath, fn), format="short_textgrid", includeBlankSpaces=True)
 
-def syllabifyTextgrids(tgPath, islePath):
 
+def syllabifyTextgrids(tgPath, islePath):
     isleDict = isletool.LexicalTool(islePath)
 
     outputPath = join(tgPath, "syllabifiedTGs")
     utils.makeDir(outputPath)
-    skipLabelList = ["<VOCNOISE>", "xx", "<SIL>", "{B_TRANS}", '{E_TRANS}']
+    skipLabelList = ["<VOCNOISE>", "xx", "<SIL>", "{B_TRANS}", "{E_TRANS}"]
 
     for fn in utils.findFiles(tgPath, filterExt=".TextGrid"):
-
         if os.path.exists(join(outputPath, fn)):
             continue
 
-        tg = tgio.openTextgrid(join(tgPath, fn))
-        
-        syllableTG = praattools.syllabifyTextgrid(isleDict, tg, "words",
-                                                  "phones",
-                                                  skipLabelList=skipLabelList)
-        
-        outputTG = tgio.Textgrid()
+        tg = textgrid.openTextgrid(join(tgPath, fn))
+
+        syllableTG = praattools.syllabifyTextgrid(
+            isleDict, tg, "words", "phones", skipLabelList=skipLabelList
+        )
+
+        outputTG = textgrid.Textgrid()
         outputTG.addTier(tg.tierDict["words"])
         outputTG.addTier(tg.tierDict["phones"])
-#         outputTG.addTier(syllableTG.tierDict["syllable"])
+        #         outputTG.addTier(syllableTG.tierDict["syllable"])
         outputTG.addTier(syllableTG.tierDict["tonic"])
-        
-        outputTG.save(join(outputPath, fn))
+
+        outputTG.save(
+            join(outputPath, fn), format="short_textgrid", includeBlankSpaces=True
+        )
+
 
 if __name__ == "__main__":
     tmpISLEPath = "/Users/tmahrt/Dropbox/workspace/pysle/test/islev2.txt"
-#     correctTextgridTimes(tgPath, 0.0025)
+    #     correctTextgridTimes(tgPath, 0.0025)
 
-    tmpTGPath = join("/Users/tmahrt/Desktop/experiments/LMEDS_studies",
-                     "RPT_English/features/tobi_textgrids/correctsTGs")
+    tmpTGPath = join(
+        "/Users/tmahrt/Desktop/experiments/LMEDS_studies",
+        "RPT_English/features/tobi_textgrids/correctsTGs",
+    )
     syllabifyTextgrids(tmpTGPath, tmpISLEPath)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/filters.py` & `pyacoustics-2.0.0/pyacoustics/utilities/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,65 @@
-'''
+"""
 Created on Oct 20, 2014
 
 @author: tmahrt
-'''
+"""
 
 import math
 
 
 def medianFilter(dist, window, useEdgePadding):
-    
     offset = int(math.floor(window / 2.0))
     length = len(dist)
 
     returnList = []
     for x in range(length):
         dataToFilter = []
         # If using edge padding or if 0 <= context <= length
         if useEdgePadding or (((0 <= x - offset) and (x + offset < length))):
-            
             preContext = []
-            currentContext = [dist[x], ]
+            currentContext = [
+                dist[x],
+            ]
             postContext = []
-            
+
             lastKnownLargeIndex = 0
             for y in range(1, offset + 1):  # 1-based
                 if x + y >= length:
                     if lastKnownLargeIndex == 0:
                         largeIndexValue = x
                     else:
                         largeIndexValue = lastKnownLargeIndex
                 else:
                     largeIndexValue = x + y
                     lastKnownLargeIndex = x + y
-                
+
                 postContext.append(dist[largeIndexValue])
-                
+
                 if x - y < 0:
                     smallIndexValue = 0
                 else:
                     smallIndexValue = x - y
-                    
+
                 preContext.insert(0, dist[smallIndexValue])
-                
+
             dataToFilter = preContext + currentContext + postContext
             value = _median(dataToFilter)
         else:
             value = dist[x]
         returnList.append(value)
-        
+
     return returnList
 
 
 def _median(valList):
-    
     valList = valList[:]
     valList.sort()
-    
+
     if len(valList) % 2 == 0:  # Even
         i = int(len(valList) / 2.0)
         medianVal = (valList[i - 1] + valList[i]) / 2.0
     else:  # Odd
         i = int(len(valList) / 2.0)
         medianVal = valList[i]
-        
+
     return medianVal
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/matlab.py` & `pyacoustics-2.0.0/pyacoustics/utilities/matlab.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-'''
+"""
 Created on Jul 28, 2015
 
 @author: tmahrt
-'''
+"""
 
 import subprocess
 
 from pyacoustics.utilities import error_utils
 
 
 def runMatlabFunction(command, matlabEXE, matlabCodePathList, printCmd=False):
     error_utils.checkForApplication(matlabEXE)
-    
-    pathCode = "".join(["addpath('%s');" % matlabCodePath
-                       for matlabCodePath in matlabCodePathList])
+
+    pathCode = "".join(
+        ["addpath('%s');" % matlabCodePath for matlabCodePath in matlabCodePathList]
+    )
     exitCode = "exit;"
-    
+
     codeSequence = pathCode + command + exitCode
 
     if printCmd is True:
         print(matlabEXE + ' -nosplash -nodesktop -r "%s"' % codeSequence)
-    myProcess = subprocess.Popen([matlabEXE, "-nosplash",
-                                  "-nodesktop", "-r", codeSequence])
+    myProcess = subprocess.Popen(
+        [matlabEXE, "-nosplash", "-nodesktop", "-r", codeSequence]
+    )
     if myProcess.wait():
         exit()  # Something has gone wrong (an error message should be printed)
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/normalize.py` & `pyacoustics-2.0.0/pyacoustics/utilities/normalize.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,101 @@
-'''
+"""
 Created on Oct 16, 2012
 
 @author: timmahrt
-'''
+"""
 
 import math
 
+
 def _zscoreNormalize(raw, mean, stdDev):
     # No problems related to integers or 64-bit floats (which don't trigger
     # a divide by zero exception)
     raw, mean, stdDev = float(raw), float(mean), float(stdDev)
     return (raw - mean) / stdDev
-    
+
 
 def zscoreNormalizeValue(value, distribution):
-    '''
+    """
     Appropriate to use when the context (the distribution) varies.
-    '''
+    """
     mean = sum(distribution) / len(distribution)
-    
+
     tmpList = [(tmpVal - mean) ** 2 for tmpVal in distribution]
     standardDeviation = math.sqrt(sum(tmpList) / len(tmpList))
-    
+
     return _zscoreNormalize(value, mean, standardDeviation)
 
 
 def syntagmaticNormalization(sampleIndexList, dataList, contextList):
-    '''
+    """
     Normalizes using local context (before and after the occurrence)
-    
+
     'sampleIndexList' contains the list of indices for values in 'contextList'
         that should be normalized.
     'contextList' provides the indices for all words that should be
         considered (including the present one)
         e.g. for +/- 2 words [-2, -1, 0, 1, 2]
     'featureExtractionFunc' provides the function that extracts the
         relevant feature to be normalized from the words (could be
         a word or syllable level feature)
-    '''
-    
+    """
+
     dataList = [float(value) for value in dataList]
-    
+
     def doSkipValue(value):
         return value == 0 or value == "None"
 
     # Get the files associated with this speaker
     #    - be patient, running retrieveStressIndex() takes some time the
     #      first time
-#    fnList = fetchFNsForSpeaker(speakerID)
+    #    fnList = fetchFNsForSpeaker(speakerID)
 
-    negativeContextList = [contextI for contextI in contextList
-                           if contextI < 0]
+    negativeContextList = [contextI for contextI in contextList if contextI < 0]
     negativeContextList.sort(reverse=True)
-    positiveContextList = [contextI for contextI in contextList
-                           if contextI > 0]
+    positiveContextList = [contextI for contextI in contextList if contextI > 0]
     positiveContextList.sort()
-    
+
     # Create index
     outputList = []
     for i in sampleIndexList:
         value = dataList[i]
-        
+
         # A value of 0.0 generally is not meaningful
         # (TODO: is there anywhere where this is not the case?)
         if i == -1 or doSkipValue(value):
             outputList.append(0)
             continue
-        
-        contextValueList = [dataList[i], ]
-        
-        for (incr, tmpContextList) in [(-1, negativeContextList[:]),
-                                       (1, positiveContextList[:])]:
+
+        contextValueList = [
+            dataList[i],
+        ]
+
+        for incr, tmpContextList in [
+            (-1, negativeContextList[:]),
+            (1, positiveContextList[:]),
+        ]:
             prevContextValue = dataList[i]
             for contextI in tmpContextList:
                 try:
-                    assert(i + contextI >= 0)
+                    assert i + contextI >= 0
                     subValue = dataList[i + contextI]
-                
+
                 # If we've gone outside the bounds of the file, just
                 # repeat the last known good value
                 except (IndexError, AssertionError):
                     contextValueList.append(prevContextValue)
                     continue
-                
+
                 # Don't count words with meaningless values as part
                 # of the context
                 if doSkipValue(subValue):
                     tmpContextList.append(tmpContextList[-1] + incr)
                     continue
-                
+
                 prevContextValue = subValue
                 contextValueList.append(subValue)
-                
+
         normalizedValue = zscoreNormalizeValue(value, contextValueList)
         outputList.append(normalizedValue)
-        
+
     return outputList
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/sequences.py` & `pyacoustics-2.0.0/pyacoustics/utilities/sequences.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,332 +1,346 @@
-'''
+"""
 Created on Jun 5, 2013
 
 @author: timmahrt
-'''
+"""
 import math
 
 from pyacoustics.utilities import my_math
 
 
 DO_SAMPLE_GATED = 1  # Each subsequence overlaps by (n-1)/2
 DO_SAMPLE_EXCLUSIVE = 2  # No index appears in two subsequences
 DO_SAMPLE_ALL = 3  # Each index acts as the control point once
 
 
 def compressList(targetList):
-    '''
+    """
     Compresses a list into pairs of the form (value, num_continuous_occurances)
-    
+
     e.g. targetList = [1, 1, 1, 1, 2, 2, 1, 1, 3]
     >> [(1,4), (2, 2), (1, 2), (3, 1),]
-    '''
-    
+    """
+
     currentValue = targetList[0]
     startIndex = 0
     i = 0
-    
+
     outputList = []
     while i < len(targetList):
         if targetList[i] == currentValue:
             i += 1
             continue
-        
+
         outputList.append([currentValue, startIndex, i])
-        
+
         currentValue = targetList[i]
         startIndex = i
         i += 1
-    
+
     if len(outputList) == 0 or outputList[-1][0] != currentValue:
         outputList.append([currentValue, startIndex, i])
-    
+
     print(len(targetList))
     print(outputList)
     return outputList
 
 
 def compressedListTransform(compressedList, timeStep, timeThreshold=None):
-    '''
+    """
     Isolates the unique values in compressedList and converts them to time
-    
+
     timeThreshold can be set to ignore values that are not long enough, adding
     their content to whatever came before (prevents fragmenting data too much).
-    '''
-    
+    """
+
     returnDict = {}
     countDict = {}
     lastGoodLabel = None
     for label, start, end in compressedList:
-     
         countDict.setdefault(label, 0)
         returnDict.setdefault(label, [])
-     
+
         startTime = start * timeStep
         endTime = end * timeStep
-        
+
         # Merge this entry with the previous one
         # if it is too short (noise tolerance)
         tmpDuration = (end - start) * timeStep
         if timeThreshold is not None and tmpDuration < timeThreshold:
-            
             # If the very first entry is less than 0.3 seconds long
             if lastGoodLabel is not None and returnDict[lastGoodLabel] != []:
                 returnDict[lastGoodLabel][-1][1] = endTime
                 continue
-        
+
         # If the previous label and this one are the same, merge entries
         if label == lastGoodLabel:
             returnDict[label][-1][1] = endTime
-            
+
         # Otherwise, create a new entry
         else:
-            returnDict[label].append([startTime, endTime,
-                                      str(countDict[label])])
+            returnDict[label].append([startTime, endTime, str(countDict[label])])
             countDict[label] += 1
             lastGoodLabel = label
-                
+
     return returnDict
 
 
 def sampleMiddle(dataList, i, chunkSize):
-    '''
+    """
     The control point lies in the center (i - 1 ) / 2.0
-    '''
-    assert((chunkSize % 2) == 1)  # i must be an odd number
+    """
+    assert (chunkSize % 2) == 1  # i must be an odd number
     halfChunk = int(math.floor(chunkSize / 2.0))
-    
+
     subList = []
     indexList = []
     start = i - halfChunk if i - halfChunk >= 0 else 0
     end = i + halfChunk if i + halfChunk < len(dataList) else len(dataList) - 1
-    
+
     # Handling underflow
     if i - halfChunk < 0:
-        subList += [dataList[0], ] * abs(i - halfChunk)
-        indexList += [0, ] * abs(i - halfChunk)
-    
+        subList += [
+            dataList[0],
+        ] * abs(i - halfChunk)
+        indexList += [
+            0,
+        ] * abs(i - halfChunk)
+
     # The normal range
     mainBody = [dataList[j] for j in range(start, end + 1)]
     uniqueChunkLen = len(mainBody)
     subList.extend(mainBody)
     indexList.extend([j for j in range(start, end + 1)])
-    
+
     # Handling overflow
     if i + halfChunk >= len(dataList):
-        subList += [dataList[len(dataList) - 1], ] * ((1 + i + halfChunk) -
-                                                      len(dataList))
-        indexList.extend([len(dataList) - 1, ] * ((1 + i + halfChunk -
-                                                   len(dataList))))
+        subList += [
+            dataList[len(dataList) - 1],
+        ] * ((1 + i + halfChunk) - len(dataList))
+        indexList.extend(
+            [
+                len(dataList) - 1,
+            ]
+            * ((1 + i + halfChunk - len(dataList)))
+        )
 
     return subList, indexList, uniqueChunkLen
 
 
 def sampleLeft(dataList, i, chunkSize):
-    '''
+    """
     The control point lies on the left edge (i = 0)
-    '''
+    """
     subList = []
     indexList = []
     start = i
     end = i + chunkSize if i + chunkSize < len(dataList) else len(dataList)
-    
+
     # The normal range
     mainBody = [dataList[j] for j in range(start, end)]
     uniqueChunkLen = len(mainBody)
     subList.extend(mainBody)
     indexList.extend([j for j in range(start, end)])
-    
+
     # Handling overflow
     if i + chunkSize >= len(dataList):
-        subList += [dataList[len(dataList) - 1], ] * ((1 + i + chunkSize) -
-                                                      len(dataList))
-        indexList += [len(dataList) - 1, ] * ((1 + i + chunkSize) -
-                                              len(dataList))
-        
+        subList += [
+            dataList[len(dataList) - 1],
+        ] * ((1 + i + chunkSize) - len(dataList))
+        indexList += [
+            len(dataList) - 1,
+        ] * ((1 + i + chunkSize) - len(dataList))
+
     return subList, indexList, uniqueChunkLen
 
 
 def sampleRight(dataList, i, chunkSize):
-    '''
+    """
     The control point lies on the right edge (i = -1)
-    '''
+    """
     subList = []
     indexList = []
     start = 1 + i - chunkSize if 1 + i - chunkSize >= 0 else 0
     end = i + 1 if i < len(dataList) else len(dataList)
-    
+
     # Handling underflow
-#     print("blah", abs(i - chunkSize), start, end)
+    #     print("blah", abs(i - chunkSize), start, end)
     if i - chunkSize < 0:
-        subList += [dataList[0], ] * (abs(i - chunkSize + 1))
-        indexList += [0, ] * (abs(i - chunkSize + 1))
-    
+        subList += [
+            dataList[0],
+        ] * (abs(i - chunkSize + 1))
+        indexList += [
+            0,
+        ] * (abs(i - chunkSize + 1))
+
     # The normal range
-#     print(start, end)
+    #     print(start, end)
     mainBody = [dataList[j] for j in range(start, end)]
     uniqueChunkLen = len(mainBody)
     subList.extend(mainBody)
     indexList.extend([j for j in range(start, end)])
-    
+
     # Handling overflow
     if i >= len(dataList):
-        subList += [dataList[len(dataList) - 1], ] * (chunkSize -
-                                                      len(indexList))
-        indexList += [len(dataList) - 1, ] * (chunkSize - len(indexList))
-    
+        subList += [
+            dataList[len(dataList) - 1],
+        ] * (chunkSize - len(indexList))
+        indexList += [
+            len(dataList) - 1,
+        ] * (chunkSize - len(indexList))
+
     return subList, indexList, uniqueChunkLen
 
 
 def subsequenceGenerator(dataList, chunkSize, sampleFunc, stepSizeFlag):
-    '''
+    """
     Can iteratively generate subsequences in a variety of fashions
-    
+
     chunkSize - the size of each chunk
     sampleFunc - e.g. sampleMiddle(), sampleLeft(), sampleRight(), determines
         the 'controlPoint'
     stepSize - the distance between starting points
-    
+
     Regardless of the parameters, all values will appear in one of the
     subsequences, including the endpoints.  Each subsequence is the same
     length--if necessary, values are repeated on the tail ends of the
     list
-    '''
-    
+    """
+
     if stepSizeFlag == DO_SAMPLE_EXCLUSIVE:
         stepSize = chunkSize
     elif stepSizeFlag == DO_SAMPLE_GATED:
         stepSize = int(math.floor(chunkSize / 2.0))
     elif stepSizeFlag == DO_SAMPLE_ALL:
         stepSize = 1
-    
+
     controlPoint = 0
     finalIndex = 0
     doneIterating = False
     while not doneIterating:
-        
-        subSequence, subSequenceIndices, sampledLen = sampleFunc(dataList,
-                                                                 controlPoint,
-                                                                 chunkSize)
-        
+        subSequence, subSequenceIndices, sampledLen = sampleFunc(
+            dataList, controlPoint, chunkSize
+        )
+
         finalIndex = subSequenceIndices[-1]
         isEndpointLastValue = finalIndex >= (len(dataList) - 1)
         isControlPointLastValue = controlPoint >= (len(dataList) - 1)
-        
+
         # Regardless of what the control point was, end when the last index
         # in the subset matches the length of the data list
         if stepSizeFlag == DO_SAMPLE_EXCLUSIVE:
             doneIterating = isEndpointLastValue
-        
+
         # When the control point index reaches the end of the data list
         # (i.e., all values have been represented in some list, end)
         else:
             doneIterating = isControlPointLastValue
 
         controlPoint += stepSize
 
         if stepSizeFlag == DO_SAMPLE_GATED:
-            
             if sampleFunc == sampleMiddle:
-                region = subSequenceIndices[int((chunkSize - 1) / 2.0):-1]
+                region = subSequenceIndices[int((chunkSize - 1) / 2.0) : -1]
             elif sampleFunc == sampleLeft:
-                region = subSequenceIndices[:int((chunkSize - 1) / 2.0)]
+                region = subSequenceIndices[: int((chunkSize - 1) / 2.0)]
             elif sampleFunc == sampleRight:
-                region = subSequenceIndices[int((chunkSize - 1) / 2.0) + 1:]
-            
+                region = subSequenceIndices[int((chunkSize - 1) / 2.0) + 1 :]
+
             sampledLen = int((chunkSize - 1) / 2.0)
             sampledLen = sampledLen - (sampledLen - len(set(region)))
-        
+
             if doneIterating and sampleFunc != sampleRight:
                 sampledLen = 0
-        
+
         yield subSequence, subSequenceIndices, sampledLen
-    
-    
+
+
 def interp(start, stop, n):
     for i in range(n):
         yield start + i * (stop - start) / float(n - 1)
 
 
 # Adapted this from online - for getting a set of evenly spaced intervals
 # from a list
 # http://stackoverflow.com/questions/10084436/generating-evenly-distributed-
 # multiples-samples-within-a-range
 def getEvenlySpacedSteps(start, end, n):
-    
-    assert (end + 1 - start >= n)
-    
+    assert end + 1 - start >= n
+
     # The usual case
     if n != 1:
         step = (end - start) / float(n - 1)
         retList = [int(round(start + x * step)) for x in range(n)]
-        
+
     # If someone only wants 1 sample, just take the middle sample
     elif n == 1:
         step = (end - start) / float(2)
-        retList = [int(round((end - start) / float(2))), ]
-    
+        retList = [
+            int(round((end - start) / float(2))),
+        ]
+
     return retList
 
 
 def binDistribution(distList, numBins, minV=None, maxV=None):
-    '''
+    """
     Places all data into the closest of n evenly spaced bins
-    '''
-    
+    """
+
     if minV is None:
         minV = min(distList)
-    
+
     if maxV is None:
         maxV = max(distList)
-        
+
     binValueArray = my_math.linspace(minV, maxV, numBins)
-    
+
     binnedValueList = []
     for value in distList:
         diffList = list(abs(binValueArray - value))
         smallestDiff = min(diffList)
         binIndex = diffList.index(smallestDiff)
-        
+
         binnedValueList.append(binValueArray[binIndex])
-    
+
     return binnedValueList
 
 
 def findLongestSublist(listOfLists):
     longestList = []
     i = None
     for i, lst in enumerate(listOfLists):
         if len(lst) > len(longestList):
             longestList = lst
 
     return i, longestList
 
 
 def invertIntervalList(entryList, minValue=0, maxValue=None):
-    '''
+    """
     Given a list of ordinal events, inverts the start and end positions
-    
+
     e.g. input [(5, 6), (10, 13), (14, 16)]
          output [(0, 5), (6, 10), (13, 14)]
-    '''
+    """
     if entryList == []:
         return []
 
     newEntryList = []
     i = 0
-    
+
     # Add possible initial interval
     if minValue is not None:
         if entryList[0][0] > minValue:
             newEntryList.append((minValue, entryList[0][0]))
-    
+
     while i + 1 < len(entryList):
         newEntryList.append((entryList[i][1], entryList[i + 1][0]))
         i += 1
-        
+
     # Add possible trailing interval
     if maxValue is not None:
         if entryList[i][1] < maxValue:
             newEntryList.append((entryList[i][1], maxValue))
-            
+
     return newEntryList
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/statistics.py` & `pyacoustics-2.0.0/pyacoustics/utilities/statistics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,68 @@
-'''
+"""
 Created on Apr 2, 2015
 
 @author: tmahrt
-'''
+"""
 
 import math
 
 
 def medianFilter(dist, window, useEdgePadding):
-    
     offset = int(math.floor(window / 2.0))
     length = len(dist)
 
     returnList = []
     for x in range(length):
         dataToFilter = []
         # If using edge padding or if 0 <= context <= length
         if useEdgePadding or (((0 <= x - offset) and (x + offset < length))):
-            
             preContext = []
-            currentContext = [dist[x], ]
+            currentContext = [
+                dist[x],
+            ]
             postContext = []
-            
+
             lastKnownLargeIndex = 0
             for y in range(1, offset + 1):  # 1-based
                 if x + y >= length:
                     if lastKnownLargeIndex == 0:
                         largeIndexValue = x
                     else:
                         largeIndexValue = lastKnownLargeIndex
                 else:
                     largeIndexValue = x + y
                     lastKnownLargeIndex = x + y
-                
+
                 postContext.append(dist[largeIndexValue])
-                
+
                 if x - y < 0:
                     smallIndexValue = 0
                 else:
                     smallIndexValue = x - y
-                    
+
                 preContext.insert(0, dist[smallIndexValue])
-                
+
             dataToFilter = preContext + currentContext + postContext
             value = getMedian(dataToFilter)
         else:
             value = dist[x]
-        
+
         returnList.append(value)
-        
+
     return returnList
 
 
 def getMedian(dist):
-    
-    assert(len(dist) > 0)
-    
+    assert len(dist) > 0
+
     dist = sorted(dist)
     length = len(dist)
-    
+
     halfPoint = int(length / 2.0)
-    
+
     if length % 2 == 0:
         median = (dist[halfPoint - 1] + dist[halfPoint]) / 2.0
     else:
         median = dist[halfPoint]
-        
+
     return median
```

### Comparing `pyacoustics-1.0.7/pyacoustics/utilities/utils.py` & `pyacoustics-2.0.0/pyacoustics/utilities/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-'''
+"""
 Created on Oct 11, 2012
 
 @author: timmahrt
-'''
+"""
 
 import os
 from os.path import join
 
 import functools
 import itertools
 import shutil
@@ -17,166 +17,188 @@
 pyAcousticsPath = os.path.split(inspect.getfile(inspect.currentframe()))[0]
 # Get out of the 'utilities' folder
 pyAcousticsPath = os.path.split(pyAcousticsPath)[0]
 scriptsPath = join(pyAcousticsPath, "praatScripts")
 
 
 def _getMatchFunc(pattern):
-    '''
+    """
     An unsophisticated pattern matching function
-    '''
-    
+    """
+
     # '#' Marks word boundaries, so if there is more than one we need to do
     #    something special to make sure we're not mis-representings them
-    assert(pattern.count('#') < 2)
+    assert pattern.count("#") < 2
 
     def startsWith(subStr, fullStr):
-        return fullStr[:len(subStr)] == subStr
-            
+        return fullStr[: len(subStr)] == subStr
+
     def endsWith(subStr, fullStr):
-        return fullStr[-1 * len(subStr):] == subStr
-    
+        return fullStr[-1 * len(subStr) :] == subStr
+
     def inStr(subStr, fullStr):
         return subStr in fullStr
 
     # Selection of the correct function
-    if pattern[0] == '#':
+    if pattern[0] == "#":
         pattern = pattern[1:]
         cmpFunc = startsWith
-        
-    elif pattern[-1] == '#':
+
+    elif pattern[-1] == "#":
         pattern = pattern[:-1]
         cmpFunc = endsWith
-        
+
     else:
         cmpFunc = inStr
-    
+
     return functools.partial(cmpFunc, pattern)
 
 
-def findFiles(path, filterPaths=False, filterExt=None, filterPattern=None,
-              skipIfNameInList=None, stripExt=False):
-    
+def findFiles(
+    path,
+    filterPaths=False,
+    filterExt=None,
+    filterPattern=None,
+    skipIfNameInList=None,
+    stripExt=False,
+):
     fnList = os.listdir(path)
-       
+
     if filterPaths is True:
-        fnList = [folderName for folderName in fnList
-                  if os.path.isdir(os.path.join(path, folderName))]
+        fnList = [
+            folderName
+            for folderName in fnList
+            if os.path.isdir(os.path.join(path, folderName))
+        ]
 
     if filterExt is not None:
-        splitFNList = [[fn, ] + list(os.path.splitext(fn)) for fn in fnList]
+        splitFNList = [
+            [
+                fn,
+            ]
+            + list(os.path.splitext(fn))
+            for fn in fnList
+        ]
         fnList = [fn for fn, name, ext in splitFNList if ext == filterExt]
-        
+
     if filterPattern is not None:
-        splitFNList = [[fn, ] + list(os.path.splitext(fn)) for fn in fnList]
+        splitFNList = [
+            [
+                fn,
+            ]
+            + list(os.path.splitext(fn))
+            for fn in fnList
+        ]
         matchFunc = _getMatchFunc(filterPattern)
         fnList = [fn for fn, name, ext in splitFNList if matchFunc(name)]
-    
+
     if skipIfNameInList is not None:
         targetNameList = [os.path.splitext(fn)[0] for fn in skipIfNameInList]
-        fnList = [fn for fn in fnList
-                  if os.path.splitext(fn)[0] not in targetNameList]
-    
+        fnList = [fn for fn in fnList if os.path.splitext(fn)[0] not in targetNameList]
+
     if stripExt is True:
         fnList = [os.path.splitext(fn)[0] for fn in fnList]
-    
+
     fnList.sort()
     return fnList
-    
+
 
 def openCSV(path, fn, valueIndex=None, encoding="utf-8"):
-    '''
+    """
     Load a feature
-    
+
     In many cases we only want a single value from the feature (mainly because
     the feature only contains one value).  In these situations, the user
     can indicate that rather than receiving a list of lists, they can receive
     a lists of values, where each value represents the item in the row
     indicated by valueIndex.
-    '''
-    
+    """
+
     # Load CSV file
     with io.open(join(path, fn), "r", encoding=encoding) as fd:
         featureList = fd.read().splitlines()
     featureList = [row.split(",") for row in featureList]
-    
+
     if valueIndex is not None:
         featureList = [row[valueIndex] for row in featureList]
-    
+
     return featureList
 
 
 def changeFileType(path, fromExt, toExt):
-    
     if fromExt[0] != ".":
         fromExt = "." + fromExt
     if toExt[0] != ".":
         toExt = "." + toExt
-        
+
     for fn in os.listdir(path):
         name, ext = os.path.splitext(fn)
         if ext == fromExt:
             shutil.move(join(path, fn), join(path, name + toExt))
 
 
 def makeDir(path):
     if not os.path.exists(path):
         os.mkdir(path)
 
 
 def extractLines(path, matchStr, outputDir="output"):
-    
     outputPath = join(path, outputDir)
     makeDir(outputPath)
-    
+
     for fn in findFiles(path, filterExt=".csv"):
-        with io.open(join(path, fn), "r", encoding='utf-8') as fd:
+        with io.open(join(path, fn), "r", encoding="utf-8") as fd:
             data = fd.read()
         dataList = data.split("\n")
-        
+
         dataList = [line for line in dataList if matchStr in line]
-        
-        with io.open(join(outputPath, fn), "w", encoding='utf-8') as fd:
+
+        with io.open(join(outputPath, fn), "w", encoding="utf-8") as fd:
             fd.write("\n".join(dataList))
 
 
 def cat(fn1, fn2, outputFN):
-    with io.open(fn1, 'r', encoding='utf-8') as fd:
+    with io.open(fn1, "r", encoding="utf-8") as fd:
         txt1 = fd.read()
-    with io.open(fn2, 'r', encoding='utf-8') as fd:
+    with io.open(fn2, "r", encoding="utf-8") as fd:
         txt2 = fd.read()
-    
-    with io.open(outputFN, 'w', encoding='utf-8') as fd:
+
+    with io.open(outputFN, "w", encoding="utf-8") as fd:
         fd.write(txt1 + txt2)
 
 
 def catAll(path, ext, ensureNewline=False):
     outputPath = join(path, "cat_output")
     makeDir(outputPath)
 
     outputList = []
     for fn in findFiles(path, filterExt=ext):
-        with io.open(join(path, fn), "r", encoding='utf-8') as fd:
+        with io.open(join(path, fn), "r", encoding="utf-8") as fd:
             data = fd.read()
 
         if ensureNewline and data[-1] != "\n":
             data += "\n"
 
         outputList.append(data)
 
     outputTxt = "".join(outputList)
     outputFN = join(outputPath, "catFiles" + ext)
-    with io.open(outputFN, "w", encoding='utf-8') as fd:
+    with io.open(outputFN, "w", encoding="utf-8") as fd:
         fd.write(outputTxt)
 
 
 def whatever(path):
     outputList = []
     for fn in findFiles(path, filterExt=".txt"):
-        outputList.extend([fn, ] * 30)
+        outputList.extend(
+            [
+                fn,
+            ]
+            * 30
+        )
 
     for fn in outputList:
         print(fn)
 
 
 def divide(numerator, denominator, zeroValue):
     if denominator == 0:
@@ -184,13 +206,12 @@
     else:
         retValue = numerator / float(denominator)
 
     return retValue
 
 
 def safeZip(listOfLists, enforceLength):
-
     if enforceLength is True:
         length = len(listOfLists[0])
-        assert(all([length == len(subList) for subList in listOfLists]))
+        assert all([length == len(subList) for subList in listOfLists])
 
     return itertools.izip_longest(*listOfLists)
```

### Comparing `pyacoustics-1.0.7/pyacoustics.egg-info/SOURCES.txt` & `pyacoustics-2.0.0/pyacoustics.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+LICENSE
 MANIFEST.in
-README.rst
+README.md
 setup.py
 praatScripts/get_pitch_and_intensity.praat
 praatScripts/psolaPitch.praat
 pyacoustics/__init__.py
 pyacoustics/aggregate_features.py
 pyacoustics.egg-info/PKG-INFO
 pyacoustics.egg-info/SOURCES.txt
```

