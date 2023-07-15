# Comparing `tmp/raya-3.5.2.dev0.tar.gz` & `tmp/raya-3.5.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raya-3.5.2.dev0.tar", last modified: Thu Jun 22 19:35:57 2023, max compression
+gzip compressed data, was "raya-3.5.3.dev0.tar", last modified: Sat Jul 15 16:23:29 2023, max compression
```

## Comparing `raya-3.5.2.dev0.tar` & `raya-3.5.3.dev0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.784581 raya-3.5.2.dev0/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-22 19:35:57.784581 raya-3.5.2.dev0/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/README.md
--rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/pyproject.toml
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-22 19:35:57.784581 raya-3.5.2.dev0/setup.cfg
--rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/setup.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/
--rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-06-22 19:35:47.000000 raya-3.5.2.dev0/src/raya/_version.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3183 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/application_base.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      672 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/constants.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/controllers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/controllers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya/controllers/analytics_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    26134 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya/controllers/arms_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      952 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/base_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/base_pseudo_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1289 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/cameras_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/communication_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/cv_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1387 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/fleet_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/grasping_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/interactions_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1298 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/leds_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1171 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/lidar_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/manipulation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2545 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/motion_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     7242 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/navigation_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1367 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/sensors_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya/controllers/skills_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2622 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/sound_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      668 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/controllers/status_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     9373 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya/controllers/ui_controller.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/entry_point.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     5581 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/enumerations.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    14002 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/exceptions.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     6730 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/exceptions_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/handlers/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/handlers/cv/__init__.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1211 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      802 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1168 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      312 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      792 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      713 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/estimators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.2.dev0/src/raya/handlers/cv/estimators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1069 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      316 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      197 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/model_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      843 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1190 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      807 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      796 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1201 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/handlers/general/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/handlers/general/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/handlers/general/callback_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/listeners/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/listeners/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/listeners/lidar_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/listeners/sensors_listeners.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      408 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/logger.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2165 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/raya_interface.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/standalone_handler.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya/tools/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.2.dev0/src/raya/tools/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      399 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/tools/filesystem.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      984 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/tools/fsm.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      294 2023-06-22 19:35:56.000000 raya-3.5.2.dev0/src/raya/tools/image.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-06-22 19:35:57.780581 raya-3.5.2.dev0/src/raya.egg-info/
--rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya.egg-info/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)     2698 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya.egg-info/SOURCES.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya.egg-info/dependency_links.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-06-22 19:35:57.000000 raya-3.5.2.dev0/src/raya.egg-info/top_level.txt
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)      150 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/README.md
+-rw-rw-r--   0 prod      (1001) prod      (1001)      103 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/pyproject.toml
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2752 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.296521 raya-3.5.3.dev0/src/
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.296521 raya-3.5.3.dev0/src/raya/
+-rw-rw-r--   0 prod      (1001) prod      (1001)       38 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2023-07-15 16:23:19.000000 raya-3.5.3.dev0/src/raya/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3177 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/application_base.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      698 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/controllers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/controllers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      260 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya/controllers/analytics_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    26366 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/arms_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      952 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/base_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       90 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/base_pseudo_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1289 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/cameras_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      425 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/communication_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2934 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/cv_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1399 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/fleet_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      523 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/grasping_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      924 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/interactions_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1322 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/leds_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1114 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/lidar_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3127 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/manipulation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2563 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/motion_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7382 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/navigation_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1613 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/sensors_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      808 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya/controllers/skills_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2622 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/sound_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      863 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/controllers/status_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8338 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya/controllers/ui_controller.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       59 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/entry_point.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7884 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/enumerations.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    14121 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6730 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/exceptions_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/handlers/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/handlers/cv/__init__.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1211 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      802 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1168 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      312 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/faces_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      792 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      713 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/estimators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.3.dev0/src/raya/handlers/cv/estimators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1069 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/estimators/estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      316 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/estimators/hand_estimator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      197 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/model_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      843 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1190 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-08 01:23:36.000000 raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      807 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      796 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1201 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/handlers/general/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/handlers/general/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      330 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/handlers/general/callback_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/listeners/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/listeners/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       77 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/listeners/lidar_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      160 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/listeners/sensors_listeners.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1026 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2165 2023-07-15 16:23:27.000000 raya-3.5.3.dev0/src/raya/raya_interface.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      257 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/standalone_handler.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.300521 raya-3.5.3.dev0/src/raya/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2023-06-07 02:42:34.000000 raya-3.5.3.dev0/src/raya/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      393 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/tools/filesystem.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1629 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/tools/fsm.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      294 2023-07-15 16:23:28.000000 raya-3.5.3.dev0/src/raya/tools/image.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2023-07-15 16:23:29.296521 raya-3.5.3.dev0/src/raya.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      568 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2698 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        5 2023-07-15 16:23:29.000000 raya-3.5.3.dev0/src/raya.egg-info/top_level.txt
```

### Comparing `raya-3.5.2.dev0/PKG-INFO` & `raya-3.5.3.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.5.2.dev0
+Version: 3.5.3.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.5.2.dev0/setup.py` & `raya-3.5.3.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/application_base.py` & `raya-3.5.3.dev0/src/raya/application_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pathlib
 from typing import Union
 from raya.exceptions import *
-from raya.logger import create_logger
+from raya.logger import RaYaLogger
 from raya.controllers.analytics_controller import AnalyticsController
 from raya.controllers.arms_controller import ArmsController
 from raya.controllers.cameras_controller import CamerasController
 from raya.controllers.communication_controller import CommunicationController
 from raya.controllers.cv_controller import CVController
 from raya.controllers.fleet_controller import FleetController
 from raya.controllers.manipulation_controller import ManipulationController
@@ -24,15 +24,15 @@
 except_no_print_bases = [pathlib.Path(__file__).parent.resolve()]
 DEPRECATED_CONTROLLER_NAMES = {'grasping': 'manipulation'}
 
 
 class RayaApplicationBase():
 
     def __init__(self, exec_settings):
-        self.log = create_logger(f'RayaApp.app.{self.__app_id}')
+        self.log = RaYaLogger(f'RayaApp.app.{self.__app_id}')
 
     @__only_in_args_getting('get_argument')
     def get_argument(self,
                      *name_or_flags: str,
                      type=str,
                      required: bool = False,
                      help: str = None,
```

### Comparing `raya-3.5.2.dev0/src/raya/constants.py` & `raya-3.5.3.dev0/src/raya/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 GET_SERVER_INFO_TIMEOUT = 0.1
 PATH_DATA_FOLDER = os.getenv('RAYA_APPS_DATA')
 PATH_RESOURCES_FOLDER = Path('res')
 SERVER_APP_NAMES = ['_ggs']
 MAIN_SERVER_APP = '_ggs'
 ROS_APPS_NAMESPACE = '/raya/apps'
 DEFAULT_COMMAND_TIMEOUT = 2.0
+CANCELATION_TIMEOUT = 2.0
 CONTROLLER_INIT_TIMEOUT = 10.0
 CONTROLLER_INIT_WAIT_PERIOD = 0.1
 CONTROLLER_INIT_TIMEOUT_TICKS = int(
     (CONTROLLER_INIT_TIMEOUT / CONTROLLER_INIT_WAIT_PERIOD))
 CONTROLLER_WAIT_PERIOD = 0.02
 LISTENER_SENSOR_DEBOUNCE_TIME = 1.0
 ROBOT_ID = 'ROBOT_ID'
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/arms_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/arms_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from rclpy.node import Node
 import typing
 from raya.controllers.base_controller import BaseController
 from raya.logger import DEPRECATION_NEW_METHOD
-from raya.enumerations import ANG_UNIT, MANAGE_ACTIONS
+from raya.enumerations import ANGLE_UNIT, ARMS_MANAGE_ACTIONS
 
 
 class ArmsController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info={}):
         pass
 
@@ -44,48 +44,56 @@
     async def get_predefined_trajectories_list(self):
         return
 
     @DEPRECATION_NEW_METHOD('get_predefined_trajectories_list')
     async def get_list_predefined_trajectories(self):
         pass
 
-    def get_joints_limits(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+    def get_joints_limits(self,
+                          arm: str,
+                          units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         return
 
     @DEPRECATION_NEW_METHOD('get_joints_limits')
-    def get_limits_of_joints(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+    def get_limits_of_joints(self,
+                             arm: str,
+                             units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     def get_arm_state(self, arm: str):
         return
 
     @DEPRECATION_NEW_METHOD('get_arm_state')
     def get_state_of_arm(self, arm: str):
         pass
 
-    async def get_current_joints_position(self,
-                                          arm: str,
-                                          units: ANG_UNIT = ANG_UNIT.DEG,
-                                          as_dict: bool = False):
+    async def get_current_joints_position(
+            self,
+            arm: str,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
+            as_dict: bool = False):
         pass
 
     @DEPRECATION_NEW_METHOD('get_current_joints_position')
     async def get_current_joint_values(self,
                                        arm: str,
-                                       units: ANG_UNIT = ANG_UNIT.DEG,
+                                       units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                                        as_dict: bool = False):
         pass
 
-    async def get_current_joint_position(self,
-                                         arm: str,
-                                         joint: str,
-                                         units: ANG_UNIT = ANG_UNIT.DEG):
+    async def get_current_joint_position(
+            self,
+            arm: str,
+            joint: str,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         return
 
-    async def get_current_pose(self, arm: str, units: ANG_UNIT = ANG_UNIT.DEG):
+    async def get_current_pose(self,
+                               arm: str,
+                               units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         return
 
     async def is_pose_valid(self,
                             arm: str,
                             x: float,
                             y: float,
                             z: float,
@@ -100,15 +108,15 @@
                             start_yaw: float = 0.0,
                             start_joints: list = [],
                             name_start_joints: list = [],
                             use_start_pose: bool = False,
                             use_start_joints: bool = False,
                             cartesian_path: bool = False,
                             tilt_constraint: bool = False,
-                            units: ANG_UNIT = ANG_UNIT.DEG,
+                            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                             use_obstacles: bool = False,
                             cameras: list = [],
                             update_obstacles: bool = False,
                             min_bbox_clear_obstacles: list = [],
                             max_bbox_clear_obstacles: list = [],
                             save_trajectory: bool = False,
                             name_trajectory: str = '',
@@ -135,15 +143,15 @@
                               start_qy: float = 0.0,
                               start_qz: float = 0.0,
                               start_qw: float = 0.0,
                               start_joints: list = [],
                               name_start_joints: list = [],
                               use_start_pose: bool = False,
                               use_start_joints: bool = False,
-                              units: ANG_UNIT = ANG_UNIT.DEG,
+                              units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                               cartesian_path: bool = False,
                               tilt_constraint: bool = False,
                               use_obstacles: bool = False,
                               cameras: list = [],
                               update_obstacles: bool = False,
                               min_bbox_clear_obstacles: list = [],
                               max_bbox_clear_obstacles: list = [],
@@ -163,15 +171,15 @@
         return
 
     async def is_joints_position_valid(
             self,
             arm: str,
             name_joints: list,
             angle_joints: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             start_joints: list = [],
             name_start_joints: list = [],
             use_start_joints: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
@@ -188,15 +196,15 @@
 
     @DEPRECATION_NEW_METHOD('is_joints_position_valid')
     async def are_joints_position_valid(
             self,
             arm: str,
             name_joints: list,
             angle_joints: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             start_joints: list = [],
             name_start_joints: list = [],
             use_start_joints: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
@@ -218,22 +226,22 @@
         return
 
     async def manage_predefined_pose(
             self,
             arm: str,
             name: str,
             position: list = [],
-            action: MANAGE_ACTIONS = MANAGE_ACTIONS.CREATE,
-            units: ANG_UNIT = ANG_UNIT.DEG):
+            action: ARMS_MANAGE_ACTIONS = ARMS_MANAGE_ACTIONS.CREATE,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     async def manage_predefined_trajectory(
             self,
             name: str,
-            action: MANAGE_ACTIONS = MANAGE_ACTIONS.GET_INFORMATION):
+            action: ARMS_MANAGE_ACTIONS = ARMS_MANAGE_ACTIONS.GET_INFORMATION):
         pass
 
     async def set_predefined_pose(
             self,
             arm: str,
             predefined_pose: str,
             tilt_constraint: bool = False,
@@ -254,15 +262,15 @@
         return
 
     async def set_joints_position(
             self,
             arm: str,
             name_joints: list,
             angle_joints: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
@@ -277,15 +285,15 @@
         return
 
     async def set_joint_position(
             self,
             arm: str,
             joint: list,
             position: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
@@ -304,15 +312,15 @@
                        x: float = None,
                        y: float = None,
                        z: float = None,
                        roll: float = None,
                        pitch: float = None,
                        yaw: float = None,
                        pose_dict: dict = None,
-                       units: ANG_UNIT = ANG_UNIT.DEG,
+                       units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                        cartesian_path: bool = False,
                        tilt_constraint: bool = False,
                        use_obstacles: bool = False,
                        cameras: list = [],
                        update_obstacles: bool = False,
                        min_bbox_clear_obstacles: list = [],
                        max_bbox_clear_obstacles: list = [],
@@ -419,15 +427,15 @@
         pass
 
     async def execute_joints_positions_array(
             self,
             arm: str,
             joint_values: list,
             name_joints_array: list = [],
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
@@ -443,15 +451,15 @@
 
     @DEPRECATION_NEW_METHOD('execute_joints_positions_array')
     async def execute_joint_values_array(
             self,
             arm: str,
             joint_values: list,
             name_joints_array: list = [],
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
@@ -465,15 +473,15 @@
             wait=False):
         pass
 
     async def execute_poses_array(
             self,
             arm: str,
             poses: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             cartesian_path: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             save_trajectory: bool = False,
             name_trajectory: str = '',
@@ -489,15 +497,15 @@
         pass
 
     @DEPRECATION_NEW_METHOD('execute_poses_array')
     async def execute_pose_array(
             self,
             arm: str,
             poses: list,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             cartesian_path: bool = False,
             tilt_constraint: bool = False,
             use_obstacles: bool = False,
             cameras: list = [],
             update_obstacles: bool = False,
             save_trajectory: bool = False,
             name_trajectory: str = '',
@@ -569,15 +577,15 @@
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
             wait: bool = False):
         return
 
@@ -594,15 +602,15 @@
             update_obstacles: bool = False,
             min_bbox_clear_obstacles: list = [],
             max_bbox_clear_obstacles: list = [],
             save_trajectory: bool = False,
             name_trajectory: str = '',
             velocity_scaling: float = 0.0,
             acceleration_scaling: float = 0.0,
-            units: ANG_UNIT = ANG_UNIT.DEG,
+            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
             wait: bool = False):
         pass
 
@@ -631,36 +639,36 @@
         pass
 
     async def add_collision_object(self,
                                    id: str,
                                    types: list,
                                    dimensions: list,
                                    shapes_poses: list,
-                                   units: ANG_UNIT = ANG_UNIT.DEG):
+                                   units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     async def remove_collision_object(self,
                                       id: str = '',
                                       remove_all_objects: bool = True):
         pass
 
     async def add_constraints(self,
                               arm: str,
                               joint_constraints: list = [],
                               orientation_constraints: list = [],
                               position_constraints: list = [],
-                              units: ANG_UNIT = ANG_UNIT.DEG):
+                              units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     async def remove_constraints(self, arm: str = ''):
         pass
 
     def convert_orientation(self,
                             orientation: dict,
-                            units: ANG_UNIT = ANG_UNIT.DEG):
+                            units: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     def convert_angle_joints_to_radians(self, arm: str, name_joints: list,
                                         angle_joints: list):
         return
 
     def convert_angle_joints_to_degrees(self, arm: str, name_joints: list,
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/base_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/base_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/cameras_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/cameras_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/cv_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/cv_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/fleet_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/fleet_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,22 +13,22 @@
                              title,
                              message,
                              timeout: float = 30.0,
                              task_id=None):
         pass
 
     async def finish_task(self,
-                          result: FINISH_STATUS = None,
+                          result: FLEET_FINISH_STATUS = None,
                           message: str = None,
                           task_id=None):
         return
 
     async def update_app_status(self,
                                 task_id: int = None,
-                                status: UPDATE_STATUS = None,
+                                status: FLEET_UPDATE_STATUS = None,
                                 message: str = None):
         return
 
     async def get_path(self, x: float, y: float, origin: str = None):
         return
 
     async def can_navigate(self,
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/grasping_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/grasping_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/interactions_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/interactions_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/leds_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/leds_controller.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 from raya.controllers.base_controller import BaseController
 from rclpy.node import Node
-from raya.enumerations import EXECUTION_CONTROL
+from raya.enumerations import LEDS_EXECUTION_CONTROL
 
 
 class LedsController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info):
         pass
 
@@ -24,15 +24,16 @@
     async def animation(
             self,
             group: str,
             color: str,
             animation: str,
             speed: int = 1,
             repetitions: int = 1,
-            execution_control: EXECUTION_CONTROL = EXECUTION_CONTROL.OVERRIDE,
+            execution_control: LEDS_EXECUTION_CONTROL = LEDS_EXECUTION_CONTROL.
+        OVERRIDE,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
             wait=True) -> None:
         return
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/lidar_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/lidar_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from rclpy.node import Node
-from raya.enumerations import ANG_UNIT
+from raya.enumerations import ANGLE_UNIT
 from raya.controllers.base_controller import BaseController
 
 
 class LidarController(BaseController):
 
     def __init__(self, name: str, node: Node, interface, extra_info):
         pass
 
-    def get_laser_info(self, ang_unit: ANG_UNIT = ANG_UNIT.DEG) -> dict:
+    def get_laser_info(self,
+                       ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES) -> dict:
         return
 
     def get_raw_data(self):
         return
 
     def check_obstacle(self,
                        lower_angle: float,
                        upper_angle: float,
                        lower_distance: float = 0.0,
                        upper_distance: float = float('inf'),
-                       ang_unit: ANG_UNIT = ANG_UNIT.DEG) -> bool:
+                       ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES) -> bool:
         return
 
-    def create_obstacle_listener(self,
-                                 listener_name: str,
-                                 callback: callable,
-                                 lower_angle: float,
-                                 upper_angle: float,
-                                 lower_distance: float = 0.0,
-                                 upper_distance: float = float('inf'),
-                                 ang_unit: ANG_UNIT = ANG_UNIT.DEG) -> None:
+    def create_obstacle_listener(
+            self,
+            listener_name: str,
+            lower_angle: float,
+            upper_angle: float,
+            callback=None,
+            callback_async=None,
+            lower_distance: float = 0.0,
+            upper_distance: float = float('inf'),
+            ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES) -> None:
         pass
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/manipulation_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/manipulation_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/motion_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/motion_controller.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 from rclpy.node import Node
 from raya.controllers.base_controller import BaseController
-from raya.enumerations import ANG_UNIT
+from raya.enumerations import ANGLE_UNIT
 
 
 class MotionController(BaseController):
 
     def __init__(self, name: str, node: Node, app, extra_info={}):
         pass
 
@@ -19,15 +19,15 @@
 
     async def set_velocity(self,
                            x_velocity: float,
                            y_velocity: float,
                            angular_velocity: float,
                            duration: float,
                            enable_obstacles: bool = True,
-                           ang_unit: ANG_UNIT = ANG_UNIT.DEG,
+                           ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                            callback_feedback: typing.Callable = None,
                            callback_feedback_async: typing.Callable = None,
                            callback_finish: typing.Callable = None,
                            callback_finish_async: typing.Callable = None,
                            wait: bool = False):
         pass
 
@@ -42,15 +42,15 @@
                           enable_obstacles: bool = True,
                           wait: bool = False):
         return
 
     async def rotate(self,
                      angle: float,
                      angular_speed: float,
-                     ang_unit: ANG_UNIT = ANG_UNIT.DEG,
+                     ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                      callback_feedback: typing.Callable = None,
                      callback_feedback_async: typing.Callable = None,
                      callback_finish: typing.Callable = None,
                      callback_finish_async: typing.Callable = None,
                      enable_obstacles: bool = True,
                      wait: bool = False):
         return
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/navigation_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/navigation_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typing
 from rclpy.node import Node
-from raya.enumerations import POS_UNIT, ANG_UNIT
+from raya.enumerations import POSITION_UNIT, ANGLE_UNIT
 from raya.controllers.base_controller import BaseController
 
 
 class NavigationController(BaseController):
 
     def __init__(self, name: str, node: Node, interface, extra_info={}):
         pass
@@ -49,25 +49,25 @@
     async def save_location(self,
                             location_name: str,
                             x: float,
                             y: float,
                             angle: float,
                             map_name: str = '',
                             current_pose: bool = False,
-                            pos_unit: POS_UNIT = POS_UNIT.PIXEL,
-                            ang_unit: ANG_UNIT = ANG_UNIT.DEG):
+                            pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS,
+                            ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         pass
 
     async def delete_location(self, location_name: str, map_name: str = ''):
         pass
 
     async def get_location(self,
                            location_name: str,
                            map_name: str = '',
-                           pos_unit: POS_UNIT = POS_UNIT.PIXEL):
+                           pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS):
         return
 
     async def get_locations_list(self, map_name: str = ''):
         return
 
     async def get_locations(self, map_name: str = ''):
         return
@@ -76,34 +76,35 @@
         return
 
     async def get_zones_list(self, map_name: str = ''):
         return
 
     async def get_zone_center(self,
                               zone_name: str,
-                              pos_unit: POS_UNIT = POS_UNIT.PIXEL):
+                              pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS):
         return
 
     async def is_in_zone(self, zone_name: str = ''):
         return
 
     async def delete_zone(self, location_name: str, map_name: str = ''):
         pass
 
     async def get_position(self,
-                           pos_unit: POS_UNIT = POS_UNIT.PIXEL,
-                           ang_unit: ANG_UNIT = ANG_UNIT.DEG):
+                           pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS,
+                           ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES):
         return
 
     async def order_zone_points(self,
                                 zone_name: str,
                                 from_current_pose: bool = False):
         return
 
-    async def get_sorted_zone_point(self, pos_unit: POS_UNIT = POS_UNIT.PIXEL):
+    async def get_sorted_zone_point(
+            self, pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS):
         return
 
     async def set_map(self,
                       map_name: str,
                       wait_localization: bool = False,
                       timeout: float = 0.0,
                       callback_feedback: typing.Callable = None,
@@ -124,16 +125,16 @@
         return
 
     async def navigate_to_position(
         self,
         x: float,
         y: float,
         angle: float,
-        pos_unit: POS_UNIT = POS_UNIT.PIXEL,
-        ang_unit: ANG_UNIT = ANG_UNIT.DEG,
+        pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS,
+        ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
         callback_feedback: typing.Callable = None,
         callback_feedback_async: typing.Callable = None,
         callback_finish: typing.Callable = None,
         callback_finish_async: typing.Callable = None,
         wait: bool = False,
         xy_tolerance: float = float('nan'),
         yaw_tolerance: float = float('nan')):
@@ -162,29 +163,29 @@
                                xy_tolerance: float = float('nan'),
                                yaw_tolerance: float = float('nan')):
         return
 
     async def go_to_angle(self,
                           angle_target: float,
                           angular_velocity: float,
-                          ang_unit: ANG_UNIT = ANG_UNIT.DEG,
+                          ang_unit: ANGLE_UNIT = ANGLE_UNIT.DEGREES,
                           callback_feedback: typing.Callable = None,
                           callback_feedback_async: typing.Callable = None,
                           callback_finish: typing.Callable = None,
                           callback_finish_async: typing.Callable = None,
                           wait=False):
         return
 
     async def navigate_close_to_position(
             self,
             x: float,
             y: float,
             min_radius: float = 0.0,
             max_radius: float = 0.8,
-            pos_unit: POS_UNIT = POS_UNIT.PIXEL,
+            pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS,
             callback_feedback: typing.Callable = None,
             callback_feedback_async: typing.Callable = None,
             callback_finish: typing.Callable = None,
             callback_finish_async: typing.Callable = None,
             wait=False):
         return
 
@@ -197,15 +198,15 @@
     def is_navigating(self):
         return
 
     async def save_zone(self,
                         zone_name: str,
                         points: list,
                         map_name: str,
-                        pos_unit: POS_UNIT = POS_UNIT.PIXEL,
+                        pos_unit: POSITION_UNIT = POSITION_UNIT.PIXELS,
                         callback_feedback: typing.Callable = None,
                         callback_feedback_async: typing.Callable = None,
                         callback_finish: typing.Callable = None,
                         callback_finish_async: typing.Callable = None,
                         wait=False):
         return
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/sensors_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/sensors_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,18 +23,24 @@
                               inside_range: bool = True,
                               abs_val: bool = False):
         pass
 
     def create_threshold_listener(self,
                                   *,
                                   listener_name: str,
-                                  callback,
                                   sensors_paths,
+                                  callback=None,
+                                  callback_async=None,
                                   lower_bound: float = float('-inf'),
                                   higher_bound: float = float('inf'),
                                   inside_range: bool = True,
                                   abs_val: bool = False):
         pass
 
-    def create_boolean_listener(self, *, listener_name: str, callback,
-                                sensors_paths, logic_state: bool):
+    def create_boolean_listener(self,
+                                *,
+                                listener_name: str,
+                                sensors_paths,
+                                callback=None,
+                                callback_async=None,
+                                logic_state: bool):
         pass
```

### Comparing `raya-3.5.2.dev0/src/raya/controllers/skills_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/skills_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/sound_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/sound_controller.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/controllers/ui_controller.py` & `raya-3.5.3.dev0/src/raya/controllers/ui_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,194 +7,198 @@
 
 
 class UIController(BasePseudoController):
 
     def __init__(self, name: str, interface):
         pass
 
-    async def display_split_screen(self,
-                                   title: str = None,
-                                   title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
-                                   first_component_type: SPLIT_TYPE = None,
-                                   first_component_data: dict = None,
-                                   second_component_type: SPLIT_TYPE = None,
-                                   second_component_data: dict = None,
-                                   show_back_button: bool = True,
-                                   back_button_text: str = 'Back',
-                                   button_size: int = 1,
-                                   languages: list = None,
-                                   chosen_language: str = None,
-                                   theme: THEME_TYPE = THEME_TYPE.DARK,
-                                   custom_style: dict = None,
-                                   wait: bool = False):
+    async def display_split_screen(
+            self,
+            title: str = None,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
+            first_component_type: UI_SPLIT_TYPE = None,
+            first_component_data: dict = None,
+            second_component_type: UI_SPLIT_TYPE = None,
+            second_component_data: dict = None,
+            show_back_button: bool = True,
+            back_button_text: str = 'Back',
+            button_size: int = 1,
+            languages: list = None,
+            chosen_language: str = None,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
+            custom_style: dict = None,
+            wait: bool = False):
         return
 
     async def display_modal(self,
                             title: str = None,
-                            title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+                            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
                             subtitle: str = None,
                             content: str = None,
-                            modal_type: MODAL_TYPE = MODAL_TYPE.INFO,
-                            modal_size: MODAL_SIZE = MODAL_SIZE.NORMAL,
+                            modal_type: UI_MODAL_TYPE = UI_MODAL_TYPE.INFO,
+                            modal_size: UI_MODAL_SIZE = UI_MODAL_SIZE.NORMAL,
                             submit_text: str = 'Yes',
                             cancel_text: str = 'No',
                             show_icon: bool = True,
                             button_size: int = 1,
-                            theme: THEME_TYPE = THEME_TYPE.DARK,
+                            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
                             custom_style: dict = None,
                             wait: bool = True,
                             callback: callable = None) -> Enum:
         pass
 
-    async def display_input_modal(self,
-                                  title: str = None,
-                                  title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
-                                  subtitle: str = None,
-                                  submit_text: str = 'OK',
-                                  cancel_text: str = 'Cancel',
-                                  placeholder: str = None,
-                                  input_type: INPUT_TYPE = INPUT_TYPE.TEXT,
-                                  show_back_button: bool = False,
-                                  back_button_text: str = 'Back',
-                                  button_size: int = 1,
-                                  languages: list = None,
-                                  chosen_language=None,
-                                  theme: THEME_TYPE = THEME_TYPE.DARK,
-                                  custom_style: dict = None,
-                                  wait: bool = True,
-                                  callback: callable = None) -> Enum:
+    async def display_input_modal(
+            self,
+            title: str = None,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
+            subtitle: str = None,
+            submit_text: str = 'OK',
+            cancel_text: str = 'Cancel',
+            placeholder: str = None,
+            input_type: UI_INPUT_TYPE = UI_INPUT_TYPE.TEXT,
+            show_back_button: bool = False,
+            back_button_text: str = 'Back',
+            button_size: int = 1,
+            languages: list = None,
+            chosen_language=None,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
+            custom_style: dict = None,
+            wait: bool = True,
+            callback: callable = None) -> Enum:
         pass
 
     async def display_screen(self,
                              title: str = None,
-                             title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+                             title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
                              subtitle: str = None,
                              show_loader: bool = True,
                              show_back_button: bool = True,
                              back_button_text: str = 'Back',
                              button_size: int = 1,
                              languages: list = None,
                              chosen_language=None,
-                             theme: THEME_TYPE = THEME_TYPE.DARK,
+                             theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
                              custom_style: dict = None) -> Enum:
         return
 
     async def display_interactive_map(
             self,
             title: str = None,
-            title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
             subtitle: str = None,
             map_name: str = None,
             show_robot_position: bool = True,
             view_only: bool = False,
             show_back_button: bool = True,
             back_button_text: str = 'Back',
             button_size: int = 1,
             languages: list = None,
             chosen_language=None,
-            theme: THEME_TYPE = THEME_TYPE.DARK,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
             custom_style: dict = None,
             wait: bool = True,
             callback: callable = None) -> Enum:
         pass
 
-    async def display_action_screen(self,
-                                    title: str = None,
-                                    title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
-                                    subtitle: str = None,
-                                    button_text: str = None,
-                                    show_back_button: bool = True,
-                                    back_button_text: str = 'Back',
-                                    button_size: str = None,
-                                    languages: list = None,
-                                    chosen_language=None,
-                                    theme: THEME_TYPE = THEME_TYPE.DARK,
-                                    custom_style: dict = None,
-                                    wait: bool = True,
-                                    callback: callable = None) -> Enum:
+    async def display_action_screen(
+            self,
+            title: str = None,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
+            subtitle: str = None,
+            button_text: str = None,
+            show_back_button: bool = True,
+            back_button_text: str = 'Back',
+            button_size: str = None,
+            languages: list = None,
+            chosen_language=None,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
+            custom_style: dict = None,
+            wait: bool = True,
+            callback: callable = None) -> Enum:
         pass
 
     async def display_choice_selector(
             self,
             data: List[Dict],
             max_items_shown: int = None,
             title: str = None,
-            title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
             scroll_arrow_buttom_text: str = None,
             scroll_arrow_upper_text: str = None,
             show_back_button: bool = True,
             back_button_text: str = 'Back',
             button_size: int = 1,
             languages: list = None,
             chosen_language=None,
-            theme: THEME_TYPE = THEME_TYPE.DARK,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
             custom_style: dict = None,
             wait: bool = True,
             callback: callable = None) -> Enum:
         pass
 
-    async def display_animation(self,
-                                title: str = None,
-                                title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
-                                subtitle: str = None,
-                                content=None,
-                                format: ANIMATION_TYPE = None,
-                                show_loader: bool = False,
-                                show_back_button: bool = True,
-                                back_button_text: str = 'Back',
-                                button_size: int = 1,
-                                languages: list = None,
-                                chosen_language: str = None,
-                                theme: THEME_TYPE = THEME_TYPE.DARK,
-                                custom_style: dict = None) -> Enum:
+    async def display_animation(
+            self,
+            title: str = None,
+            title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
+            subtitle: str = None,
+            content=None,
+            format: UI_ANIMATION_TYPE = None,
+            show_loader: bool = False,
+            show_back_button: bool = True,
+            back_button_text: str = 'Back',
+            button_size: int = 1,
+            languages: list = None,
+            chosen_language: str = None,
+            theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
+            custom_style: dict = None) -> Enum:
         return
 
     async def open_link(self,
                         url: str,
                         title: str = None,
-                        title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+                        title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
                         show_back_button: bool = True,
                         back_button_text: str = 'Back',
                         button_size: int = 1,
                         languages: list = None,
                         chosen_language=None,
-                        theme: THEME_TYPE = THEME_TYPE.DARK,
+                        theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
                         custom_style: dict = None,
                         wait: bool = True,
                         callback: callable = None) -> Enum:
         pass
 
     async def open_video(self,
                          url: str,
                          title: str = None,
-                         title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+                         title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
                          show_back_button: bool = True,
                          back_button_text: str = 'Back',
                          button_size: int = 1,
                          width: str = '85%',
                          height: str = '75%',
                          languages: list = None,
                          chosen_language=None,
-                         theme: THEME_TYPE = THEME_TYPE.DARK,
+                         theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
                          custom_style: dict = None,
                          wait: bool = True,
                          callback: callable = None) -> Enum:
         pass
 
     async def open_conference(self,
                               title: str = None,
-                              title_size: TITLE_SIZE = TITLE_SIZE.MEDIUM,
+                              title_size: UI_TITLE_SIZE = UI_TITLE_SIZE.MEDIUM,
                               subtitle: str = None,
                               client: str = None,
                               call_on_join: bool = False,
                               button_text: str = 'Make a Call',
                               loading_subtitle: str = 'Loading ...',
                               show_back_button: bool = True,
                               back_button_text: str = 'Back',
                               button_size: int = 1,
                               languages: list = None,
-                              theme: THEME_TYPE = THEME_TYPE.DARK,
+                              theme: UI_THEME_TYPE = UI_THEME_TYPE.DARK,
                               chosen_language=None,
                               custom_style: dict = None,
                               wait: bool = True,
                               callback: callable = None) -> Enum:
         pass
```

### Comparing `raya-3.5.2.dev0/src/raya/exceptions.py` & `raya-3.5.3.dev0/src/raya/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     pass
 
 
 class RayaCommandTimeout(RayaCommandException):
     pass
 
 
+class RayaCommandFrozen(RayaCommandException):
+    pass
+
+
 class RayaApplicationException(RayaException):
     pass
 
 
 class RayaApplicationAlreadyRegistered(RayaApplicationException):
     pass
 
@@ -508,14 +512,18 @@
     pass
 
 
 class RayaUnableToEnableCamera(RayaMotionException):
     pass
 
 
+class RayaNoWaitableCommand(RayaMotionException):
+    pass
+
+
 class RayaInteractionsException(RayaControllerException):
     pass
 
 
 class RayaInteractionsAlreadyRunning(RayaInteractionsException):
     pass
```

### Comparing `raya-3.5.2.dev0/src/raya/exceptions_handler.py` & `raya-3.5.3.dev0/src/raya/exceptions_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/classifiers/objects_classifier_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/detectors/detector_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/detectors/detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/detectors/objects_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/detectors/tags_detector_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/estimators/estimator_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/estimators/estimator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/faces_recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/recognizers/recognizer_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/objects_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/planes_segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py` & `raya-3.5.3.dev0/src/raya/handlers/cv/segmentators/segmentator_handler.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya/raya_interface.py` & `raya-3.5.3.dev0/src/raya/raya_interface.py`

 * *Files identical despite different names*

### Comparing `raya-3.5.2.dev0/src/raya.egg-info/PKG-INFO` & `raya-3.5.3.dev0/src/raya.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raya
-Version: 3.5.2.dev0
+Version: 3.5.3.dev0
 Summary: Unlimited Robotics - Ra-Ya Python Library
 Home-page: https://documentation.unlimited-robotics.com/
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: UNKNOWN
```

### Comparing `raya-3.5.2.dev0/src/raya.egg-info/SOURCES.txt` & `raya-3.5.3.dev0/src/raya.egg-info/SOURCES.txt`

 * *Files identical despite different names*

