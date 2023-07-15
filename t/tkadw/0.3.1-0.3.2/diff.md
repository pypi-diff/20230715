# Comparing `tmp/tkadw-0.3.1.tar.gz` & `tmp/tkadw-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.3.1.tar", max compression
+gzip compressed data, was "tkadw-0.3.2.tar", max compression
```

## Comparing `tkadw-0.3.1.tar` & `tkadw-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,80 @@
--rw-r--r--   0        0        0      421 2023-07-05 05:18:37.520861 tkadw-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2545 2023-07-05 03:30:06.306836 tkadw-0.3.1/README.md
--rw-r--r--   0        0        0      563 2023-07-05 02:48:08.195395 tkadw-0.3.1/tkadw/__init__.py
--rw-r--r--   0        0        0      688 2023-07-04 14:23:05.022510 tkadw-0.3.1/tkadw/__main__.py
--rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.1/tkadw/utility/__init__.py
--rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.1/tkadw/utility/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.1/tkadw/utility/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.1/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
--rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.1/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.1/tkadw/utility/app.config
--rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.1/tkadw/utility/appconfig.py
--rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.1/tkadw/windows/__init__.py
--rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.1/tkadw/windows/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.1/tkadw/windows/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.1/tkadw/windows/__pycache__/theme.cpython-310.pyc
--rw-r--r--   0        0        0    11424 2023-07-05 02:48:08.391935 tkadw-0.3.1/tkadw/windows/__pycache__/theme.cpython-311.pyc
--rw-r--r--   0        0        0      974 2023-07-05 01:35:29.305457 tkadw-0.3.1/tkadw/windows/canvas/__init__.py
--rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1655 2023-07-05 01:35:29.383630 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0    22814 2023-07-05 01:35:37.012855 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
--rw-r--r--   0        0        0    44914 2023-07-05 01:35:29.406154 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0    11531 2023-07-05 01:36:48.740493 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
--rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
--rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
--rw-r--r--   0        0        0    24973 2023-07-05 01:35:47.767087 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
--rw-r--r--   0        0        0     1416 2023-07-05 01:35:40.147781 tkadw-0.3.1/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
--rw-r--r--   0        0        0    17936 2023-07-05 01:35:36.885314 tkadw-0.3.1/tkadw/windows/canvas/button.py
--rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.1/tkadw/windows/canvas/checkbox.py
--rw-r--r--   0        0        0    39862 2023-07-04 09:19:04.412974 tkadw-0.3.1/tkadw/windows/canvas/drawengine.py
--rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.1/tkadw/windows/canvas/entry.py
--rw-r--r--   0        0        0     6460 2023-07-05 01:36:48.456711 tkadw-0.3.1/tkadw/windows/canvas/frame.py
--rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.1/tkadw/windows/canvas/separator.py
--rw-r--r--   0        0        0    17760 2023-07-05 01:35:47.588176 tkadw-0.3.1/tkadw/windows/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.3.1/tkadw/windows/canvas/titlebar.py
--rw-r--r--   0        0        0      406 2023-07-05 01:35:39.966879 tkadw-0.3.1/tkadw/windows/canvas/widget.py
--rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.1/tkadw/windows/fluent/__init__.py
--rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
--rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
--rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
--rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.1/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.1/tkadw/windows/fluent/button.py
--rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.1/tkadw/windows/fluent/entry.py
--rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.1/tkadw/windows/fluent/frame.py
--rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.1/tkadw/windows/fluent/GeneralSans-Regular.ttf
--rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.1/tkadw/windows/fluent/test.py
--rw-r--r--   0        0        0    15923 2023-07-05 03:12:28.673805 tkadw-0.3.1/tkadw/windows/theme.py
--rw-r--r--   0        0        0      105 2023-07-05 02:48:08.250687 tkadw-0.3.1/tkadw/windows/widgets/__init__.py
--rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      323 2023-07-05 02:48:08.362447 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
--rw-r--r--   0        0        0    21509 2023-07-05 02:08:39.052688 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
--rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
--rw-r--r--   0        0        0     4377 2023-07-05 01:35:47.771212 tkadw-0.3.1/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
--rw-r--r--   0        0        0    19150 2023-07-04 14:22:25.521559 tkadw-0.3.1/tkadw/windows/widgets/adw.py
--rw-r--r--   0        0        0     1992 2023-07-04 10:38:07.052633 tkadw-0.3.1/tkadw/windows/widgets/label.py
--rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.1/tkadw/windows/widgets/listbox.py
--rw-r--r--   0        0        0     1115 2023-07-04 15:01:03.382573 tkadw-0.3.1/tkadw/windows/widgets/mdi.py
--rw-r--r--   0        0        0     3142 1970-01-01 00:00:00.000000 tkadw-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      421 2023-07-15 05:12:31.168424 tkadw-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2623 2023-07-15 05:13:40.274575 tkadw-0.3.2/README.md
+-rw-r--r--   0        0        0      591 2023-07-14 05:18:03.595214 tkadw-0.3.2/tkadw/__init__.py
+-rw-r--r--   0        0        0      729 2023-07-15 04:57:05.864349 tkadw-0.3.2/tkadw/__main__.py
+-rw-r--r--   0        0        0       82 2023-07-09 09:06:40.819424 tkadw-0.3.2/tkadw/game/__init__.py
+-rw-r--r--   0        0        0      274 2023-07-09 10:06:51.337745 tkadw-0.3.2/tkadw/game/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1081 2023-07-09 09:05:04.428075 tkadw-0.3.2/tkadw/game/__pycache__/surface.cpython-311.pyc
+-rw-r--r--   0        0        0     1486 2023-07-09 10:06:51.339744 tkadw-0.3.2/tkadw/game/__pycache__/window.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-07-09 09:06:15.869430 tkadw-0.3.2/tkadw/game/action.py
+-rw-r--r--   0        0        0      302 2023-07-09 09:05:03.855776 tkadw-0.3.2/tkadw/game/surface.py
+-rw-r--r--   0        0        0      503 2023-07-09 09:03:53.662343 tkadw-0.3.2/tkadw/game/window.py
+-rw-r--r--   0        0        0        0 2023-07-05 02:47:22.168814 tkadw-0.3.2/tkadw/utility/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-05 03:10:22.091006 tkadw-0.3.2/tkadw/utility/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      143 2023-07-05 02:48:08.371100 tkadw-0.3.2/tkadw/utility/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      851 2023-07-05 03:10:22.094005 tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-310.pyc
+-rw-r--r--   0        0        0     1779 2023-07-05 02:48:08.372100 tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-311.pyc
+-rw-r--r--   0        0        0    10003 2023-07-15 00:06:35.798144 tkadw-0.3.2/tkadw/utility/__pycache__/dragtool.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.3.2/tkadw/utility/app.config
+-rw-r--r--   0        0        0      944 2023-07-05 02:48:08.189796 tkadw-0.3.2/tkadw/utility/appconfig.py
+-rw-r--r--   0        0        0     5435 2023-07-15 00:06:32.738325 tkadw-0.3.2/tkadw/utility/dragtool.py
+-rw-r--r--   0        0        0      107 2023-07-05 01:34:36.098785 tkadw-0.3.2/tkadw/windows/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-05 03:10:20.021585 tkadw-0.3.2/tkadw/windows/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      273 2023-07-05 01:35:29.380630 tkadw-0.3.2/tkadw/windows/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6883 2023-07-05 03:12:28.822756 tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-310.pyc
+-rw-r--r--   0        0        0    14199 2023-07-09 15:40:13.496015 tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-311.pyc
+-rw-r--r--   0        0        0     1138 2023-07-14 23:55:33.173781 tkadw-0.3.2/tkadw/windows/canvas/__init__.py
+-rw-r--r--   0        0        0     1263 2023-07-05 03:10:20.085734 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1945 2023-07-14 23:57:15.913264 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12827 2023-07-05 03:10:21.840626 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0    23268 2023-07-14 05:54:14.950226 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0    38279 2023-07-05 03:10:20.174751 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc
+-rw-r--r--   0        0        0    44914 2023-07-05 01:35:29.406154 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    11053 2023-07-05 03:10:21.911520 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0    21085 2023-07-05 01:35:43.431699 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     6171 2023-07-05 03:10:22.086485 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0    11531 2023-07-05 01:36:48.740493 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2694 2023-07-05 03:12:28.867163 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc
+-rw-r--r--   0        0        0     4558 2023-07-05 01:36:52.241618 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc
+-rw-r--r--   0        0        0    13219 2023-07-05 03:10:21.930952 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc
+-rw-r--r--   0        0        0    25106 2023-07-09 15:08:09.223638 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0      943 2023-07-05 03:10:21.883207 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1538 2023-07-14 05:57:28.861208 tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc
+-rw-r--r--   0        0        0    18129 2023-07-14 05:53:34.112161 tkadw-0.3.2/tkadw/windows/canvas/button.py
+-rw-r--r--   0        0        0     6156 2023-07-05 01:39:19.281978 tkadw-0.3.2/tkadw/windows/canvas/checkbox.py
+-rw-r--r--   0        0        0    39862 2023-07-04 09:19:04.412974 tkadw-0.3.2/tkadw/windows/canvas/drawengine.py
+-rw-r--r--   0        0        0    15971 2023-07-05 01:35:43.285417 tkadw-0.3.2/tkadw/windows/canvas/entry.py
+-rw-r--r--   0        0        0     6460 2023-07-05 01:36:48.456711 tkadw-0.3.2/tkadw/windows/canvas/frame.py
+-rw-r--r--   0        0        0     2442 2023-07-05 01:36:52.052770 tkadw-0.3.2/tkadw/windows/canvas/separator.py
+-rw-r--r--   0        0        0    17817 2023-07-09 15:08:09.086448 tkadw-0.3.2/tkadw/windows/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.3.2/tkadw/windows/canvas/titlebar.py
+-rw-r--r--   0        0        0      520 2023-07-14 05:57:26.216938 tkadw-0.3.2/tkadw/windows/canvas/widget.py
+-rw-r--r--   0        0        0      223 2023-07-05 01:38:08.509601 tkadw-0.3.2/tkadw/windows/fluent/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-05 03:10:21.986646 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      481 2023-07-05 01:38:08.644612 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2899 2023-07-05 03:10:22.025283 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc
+-rw-r--r--   0        0        0     5148 2023-07-05 01:38:39.662205 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     2955 2023-07-05 03:10:22.017187 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc
+-rw-r--r--   0        0        0     5190 2023-07-05 01:36:27.311777 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     1315 2023-07-05 03:10:22.047317 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc
+-rw-r--r--   0        0        0     1968 2023-07-05 01:38:48.418651 tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     4604 2023-07-05 01:38:39.519641 tkadw-0.3.2/tkadw/windows/fluent/button.py
+-rw-r--r--   0        0        0     4545 2023-07-05 01:36:27.195727 tkadw-0.3.2/tkadw/windows/fluent/entry.py
+-rw-r--r--   0        0        0      952 2023-07-05 01:38:48.118337 tkadw-0.3.2/tkadw/windows/fluent/frame.py
+-rw-r--r--   0        0        0    66280 2022-07-26 17:24:46.000000 tkadw-0.3.2/tkadw/windows/fluent/GeneralSans-Regular.ttf
+-rw-r--r--   0        0        0      639 2023-07-05 01:37:20.730737 tkadw-0.3.2/tkadw/windows/fluent/test.py
+-rw-r--r--   0        0        0    20620 2023-07-09 15:40:13.355715 tkadw-0.3.2/tkadw/windows/theme.py
+-rw-r--r--   0        0        0      151 2023-07-15 04:00:51.951970 tkadw-0.3.2/tkadw/windows/widgets/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-05 03:10:21.933019 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      395 2023-07-15 04:02:14.716290 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19005 2023-07-05 03:10:21.948576 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc
+-rw-r--r--   0        0        0    21509 2023-07-05 02:08:39.052688 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc
+-rw-r--r--   0        0        0     2545 2023-07-05 03:10:21.971123 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc
+-rw-r--r--   0        0        0     4377 2023-07-05 01:35:47.771212 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc
+-rw-r--r--   0        0        0     3435 2023-07-15 04:48:08.638319 tkadw-0.3.2/tkadw/windows/widgets/__pycache__/mdi.cpython-311.pyc
+-rw-r--r--   0        0        0    19150 2023-07-04 14:22:25.521559 tkadw-0.3.2/tkadw/windows/widgets/adw.py
+-rw-r--r--   0        0        0     1992 2023-07-04 10:38:07.052633 tkadw-0.3.2/tkadw/windows/widgets/label.py
+-rw-r--r--   0        0        0        0 2023-07-04 10:38:58.527667 tkadw-0.3.2/tkadw/windows/widgets/listbox.py
+-rw-r--r--   0        0        0     1469 2023-07-15 04:48:08.519396 tkadw-0.3.2/tkadw/windows/widgets/mdi.py
+-rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 tkadw-0.3.2/PKG-INFO
```

### Comparing `tkadw-0.3.1/README.md` & `tkadw-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,8 +66,13 @@
 > `0.3.0`
 >> `301`新增`AdwSeparator`分割线组件 新增`AdwWidget`简化组件绘制流程
 > 
 >> `302`分支`widgets`库，将加入仅使用组件组合起来的控件，而非用canvas绘出来的组件
 > 
 >> `303`调改`AdwDrawEntry`和`AdwDrawText`的焦点事件绑定
 > 
->> `304`新增主题类组件，只需使用`set_default_theme`设置主题。对于经过特殊设计和特殊样式的组件，比如`Fluent`主题组件、`Win11`主题控件`AccentButton`，将不加入主题变量内
+>> `304`新增主题类组件，只需使用`set_default_theme`设置主题。对于经过特殊设计和特殊样式的组件，比如`Fluent`主题组件、`Win11`主题控件`AccentButton`，将不加入主题变量内
+
+> `0.3.2`
+>> `321` 新增`AdwMDI`组件
+> 
+>> `322` 添加`metro`主题
```

### Comparing `tkadw-0.3.1/tkadw/__main__.py` & `tkadw-0.3.2/tkadw/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from tkadw import *
 
 root = Adwite(wincaption=(53, 53, 53))
+root.set_default_theme("metro", "dark")
 
 frame = AdwTFrame(root)
 
 label1 = AdwTLabel(frame.frame, text="GTkLabel")
 label1.pack(fill="x", ipadx=5, padx=5, pady=5)
 
 button1 = AdwTButton(frame.frame, text="GTkButton")
```

### Comparing `tkadw-0.3.1/tkadw/utility/__pycache__/appconfig.cpython-310.pyc` & `tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/utility/__pycache__/appconfig.cpython-311.pyc` & `tkadw-0.3.2/tkadw/utility/__pycache__/appconfig.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/utility/appconfig.py` & `tkadw-0.3.2/tkadw/utility/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/__pycache__/theme.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/__pycache__/theme.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/__pycache__/theme.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xa6d0a464 (Wed Jul  5 02:08:38 2023 UTC)
-files sz: 15479
+moddate:  0xddd4aa64 (Sun Jul  9 15:40:13 2023 UTC)
+files sz: 20620
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 20
    flags     : 0
    code
       0x97006400640169016402640364049c0264056406640764086409640a64
@@ -33,42 +33,52 @@
       316417644a641564096437643164199c06641a9c09644364146417644464
       156409643564316417644a641564096437643164199c06641a9c09644964
       09641c641d9c03641e9c075a046400644b69016402641764049c02644364
       4c644d644e6409644d644d644e6409640c9c04644f644d64506409640c9c
       04640f9c07644764516452641264139c0464436414644b644d6426640964
       356431644b6453642664096453643164199c06641a9c0964436414644b64
       4d6426640964356431644b6453642664096453643164199c06641a9c0964
-      526409641c641d9c03641e9c075a05645484005a06645584005a07647464
-      5784015a08020065086458a6010000ab0100000000000000000100643164
-      596c096d0a5a0a010002004700645a8400645b650aa6030000ab03000000
-      00000000005a0b6431645c6c0c6d0d5a0d010002004700645d8400645e65
-      0da6030000ab0300000000000000005a0e6431645f6c0f6d105a10010002
-      0047006460840064616510a6030000ab0300000000000000005a11643164
-      626c126d135a130100020047006463840064646513a6030000ab03000000
-      00000000005a14643164656c156d165a1601000200470064668400646765
-      16a6030000ab0300000000000000005a17643164686c186d195a19010002
-      00470064698400646a6519a6030000ab0300000000000000005a1a643164
-      6b6c1b6d1c5a1c010002004700646c8400646d651ca6030000ab03000000
-      00000000005a1d651e646e6b020000000072e56431646f6c1f6d205a2001
-      000200650ba6000000ab0000000000000000005a216521a0080000000000
-      0000000000000000000000000000006458a6010000ab0100000000000000
-      00010002006511a6000000ab0000000000000000005a226522a023000000
-      0000000000000000000000000000000000647064716471ac72a6030000ab
-      03000000000000000001000200651da6000000ab0000000000000000005a
-      246524a02300000000000000000000000000000000000000006470647164
-      71ac72a6030000ab030000000000000000010002006514a6000000ab0000
-      000000000000005a256525a0230000000000000000000000000000000000
-      000000647064716471ac72a6030000ab0300000000000000000100020065
-      17a6000000ab0000000000000000005a266526a023000000000000000000
-      0000000000000000000000647064716471ac72a6030000ab030000000000
-      00000001000200651aa6000000ab0000000000000000005a276527a02300
-      00000000000000000000000000000000000000647064716471ac72a60300
-      00ab03000000000000000001006521a02800000000000000000000000000
-      00000000000000a6000000ab000000000000000000010064735300647353
-      00
+      526409641c641d9c03641e9c075a056400641769016402640364049c0264
+      3164546442640364096455645564176409640c9c04645664566417640964
+      0c9c04640f9c07643164176457641264139c046431645864176459640364
+      09641764316417645a640364096417643164199c06641a9c096431645864
+      17645964036409641764316417645a640364096417643164199c06641a9c
+      0964596409641c641d9c03641e9c075a066400645b69016402640364049c
+      026431645c645d64176409645e645e64036409640c9c0464546454640364
+      09640c9c04640f9c076431645b643d641264139c0464316458645b645964
+      17640964036431645b645a641764096403643164199c06641a9c09643164
+      58645b64596417640964036431645b645a641764096403643164199c0664
+      1a9c0964596409645f641d9c03641e9c075a07646084005a08646184005a
+      096484646384015a0a0200650a6464a6010000ab01000000000000000001
+      00643164656c0b6d0c5a0c010002004700646684006467650ca6030000ab
+      0300000000000000005a0d643164686c0e6d0f5a0f010002004700646984
+      00646a650fa6030000ab0300000000000000005a106431646b6c116d125a
+      12010002004700646c8400646d6512a6030000ab0300000000000000005a
+      136431646e6c146d155a15010002004700646f840064706515a6030000ab
+      0300000000000000005a16643164716c176d185a18010002004700647284
+      0064736518a6030000ab0300000000000000005a19643164746c1a6d1b5a
+      1b010002004700647584006476651ba6030000ab0300000000000000005a
+      1c643164776c1d6d1e5a1e010002004700647884006479651ea6030000ab
+      0300000000000000005a1f6520647a6b020000000072ef6431647b6c216d
+      225a2201000200650da6000000ab0000000000000000005a236523a00a00
+      00000000000000000000000000000000000000647ca6010000ab01000000
+      00000000000100647d84005a2402006513646d6524ac7ea6020000ab0200
+      000000000000005a256525a0260000000000000000000000000000000000
+      000000647f64806480ac81a6030000ab0300000000000000000100020065
+      1fa6000000ab0000000000000000005a276527a026000000000000000000
+      0000000000000000000000647f64806480ac81a6030000ab030000000000
+      0000000100020065166470ac82a6010000ab0100000000000000005a2865
+      28a0260000000000000000000000000000000000000000647f64806480ac
+      81a6030000ab0300000000000000000100020065196473ac82a6010000ab
+      0100000000000000005a296529a026000000000000000000000000000000
+      0000000000647f64806480ac81a6030000ab030000000000000000010002
+      00651ca6000000ab0000000000000000005a2a652aa02600000000000000
+      00000000000000000000000000647f64806480ac81a6030000ab03000000
+      000000000001006523a02b00000000000000000000000000000000000000
+      00a6000000ab00000000000000000001006483530064835300
      0           0 RESUME                   0
    
      3           2 LOAD_CONST               0 ('back')
                  4 LOAD_CONST               1 ('#f4f4f4')
    
      2           6 BUILD_MAP                1
    
@@ -897,268 +907,557 @@
    551         904 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
                906 BUILD_CONST_KEY_MAP      3
    
    466         908 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
                910 BUILD_CONST_KEY_MAP      7
                912 STORE_NAME               5 (bilibili_dark_theme)
    
-   560         914 LOAD_CONST              84 (<code object get_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 560>)
-               916 MAKE_FUNCTION            0
-               918 STORE_NAME               6 (get_default_theme)
-   
-   569         920 LOAD_CONST              85 (<code object _set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 569>)
-               922 MAKE_FUNCTION            0
-               924 STORE_NAME               7 (_set_default_theme)
-   
-   575         926 LOAD_CONST             116 (('system',))
-               928 LOAD_CONST              87 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 575>)
-               930 MAKE_FUNCTION            1 (defaults)
-               932 STORE_NAME               8 (set_default_theme)
-   
-   613         934 PUSH_NULL
-               936 LOAD_NAME                8 (set_default_theme)
-               938 LOAD_CONST              88 ('win11')
-               940 PRECALL                  1
-               944 CALL                     1
-               954 POP_TOP
-   
-   616         956 LOAD_CONST              49 (0)
-               958 LOAD_CONST              89 (('Adw',))
-               960 IMPORT_NAME              9 (tkadw.windows.widgets.adw)
-               962 IMPORT_FROM             10 (Adw)
-               964 STORE_NAME              10 (Adw)
-               966 POP_TOP
-   
-   619         968 PUSH_NULL
-               970 LOAD_BUILD_CLASS
-               972 LOAD_CONST              90 (<code object Adwite, file "D:\tkadw\tkadw\windows\theme.py", line 619>)
-               974 MAKE_FUNCTION            0
-               976 LOAD_CONST              91 ('Adwite')
-               978 LOAD_NAME               10 (Adw)
-               980 PRECALL                  3
-               984 CALL                     3
-               994 STORE_NAME              11 (Adwite)
-   
-   631         996 LOAD_CONST              49 (0)
-               998 LOAD_CONST              92 (('AdwLabel',))
-              1000 IMPORT_NAME             12 (tkadw.windows.widgets)
-              1002 IMPORT_FROM             13 (AdwLabel)
-              1004 STORE_NAME              13 (AdwLabel)
-              1006 POP_TOP
-   
-   634        1008 PUSH_NULL
-              1010 LOAD_BUILD_CLASS
-              1012 LOAD_CONST              93 (<code object AdwTLabel, file "D:\tkadw\tkadw\windows\theme.py", line 634>)
-              1014 MAKE_FUNCTION            0
-              1016 LOAD_CONST              94 ('AdwTLabel')
-              1018 LOAD_NAME               13 (AdwLabel)
-              1020 PRECALL                  3
-              1024 CALL                     3
-              1034 STORE_NAME              14 (AdwTLabel)
-   
-   639        1036 LOAD_CONST              49 (0)
-              1038 LOAD_CONST              95 (('AdwDrawRoundButton3',))
-              1040 IMPORT_NAME             15 (tkadw.windows.canvas.button)
-              1042 IMPORT_FROM             16 (AdwDrawRoundButton3)
-              1044 STORE_NAME              16 (AdwDrawRoundButton3)
-              1046 POP_TOP
-   
-   642        1048 PUSH_NULL
-              1050 LOAD_BUILD_CLASS
-              1052 LOAD_CONST              96 (<code object AdwTButton, file "D:\tkadw\tkadw\windows\theme.py", line 642>)
-              1054 MAKE_FUNCTION            0
-              1056 LOAD_CONST              97 ('AdwTButton')
-              1058 LOAD_NAME               16 (AdwDrawRoundButton3)
-              1060 PRECALL                  3
-              1064 CALL                     3
-              1074 STORE_NAME              17 (AdwTButton)
-   
-   647        1076 LOAD_CONST              49 (0)
-              1078 LOAD_CONST              98 (('AdwDrawRoundEntry3',))
-              1080 IMPORT_NAME             18 (tkadw.windows.canvas.entry)
-              1082 IMPORT_FROM             19 (AdwDrawRoundEntry3)
-              1084 STORE_NAME              19 (AdwDrawRoundEntry3)
-              1086 POP_TOP
-   
-   650        1088 PUSH_NULL
-              1090 LOAD_BUILD_CLASS
-              1092 LOAD_CONST              99 (<code object AdwTEntry, file "D:\tkadw\tkadw\windows\theme.py", line 650>)
-              1094 MAKE_FUNCTION            0
-              1096 LOAD_CONST             100 ('AdwTEntry')
-              1098 LOAD_NAME               19 (AdwDrawRoundEntry3)
-              1100 PRECALL                  3
-              1104 CALL                     3
-              1114 STORE_NAME              20 (AdwTEntry)
-   
-   655        1116 LOAD_CONST              49 (0)
-              1118 LOAD_CONST             101 (('AdwDrawRoundText3',))
-              1120 IMPORT_NAME             21 (tkadw.windows.canvas.textbox)
-              1122 IMPORT_FROM             22 (AdwDrawRoundText3)
-              1124 STORE_NAME              22 (AdwDrawRoundText3)
-              1126 POP_TOP
-   
-   658        1128 PUSH_NULL
-              1130 LOAD_BUILD_CLASS
-              1132 LOAD_CONST             102 (<code object AdwTText, file "D:\tkadw\tkadw\windows\theme.py", line 658>)
-              1134 MAKE_FUNCTION            0
-              1136 LOAD_CONST             103 ('AdwTText')
-              1138 LOAD_NAME               22 (AdwDrawRoundText3)
-              1140 PRECALL                  3
-              1144 CALL                     3
-              1154 STORE_NAME              23 (AdwTText)
-   
-   663        1156 LOAD_CONST              49 (0)
-              1158 LOAD_CONST             104 (('AdwDrawRoundFrame3',))
-              1160 IMPORT_NAME             24 (tkadw.windows.canvas.frame)
-              1162 IMPORT_FROM             25 (AdwDrawRoundFrame3)
-              1164 STORE_NAME              25 (AdwDrawRoundFrame3)
-              1166 POP_TOP
-   
-   666        1168 PUSH_NULL
-              1170 LOAD_BUILD_CLASS
-              1172 LOAD_CONST             105 (<code object AdwTFrame, file "D:\tkadw\tkadw\windows\theme.py", line 666>)
-              1174 MAKE_FUNCTION            0
-              1176 LOAD_CONST             106 ('AdwTFrame')
-              1178 LOAD_NAME               25 (AdwDrawRoundFrame3)
-              1180 PRECALL                  3
-              1184 CALL                     3
-              1194 STORE_NAME              26 (AdwTFrame)
-   
-   671        1196 LOAD_CONST              49 (0)
-              1198 LOAD_CONST             107 (('AdwDrawSeparator',))
-              1200 IMPORT_NAME             27 (tkadw.windows.canvas.separator)
-              1202 IMPORT_FROM             28 (AdwDrawSeparator)
-              1204 STORE_NAME              28 (AdwDrawSeparator)
-              1206 POP_TOP
-   
-   674        1208 PUSH_NULL
-              1210 LOAD_BUILD_CLASS
-              1212 LOAD_CONST             108 (<code object AdwTSeparator, file "D:\tkadw\tkadw\windows\theme.py", line 674>)
-              1214 MAKE_FUNCTION            0
-              1216 LOAD_CONST             109 ('AdwTSeparator')
-              1218 LOAD_NAME               28 (AdwDrawSeparator)
-              1220 PRECALL                  3
-              1224 CALL                     3
-              1234 STORE_NAME              29 (AdwTSeparator)
-   
-   679        1236 LOAD_NAME               30 (__name__)
-              1238 LOAD_CONST             110 ('__main__')
-              1240 COMPARE_OP               2 (==)
-              1246 POP_JUMP_FORWARD_IF_FALSE   229 (to 1706)
-   
-   680        1248 LOAD_CONST              49 (0)
-              1250 LOAD_CONST             111 (('isDark',))
-              1252 IMPORT_NAME             31 (darkdetect)
-              1254 IMPORT_FROM             32 (isDark)
-              1256 STORE_NAME              32 (isDark)
+   561         914 LOAD_CONST               0 ('back')
+               916 LOAD_CONST              23 ('#ffffff')
+   
+   560         918 BUILD_MAP                1
+   
+   565         920 LOAD_CONST               2 ('transparent')
+   
+   566         922 LOAD_CONST               3 ('#000000')
+   
+   564         924 LOAD_CONST               4 (('back', 'text_back'))
+               926 BUILD_CONST_KEY_MAP      2
+   
+   570         928 LOAD_CONST              49 (0)
+   
+   571         930 LOAD_CONST              84 ('#eeeeee')
+   
+   572         932 LOAD_CONST              66 ('#cccccc')
+   
+   573         934 LOAD_CONST               3 ('#000000')
+   
+   574         936 LOAD_CONST               9 (1)
+   
+   577         938 LOAD_CONST              85 ('#666666')
+   
+   578         940 LOAD_CONST              85 ('#666666')
+   
+   579         942 LOAD_CONST              23 ('#ffffff')
+   
+   580         944 LOAD_CONST               9 (1)
+   
+   576         946 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               948 BUILD_CONST_KEY_MAP      4
+   
+   584         950 LOAD_CONST              86 ('#333333')
+   
+   585         952 LOAD_CONST              86 ('#333333')
+   
+   586         954 LOAD_CONST              23 ('#ffffff')
+   
+   587         956 LOAD_CONST               9 (1)
+   
+   583         958 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+               960 BUILD_CONST_KEY_MAP      4
+   
+   569         962 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               964 BUILD_CONST_KEY_MAP      7
+   
+   592         966 LOAD_CONST              49 (0)
+   
+   593         968 LOAD_CONST              23 ('#ffffff')
+   
+   594         970 LOAD_CONST              87 ('#bfbfbf')
+   
+   595         972 LOAD_CONST              18 (2)
+   
+   591         974 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
+               976 BUILD_CONST_KEY_MAP      4
+   
+   599         978 LOAD_CONST              49 (0)
+   
+   600         980 LOAD_CONST              88 ((3, 3))
+   
+   602         982 LOAD_CONST              23 ('#ffffff')
+   
+   603         984 LOAD_CONST              89 ('#999999')
+   
+   604         986 LOAD_CONST               3 ('#000000')
+   
+   605         988 LOAD_CONST               9 (1)
+   
+   607         990 LOAD_CONST              23 ('#ffffff')
+   
+   608         992 LOAD_CONST              49 (0)
+   
+   611         994 LOAD_CONST              23 ('#ffffff')
+   
+   612         996 LOAD_CONST              90 ('#00aedb')
+   
+   613         998 LOAD_CONST               3 ('#000000')
+   
+   614        1000 LOAD_CONST               9 (1)
+   
+   616        1002 LOAD_CONST              23 ('#ffffff')
+   
+   617        1004 LOAD_CONST              49 (0)
+   
+   610        1006 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+              1008 BUILD_CONST_KEY_MAP      6
+   
+   598        1010 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+              1012 BUILD_CONST_KEY_MAP      9
+   
+   622        1014 LOAD_CONST              49 (0)
+   
+   623        1016 LOAD_CONST              88 ((3, 3))
+   
+   625        1018 LOAD_CONST              23 ('#ffffff')
+   
+   626        1020 LOAD_CONST              89 ('#999999')
+   
+   627        1022 LOAD_CONST               3 ('#000000')
+   
+   628        1024 LOAD_CONST               9 (1)
+   
+   630        1026 LOAD_CONST              23 ('#ffffff')
+   
+   631        1028 LOAD_CONST              49 (0)
+   
+   634        1030 LOAD_CONST              23 ('#ffffff')
+   
+   635        1032 LOAD_CONST              90 ('#00aedb')
+   
+   636        1034 LOAD_CONST               3 ('#000000')
+   
+   637        1036 LOAD_CONST               9 (1)
+   
+   639        1038 LOAD_CONST              23 ('#ffffff')
+   
+   640        1040 LOAD_CONST              49 (0)
+   
+   633        1042 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+              1044 BUILD_CONST_KEY_MAP      6
+   
+   621        1046 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+              1048 BUILD_CONST_KEY_MAP      9
+   
+   645        1050 LOAD_CONST              89 ('#999999')
+   
+   646        1052 LOAD_CONST               9 (1)
+   
+   648        1054 LOAD_CONST              28 (True)
+   
+   644        1056 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
+              1058 BUILD_CONST_KEY_MAP      3
+   
+   559        1060 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+              1062 BUILD_CONST_KEY_MAP      7
+              1064 STORE_NAME               6 (metro_theme)
+   
+   654        1066 LOAD_CONST               0 ('back')
+              1068 LOAD_CONST              91 ('#111111')
+   
+   653        1070 BUILD_MAP                1
+   
+   658        1072 LOAD_CONST               2 ('transparent')
+   
+   659        1074 LOAD_CONST               3 ('#000000')
+   
+   657        1076 LOAD_CONST               4 (('back', 'text_back'))
+              1078 BUILD_CONST_KEY_MAP      2
+   
+   663        1080 LOAD_CONST              49 (0)
+   
+   664        1082 LOAD_CONST              92 ('#222222')
+   
+   665        1084 LOAD_CONST              93 ('#444444')
+   
+   666        1086 LOAD_CONST              23 ('#ffffff')
+   
+   667        1088 LOAD_CONST               9 (1)
+   
+   670        1090 LOAD_CONST              94 ('#aaaaaa')
+   
+   671        1092 LOAD_CONST              94 ('#aaaaaa')
+   
+   672        1094 LOAD_CONST               3 ('#000000')
+   
+   673        1096 LOAD_CONST               9 (1)
+   
+   669        1098 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+              1100 BUILD_CONST_KEY_MAP      4
+   
+   677        1102 LOAD_CONST              84 ('#eeeeee')
+   
+   678        1104 LOAD_CONST              84 ('#eeeeee')
+   
+   679        1106 LOAD_CONST               3 ('#000000')
+   
+   680        1108 LOAD_CONST               9 (1)
+   
+   676        1110 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width'))
+              1112 BUILD_CONST_KEY_MAP      4
+   
+   662        1114 LOAD_CONST              15 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+              1116 BUILD_CONST_KEY_MAP      7
+   
+   685        1118 LOAD_CONST              49 (0)
+   
+   686        1120 LOAD_CONST              91 ('#111111')
+   
+   687        1122 LOAD_CONST              61 ('#373737')
+   
+   688        1124 LOAD_CONST              18 (2)
+   
+   684        1126 LOAD_CONST              19 (('radius', 'back', 'border', 'border_width'))
+              1128 BUILD_CONST_KEY_MAP      4
+   
+   692        1130 LOAD_CONST              49 (0)
+   
+   693        1132 LOAD_CONST              88 ((3, 3))
+   
+   695        1134 LOAD_CONST              91 ('#111111')
+   
+   696        1136 LOAD_CONST              89 ('#999999')
+   
+   697        1138 LOAD_CONST              23 ('#ffffff')
+   
+   698        1140 LOAD_CONST               9 (1)
+   
+   700        1142 LOAD_CONST               3 ('#000000')
+   
+   701        1144 LOAD_CONST              49 (0)
+   
+   704        1146 LOAD_CONST              91 ('#111111')
+   
+   705        1148 LOAD_CONST              90 ('#00aedb')
+   
+   706        1150 LOAD_CONST              23 ('#ffffff')
+   
+   707        1152 LOAD_CONST               9 (1)
+   
+   709        1154 LOAD_CONST               3 ('#000000')
+   
+   710        1156 LOAD_CONST              49 (0)
+   
+   703        1158 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+              1160 BUILD_CONST_KEY_MAP      6
+   
+   691        1162 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+              1164 BUILD_CONST_KEY_MAP      9
+   
+   715        1166 LOAD_CONST              49 (0)
+   
+   716        1168 LOAD_CONST              88 ((3, 3))
+   
+   718        1170 LOAD_CONST              91 ('#111111')
+   
+   719        1172 LOAD_CONST              89 ('#999999')
+   
+   720        1174 LOAD_CONST              23 ('#ffffff')
+   
+   721        1176 LOAD_CONST               9 (1)
+   
+   723        1178 LOAD_CONST               3 ('#000000')
+   
+   724        1180 LOAD_CONST              49 (0)
+   
+   727        1182 LOAD_CONST              91 ('#111111')
+   
+   728        1184 LOAD_CONST              90 ('#00aedb')
+   
+   729        1186 LOAD_CONST              23 ('#ffffff')
+   
+   730        1188 LOAD_CONST               9 (1)
+   
+   732        1190 LOAD_CONST               3 ('#000000')
+   
+   733        1192 LOAD_CONST              49 (0)
+   
+   726        1194 LOAD_CONST              25 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+              1196 BUILD_CONST_KEY_MAP      6
+   
+   714        1198 LOAD_CONST              26 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+              1200 BUILD_CONST_KEY_MAP      9
+   
+   738        1202 LOAD_CONST              89 ('#999999')
+   
+   739        1204 LOAD_CONST               9 (1)
+   
+   741        1206 LOAD_CONST              95 (False)
+   
+   737        1208 LOAD_CONST              29 (('back', 'border_width', 'rounded'))
+              1210 BUILD_CONST_KEY_MAP      3
+   
+   652        1212 LOAD_CONST              30 (('window', 'label', 'button', 'frame', 'entry', 'text', 'separator'))
+              1214 BUILD_CONST_KEY_MAP      7
+              1216 STORE_NAME               7 (metro_dark_theme)
+   
+   746        1218 LOAD_CONST              96 (<code object get_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 746>)
+              1220 MAKE_FUNCTION            0
+              1222 STORE_NAME               8 (get_default_theme)
+   
+   755        1224 LOAD_CONST              97 (<code object _set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 755>)
+              1226 MAKE_FUNCTION            0
+              1228 STORE_NAME               9 (_set_default_theme)
+   
+   761        1230 LOAD_CONST             132 (('system',))
+              1232 LOAD_CONST              99 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 761>)
+              1234 MAKE_FUNCTION            1 (defaults)
+              1236 STORE_NAME              10 (set_default_theme)
+   
+   827        1238 PUSH_NULL
+              1240 LOAD_NAME               10 (set_default_theme)
+              1242 LOAD_CONST             100 ('win11')
+              1244 PRECALL                  1
+              1248 CALL                     1
               1258 POP_TOP
    
-   682        1260 PUSH_NULL
-              1262 LOAD_NAME               11 (Adwite)
-              1264 PRECALL                  0
-              1268 CALL                     0
-              1278 STORE_NAME              33 (root)
-   
-   683        1280 LOAD_NAME               33 (root)
-              1282 LOAD_METHOD              8 (set_default_theme)
-              1304 LOAD_CONST              88 ('win11')
-              1306 PRECALL                  1
-              1310 CALL                     1
-              1320 POP_TOP
-   
-   684        1322 PUSH_NULL
-              1324 LOAD_NAME               17 (AdwTButton)
-              1326 PRECALL                  0
-              1330 CALL                     0
-              1340 STORE_NAME              34 (button)
-   
-   685        1342 LOAD_NAME               34 (button)
-              1344 LOAD_METHOD             35 (pack)
-              1366 LOAD_CONST             112 ('x')
-              1368 LOAD_CONST             113 (5)
-              1370 LOAD_CONST             113 (5)
-              1372 KW_NAMES               114
-              1374 PRECALL                  3
-              1378 CALL                     3
-              1388 POP_TOP
-   
-   686        1390 PUSH_NULL
-              1392 LOAD_NAME               29 (AdwTSeparator)
-              1394 PRECALL                  0
-              1398 CALL                     0
-              1408 STORE_NAME              36 (separator)
-   
-   687        1410 LOAD_NAME               36 (separator)
-              1412 LOAD_METHOD             35 (pack)
-              1434 LOAD_CONST             112 ('x')
-              1436 LOAD_CONST             113 (5)
-              1438 LOAD_CONST             113 (5)
-              1440 KW_NAMES               114
-              1442 PRECALL                  3
-              1446 CALL                     3
-              1456 POP_TOP
-   
-   688        1458 PUSH_NULL
-              1460 LOAD_NAME               20 (AdwTEntry)
-              1462 PRECALL                  0
-              1466 CALL                     0
-              1476 STORE_NAME              37 (entry)
-   
-   689        1478 LOAD_NAME               37 (entry)
-              1480 LOAD_METHOD             35 (pack)
-              1502 LOAD_CONST             112 ('x')
-              1504 LOAD_CONST             113 (5)
-              1506 LOAD_CONST             113 (5)
-              1508 KW_NAMES               114
-              1510 PRECALL                  3
-              1514 CALL                     3
-              1524 POP_TOP
-   
-   690        1526 PUSH_NULL
-              1528 LOAD_NAME               23 (AdwTText)
-              1530 PRECALL                  0
-              1534 CALL                     0
-              1544 STORE_NAME              38 (text)
-   
-   691        1546 LOAD_NAME               38 (text)
-              1548 LOAD_METHOD             35 (pack)
-              1570 LOAD_CONST             112 ('x')
-              1572 LOAD_CONST             113 (5)
-              1574 LOAD_CONST             113 (5)
-              1576 KW_NAMES               114
-              1578 PRECALL                  3
-              1582 CALL                     3
-              1592 POP_TOP
-   
-   692        1594 PUSH_NULL
-              1596 LOAD_NAME               26 (AdwTFrame)
-              1598 PRECALL                  0
-              1602 CALL                     0
-              1612 STORE_NAME              39 (frame)
-   
-   693        1614 LOAD_NAME               39 (frame)
-              1616 LOAD_METHOD             35 (pack)
-              1638 LOAD_CONST             112 ('x')
-              1640 LOAD_CONST             113 (5)
-              1642 LOAD_CONST             113 (5)
-              1644 KW_NAMES               114
-              1646 PRECALL                  3
-              1650 CALL                     3
-              1660 POP_TOP
-   
-   694        1662 LOAD_NAME               33 (root)
-              1664 LOAD_METHOD             40 (mainloop)
-              1686 PRECALL                  0
-              1690 CALL                     0
-              1700 POP_TOP
-              1702 LOAD_CONST             115 (None)
-              1704 RETURN_VALUE
+   830        1260 LOAD_CONST              49 (0)
+              1262 LOAD_CONST             101 (('Adw',))
+              1264 IMPORT_NAME             11 (tkadw.windows.widgets.adw)
+              1266 IMPORT_FROM             12 (Adw)
+              1268 STORE_NAME              12 (Adw)
+              1270 POP_TOP
+   
+   833        1272 PUSH_NULL
+              1274 LOAD_BUILD_CLASS
+              1276 LOAD_CONST             102 (<code object Adwite, file "D:\tkadw\tkadw\windows\theme.py", line 833>)
+              1278 MAKE_FUNCTION            0
+              1280 LOAD_CONST             103 ('Adwite')
+              1282 LOAD_NAME               12 (Adw)
+              1284 PRECALL                  3
+              1288 CALL                     3
+              1298 STORE_NAME              13 (Adwite)
+   
+   847        1300 LOAD_CONST              49 (0)
+              1302 LOAD_CONST             104 (('AdwLabel',))
+              1304 IMPORT_NAME             14 (tkadw.windows.widgets)
+              1306 IMPORT_FROM             15 (AdwLabel)
+              1308 STORE_NAME              15 (AdwLabel)
+              1310 POP_TOP
+   
+   850        1312 PUSH_NULL
+              1314 LOAD_BUILD_CLASS
+              1316 LOAD_CONST             105 (<code object AdwTLabel, file "D:\tkadw\tkadw\windows\theme.py", line 850>)
+              1318 MAKE_FUNCTION            0
+              1320 LOAD_CONST             106 ('AdwTLabel')
+              1322 LOAD_NAME               15 (AdwLabel)
+              1324 PRECALL                  3
+              1328 CALL                     3
+              1338 STORE_NAME              16 (AdwTLabel)
+   
+   855        1340 LOAD_CONST              49 (0)
+              1342 LOAD_CONST             107 (('AdwDrawRoundButton3',))
+              1344 IMPORT_NAME             17 (tkadw.windows.canvas.button)
+              1346 IMPORT_FROM             18 (AdwDrawRoundButton3)
+              1348 STORE_NAME              18 (AdwDrawRoundButton3)
+              1350 POP_TOP
+   
+   858        1352 PUSH_NULL
+              1354 LOAD_BUILD_CLASS
+              1356 LOAD_CONST             108 (<code object AdwTButton, file "D:\tkadw\tkadw\windows\theme.py", line 858>)
+              1358 MAKE_FUNCTION            0
+              1360 LOAD_CONST             109 ('AdwTButton')
+              1362 LOAD_NAME               18 (AdwDrawRoundButton3)
+              1364 PRECALL                  3
+              1368 CALL                     3
+              1378 STORE_NAME              19 (AdwTButton)
+   
+   863        1380 LOAD_CONST              49 (0)
+              1382 LOAD_CONST             110 (('AdwDrawRoundEntry3',))
+              1384 IMPORT_NAME             20 (tkadw.windows.canvas.entry)
+              1386 IMPORT_FROM             21 (AdwDrawRoundEntry3)
+              1388 STORE_NAME              21 (AdwDrawRoundEntry3)
+              1390 POP_TOP
+   
+   866        1392 PUSH_NULL
+              1394 LOAD_BUILD_CLASS
+              1396 LOAD_CONST             111 (<code object AdwTEntry, file "D:\tkadw\tkadw\windows\theme.py", line 866>)
+              1398 MAKE_FUNCTION            0
+              1400 LOAD_CONST             112 ('AdwTEntry')
+              1402 LOAD_NAME               21 (AdwDrawRoundEntry3)
+              1404 PRECALL                  3
+              1408 CALL                     3
+              1418 STORE_NAME              22 (AdwTEntry)
+   
+   871        1420 LOAD_CONST              49 (0)
+              1422 LOAD_CONST             113 (('AdwDrawRoundText3',))
+              1424 IMPORT_NAME             23 (tkadw.windows.canvas.textbox)
+              1426 IMPORT_FROM             24 (AdwDrawRoundText3)
+              1428 STORE_NAME              24 (AdwDrawRoundText3)
+              1430 POP_TOP
+   
+   874        1432 PUSH_NULL
+              1434 LOAD_BUILD_CLASS
+              1436 LOAD_CONST             114 (<code object AdwTText, file "D:\tkadw\tkadw\windows\theme.py", line 874>)
+              1438 MAKE_FUNCTION            0
+              1440 LOAD_CONST             115 ('AdwTText')
+              1442 LOAD_NAME               24 (AdwDrawRoundText3)
+              1444 PRECALL                  3
+              1448 CALL                     3
+              1458 STORE_NAME              25 (AdwTText)
+   
+   879        1460 LOAD_CONST              49 (0)
+              1462 LOAD_CONST             116 (('AdwDrawRoundFrame3',))
+              1464 IMPORT_NAME             26 (tkadw.windows.canvas.frame)
+              1466 IMPORT_FROM             27 (AdwDrawRoundFrame3)
+              1468 STORE_NAME              27 (AdwDrawRoundFrame3)
+              1470 POP_TOP
+   
+   882        1472 PUSH_NULL
+              1474 LOAD_BUILD_CLASS
+              1476 LOAD_CONST             117 (<code object AdwTFrame, file "D:\tkadw\tkadw\windows\theme.py", line 882>)
+              1478 MAKE_FUNCTION            0
+              1480 LOAD_CONST             118 ('AdwTFrame')
+              1482 LOAD_NAME               27 (AdwDrawRoundFrame3)
+              1484 PRECALL                  3
+              1488 CALL                     3
+              1498 STORE_NAME              28 (AdwTFrame)
+   
+   887        1500 LOAD_CONST              49 (0)
+              1502 LOAD_CONST             119 (('AdwDrawSeparator',))
+              1504 IMPORT_NAME             29 (tkadw.windows.canvas.separator)
+              1506 IMPORT_FROM             30 (AdwDrawSeparator)
+              1508 STORE_NAME              30 (AdwDrawSeparator)
+              1510 POP_TOP
+   
+   890        1512 PUSH_NULL
+              1514 LOAD_BUILD_CLASS
+              1516 LOAD_CONST             120 (<code object AdwTSeparator, file "D:\tkadw\tkadw\windows\theme.py", line 890>)
+              1518 MAKE_FUNCTION            0
+              1520 LOAD_CONST             121 ('AdwTSeparator')
+              1522 LOAD_NAME               30 (AdwDrawSeparator)
+              1524 PRECALL                  3
+              1528 CALL                     3
+              1538 STORE_NAME              31 (AdwTSeparator)
+   
+   895        1540 LOAD_NAME               32 (__name__)
+              1542 LOAD_CONST             122 ('__main__')
+              1544 COMPARE_OP               2 (==)
+              1550 POP_JUMP_FORWARD_IF_FALSE   239 (to 2030)
+   
+   896        1552 LOAD_CONST              49 (0)
+              1554 LOAD_CONST             123 (('isDark',))
+              1556 IMPORT_NAME             33 (darkdetect)
+              1558 IMPORT_FROM             34 (isDark)
+              1560 STORE_NAME              34 (isDark)
+              1562 POP_TOP
+   
+   898        1564 PUSH_NULL
+              1566 LOAD_NAME               13 (Adwite)
+              1568 PRECALL                  0
+              1572 CALL                     0
+              1582 STORE_NAME              35 (root)
+   
+   899        1584 LOAD_NAME               35 (root)
+              1586 LOAD_METHOD             10 (set_default_theme)
+              1608 LOAD_CONST             124 ('metro')
+              1610 PRECALL                  1
+              1614 CALL                     1
+              1624 POP_TOP
+   
+   901        1626 LOAD_CONST             125 (<code object toggle, file "D:\tkadw\tkadw\windows\theme.py", line 901>)
+              1628 MAKE_FUNCTION            0
+              1630 STORE_NAME              36 (toggle)
+   
+   904        1632 PUSH_NULL
+              1634 LOAD_NAME               19 (AdwTButton)
+              1636 LOAD_CONST             109 ('AdwTButton')
+              1638 LOAD_NAME               36 (toggle)
+              1640 KW_NAMES               126
+              1642 PRECALL                  2
+              1646 CALL                     2
+              1656 STORE_NAME              37 (button)
+   
+   905        1658 LOAD_NAME               37 (button)
+              1660 LOAD_METHOD             38 (pack)
+              1682 LOAD_CONST             127 ('x')
+              1684 LOAD_CONST             128 (5)
+              1686 LOAD_CONST             128 (5)
+              1688 KW_NAMES               129
+              1690 PRECALL                  3
+              1694 CALL                     3
+              1704 POP_TOP
+   
+   906        1706 PUSH_NULL
+              1708 LOAD_NAME               31 (AdwTSeparator)
+              1710 PRECALL                  0
+              1714 CALL                     0
+              1724 STORE_NAME              39 (separator)
+   
+   907        1726 LOAD_NAME               39 (separator)
+              1728 LOAD_METHOD             38 (pack)
+              1750 LOAD_CONST             127 ('x')
+              1752 LOAD_CONST             128 (5)
+              1754 LOAD_CONST             128 (5)
+              1756 KW_NAMES               129
+              1758 PRECALL                  3
+              1762 CALL                     3
+              1772 POP_TOP
+   
+   908        1774 PUSH_NULL
+              1776 LOAD_NAME               22 (AdwTEntry)
+              1778 LOAD_CONST             112 ('AdwTEntry')
+              1780 KW_NAMES               130
+              1782 PRECALL                  1
+              1786 CALL                     1
+              1796 STORE_NAME              40 (entry)
+   
+   909        1798 LOAD_NAME               40 (entry)
+              1800 LOAD_METHOD             38 (pack)
+              1822 LOAD_CONST             127 ('x')
+              1824 LOAD_CONST             128 (5)
+              1826 LOAD_CONST             128 (5)
+              1828 KW_NAMES               129
+              1830 PRECALL                  3
+              1834 CALL                     3
+              1844 POP_TOP
+   
+   910        1846 PUSH_NULL
+              1848 LOAD_NAME               25 (AdwTText)
+              1850 LOAD_CONST             115 ('AdwTText')
+              1852 KW_NAMES               130
+              1854 PRECALL                  1
+              1858 CALL                     1
+              1868 STORE_NAME              41 (text)
+   
+   911        1870 LOAD_NAME               41 (text)
+              1872 LOAD_METHOD             38 (pack)
+              1894 LOAD_CONST             127 ('x')
+              1896 LOAD_CONST             128 (5)
+              1898 LOAD_CONST             128 (5)
+              1900 KW_NAMES               129
+              1902 PRECALL                  3
+              1906 CALL                     3
+              1916 POP_TOP
+   
+   912        1918 PUSH_NULL
+              1920 LOAD_NAME               28 (AdwTFrame)
+              1922 PRECALL                  0
+              1926 CALL                     0
+              1936 STORE_NAME              42 (frame)
+   
+   913        1938 LOAD_NAME               42 (frame)
+              1940 LOAD_METHOD             38 (pack)
+              1962 LOAD_CONST             127 ('x')
+              1964 LOAD_CONST             128 (5)
+              1966 LOAD_CONST             128 (5)
+              1968 KW_NAMES               129
+              1970 PRECALL                  3
+              1974 CALL                     3
+              1984 POP_TOP
+   
+   914        1986 LOAD_NAME               35 (root)
+              1988 LOAD_METHOD             43 (mainloop)
+              2010 PRECALL                  0
+              2014 CALL                     0
+              2024 POP_TOP
+              2026 LOAD_CONST             131 (None)
+              2028 RETURN_VALUE
    
-   679     >> 1706 LOAD_CONST             115 (None)
-              1708 RETURN_VALUE
+   895     >> 2030 LOAD_CONST             131 (None)
+              2032 RETURN_VALUE
    consts
       'back'
       '#f4f4f4'
       'transparent'
       '#000000'
       ('back', 'text_back')
       13
@@ -1236,62 +1535,74 @@
       '#2f3134'
       '#dcdee0'
       '#26282a'
       '#a9abad'
       '#1e2022'
       '#232527'
       '#d44e7d'
+      '#eeeeee'
+      '#666666'
+      '#333333'
+      '#bfbfbf'
+      (3, 3)
+      '#999999'
+      '#00aedb'
+      '#111111'
+      '#222222'
+      '#444444'
+      '#aaaaaa'
+      False
       code
          argcount  : 0
          nlocals   : 2
          stacksize : 4
          flags     : 3
          code
             0x9700640164026c006d017d000100640164036c026d037d010100090002
             007c017c00640419000000000000000000a6010000ab0100000000000000
             005300230074080000000000000000000024007204010059006400530077
             00780359007701
-         560           0 RESUME                   0
+         746           0 RESUME                   0
          
-         561           2 LOAD_CONST               1 (0)
+         747           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('environ',))
                        6 IMPORT_NAME              0 (os)
                        8 IMPORT_FROM              1 (environ)
                       10 STORE_FAST               0 (environ)
                       12 POP_TOP
          
-         562          14 LOAD_CONST               1 (0)
+         748          14 LOAD_CONST               1 (0)
                       16 LOAD_CONST               3 (('loads',))
                       18 IMPORT_NAME              2 (json)
                       20 IMPORT_FROM              3 (loads)
                       22 STORE_FAST               1 (loads)
                       24 POP_TOP
          
-         563          26 NOP
+         749          26 NOP
          
-         564          28 PUSH_NULL
+         750          28 PUSH_NULL
                       30 LOAD_FAST                1 (loads)
                       32 LOAD_FAST                0 (environ)
                       34 LOAD_CONST               4 ('tkAdwite.DefaultTheme')
                       36 BINARY_SUBSCR
                       46 PRECALL                  1
                       50 CALL                     1
                       60 RETURN_VALUE
                  >>   62 PUSH_EXC_INFO
          
-         565          64 LOAD_GLOBAL              8 (KeyError)
+         751          64 LOAD_GLOBAL              8 (KeyError)
                       76 CHECK_EXC_MATCH
                       78 POP_JUMP_FORWARD_IF_FALSE     4 (to 88)
                       80 POP_TOP
          
-         566          82 POP_EXCEPT
+         752          82 POP_EXCEPT
                       84 LOAD_CONST               0 (None)
                       86 RETURN_VALUE
          
-         565     >>   88 RERAISE                  0
+         751     >>   88 RERAISE                  0
                  >>   90 COPY                     3
                       92 POP_EXCEPT
                       94 RERAISE                  1
          ExceptionTable:
            28 to 58 -> 62 [0]
            62 to 80 -> 90 [1] lasti
            88 to 88 -> 90 [1] lasti
@@ -1303,41 +1614,41 @@
             'tkAdwite.DefaultTheme'
          names      ('os', 'environ', 'json', 'loads', 'KeyError')
          varnames   ('environ', 'loads')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'get_default_theme'
-         firstlineno 560
+         firstlineno 746
          lnotab 0x02010c010c0102012401120106ff
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 3
          flags     : 3
          code
             0x9700640164026c006d017d010100640164036c026d037d02010002007c
             027c00a6010000ab0100000000000000007c0164043c00000064005300
-         569           0 RESUME                   0
+         755           0 RESUME                   0
          
-         570           2 LOAD_CONST               1 (0)
+         756           2 LOAD_CONST               1 (0)
                        4 LOAD_CONST               2 (('environ',))
                        6 IMPORT_NAME              0 (os)
                        8 IMPORT_FROM              1 (environ)
                       10 STORE_FAST               1 (environ)
                       12 POP_TOP
          
-         571          14 LOAD_CONST               1 (0)
+         757          14 LOAD_CONST               1 (0)
                       16 LOAD_CONST               3 (('dumps',))
                       18 IMPORT_NAME              2 (json)
                       20 IMPORT_FROM              3 (dumps)
                       22 STORE_FAST               2 (dumps)
                       24 POP_TOP
          
-         572          26 PUSH_NULL
+         758          26 PUSH_NULL
                       28 LOAD_FAST                2 (dumps)
                       30 LOAD_FAST                0 (theme)
                       32 PRECALL                  1
                       36 CALL                     1
                       46 LOAD_FAST                1 (environ)
                       48 LOAD_CONST               4 ('tkAdwite.DefaultTheme')
                       50 STORE_SUBSCR
@@ -1351,311 +1662,512 @@
             'tkAdwite.DefaultTheme'
          names      ('os', 'environ', 'json', 'dumps')
          varnames   ('theme', 'environ', 'dumps')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       '_set_default_theme'
-         firstlineno 569
+         firstlineno 755
          lnotab 0x02010c010c01
       'system'
       code
          argcount  : 2
          nlocals   : 3
-         stacksize : 3
+         stacksize : 4
          flags     : 3
          code
             0x97007c0064016b020000000073127c0064026b0200000000730c7c0064
-            036b020000000073067c0064046b020000000072b07c01a0000000000000
+            036b020000000073067c0064046b020000000072d67c01a0000000000000
             000000000000000000000000000000a6000000ab00000000000000000064
             056b020000000073187c01a0000000000000000000000000000000000000
-            000000a6000000ab00000000000000000064066b0200000000723c640764
-            086c016d027d02010002007c02a6000000ab000000000000000000721674
-            0700000000000000000000740800000000000000000000a6010000ab0100
-            00000000000000010064005300740700000000000000000000740a000000
-            00000000000000a6010000ab0100000000000000000100640053007c01a0
-            000000000000000000000000000000000000000000a6000000ab00000000
-            000000000064096b02000000007216740700000000000000000000740800
-            000000000000000000a6010000ab01000000000000000001006400530074
-            0700000000000000000000740a00000000000000000000a6010000ab0100
-            000000000000000100640053007c00640a6b020000000073067c00640b6b
-            020000000072b07c01a00000000000000000000000000000000000000000
-            00a6000000ab00000000000000000064056b020000000073187c01a00000
-            00000000000000000000000000000000000000a6000000ab000000000000
-            00000064066b0200000000723c640764086c016d027d02010002007c02a6
-            000000ab0000000000000000007216740700000000000000000000740c00
-            000000000000000000a6010000ab01000000000000000001006400530074
-            0700000000000000000000740e00000000000000000000a6010000ab0100
-            000000000000000100640053007c01a00000000000000000000000000000
+            000000a6000000ab00000000000000000064066b02000000007262090064
+            0764086c016d027d02010002007c02a6000000ab00000000000000000072
+            16740700000000000000000000740800000000000000000000a6010000ab
+            010000000000000000010064005300740700000000000000000000740a00
+            000000000000000000a6010000ab01000000000000000001006400530023
+            00740c000000000000000000002400721801007407000000000000000000
+            00740a00000000000000000000a6010000ab010000000000000000010059
+            006400530077007803590077017c01a00000000000000000000000000000
             00000000000000a6000000ab00000000000000000064096b020000000072
-            16740700000000000000000000740c00000000000000000000a6010000ab
-            010000000000000000010064005300740700000000000000000000740e00
+            16740700000000000000000000740800000000000000000000a6010000ab
+            010000000000000000010064005300740700000000000000000000740a00
             000000000000000000a6010000ab0100000000000000000100640053007c
-            00640c6b020000000073067c00640d6b020000000072b07c01a000000000
+            00640a6b020000000073067c00640b6b020000000072d67c01a000000000
             0000000000000000000000000000000000a6000000ab0000000000000000
             0064056b020000000073187c01a000000000000000000000000000000000
-            0000000000a6000000ab00000000000000000064066b0200000000723c64
-            0764086c016d027d02010002007c02a6000000ab00000000000000000072
-            16740700000000000000000000741000000000000000000000a6010000ab
-            010000000000000000010064005300740700000000000000000000741200
-            000000000000000000a6010000ab0100000000000000000100640053007c
-            01a0000000000000000000000000000000000000000000a6000000ab0000
-            0000000000000064096b0200000000721674070000000000000000000074
+            0000000000a6000000ab00000000000000000064066b0200000000726209
+            00640764086c016d027d02010002007c02a6000000ab0000000000000000
+            007216740700000000000000000000740e00000000000000000000a60100
+            00ab01000000000000000001006400530074070000000000000000000074
+            1000000000000000000000a6010000ab0100000000000000000100640053
+            002300740c00000000000000000000240072180100740700000000000000
+            000000741000000000000000000000a6010000ab01000000000000000001
+            0059006400530077007803590077017c01a0000000000000000000000000
+            000000000000000000a6000000ab00000000000000000064096b02000000
+            007216740700000000000000000000740e00000000000000000000a60100
+            00ab01000000000000000001006400530074070000000000000000000074
             1000000000000000000000a6010000ab0100000000000000000100640053
-            00740700000000000000000000741200000000000000000000a6010000ab
-            0100000000000000000100640053007407000000000000000000007c00a6
-            010000ab010000000000000000010064005300
-         575           0 RESUME                   0
+            007c00640c6b020000000073067c00640d6b020000000072d67c01a00000
+            00000000000000000000000000000000000000a6000000ab000000000000
+            00000064056b020000000073187c01a00000000000000000000000000000
+            00000000000000a6000000ab00000000000000000064066b020000000072
+            620900640764086c016d027d02010002007c02a6000000ab000000000000
+            0000007216740700000000000000000000741200000000000000000000a6
+            010000ab0100000000000000000100640053007407000000000000000000
+            00741400000000000000000000a6010000ab010000000000000000010064
+            0053002300740c0000000000000000000024007218010074070000000000
+            0000000000741400000000000000000000a6010000ab0100000000000000
+            00010059006400530077007803590077017c01a000000000000000000000
+            0000000000000000000000a6000000ab00000000000000000064096b0200
+            0000007216740700000000000000000000741200000000000000000000a6
+            010000ab0100000000000000000100640053007407000000000000000000
+            00741400000000000000000000a6010000ab010000000000000000010064
+            0053007c00640e6b020000000073067c00640f6b020000000072d67c01a0
+            000000000000000000000000000000000000000000a6000000ab00000000
+            000000000064056b020000000073187c01a0000000000000000000000000
+            000000000000000000a6000000ab00000000000000000064066b02000000
+            0072620900640764086c016d027d02010002007c02a6000000ab00000000
+            000000000072167407000000000000000000007416000000000000000000
+            00a6010000ab010000000000000000010064005300740700000000000000
+            000000741800000000000000000000a6010000ab01000000000000000001
+            00640053002300740c000000000000000000002400721801007407000000
+            00000000000000741800000000000000000000a6010000ab010000000000
+            000000010059006400530077007803590077017c01a00000000000000000
+            00000000000000000000000000a6000000ab00000000000000000064096b
+            020000000072167407000000000000000000007416000000000000000000
+            00a6010000ab010000000000000000010064005300740700000000000000
+            000000741800000000000000000000a6010000ab01000000000000000001
+            00640053007407000000000000000000007c00a6010000ab010000000000
+            000000010064005300
+         761           0 RESUME                   0
          
-         576           2 LOAD_FAST                0 (theme)
+         762           2 LOAD_FAST                0 (theme)
                        4 LOAD_CONST               1 ('win11')
                        6 COMPARE_OP               2 (==)
                       12 POP_JUMP_FORWARD_IF_TRUE    18 (to 50)
                       14 LOAD_FAST                0 (theme)
                       16 LOAD_CONST               2 ('windows11')
                       18 COMPARE_OP               2 (==)
                       24 POP_JUMP_FORWARD_IF_TRUE    12 (to 50)
                       26 LOAD_FAST                0 (theme)
                       28 LOAD_CONST               3 ('Windows11')
                       30 COMPARE_OP               2 (==)
                       36 POP_JUMP_FORWARD_IF_TRUE     6 (to 50)
                       38 LOAD_FAST                0 (theme)
                       40 LOAD_CONST               4 ('Win11')
                       42 COMPARE_OP               2 (==)
-                      48 POP_JUMP_FORWARD_IF_FALSE   176 (to 402)
+                      48 POP_JUMP_FORWARD_IF_FALSE   214 (to 478)
          
-         577     >>   50 LOAD_FAST                1 (mode)
+         763     >>   50 LOAD_FAST                1 (mode)
                       52 LOAD_METHOD              0 (lower)
                       74 PRECALL                  0
                       78 CALL                     0
                       88 LOAD_CONST               5 ('system')
                       90 COMPARE_OP               2 (==)
                       96 POP_JUMP_FORWARD_IF_TRUE    24 (to 146)
                       98 LOAD_FAST                1 (mode)
                      100 LOAD_METHOD              0 (lower)
                      122 PRECALL                  0
                      126 CALL                     0
                      136 LOAD_CONST               6 ('auto')
                      138 COMPARE_OP               2 (==)
-                     144 POP_JUMP_FORWARD_IF_FALSE    60 (to 266)
+                     144 POP_JUMP_FORWARD_IF_FALSE    98 (to 342)
+         
+         764     >>  146 NOP
          
-         578     >>  146 LOAD_CONST               7 (0)
-                     148 LOAD_CONST               8 (('isDark',))
-                     150 IMPORT_NAME              1 (darkdetect)
-                     152 IMPORT_FROM              2 (isDark)
-                     154 STORE_FAST               2 (isDark)
-                     156 POP_TOP
-         
-         579         158 PUSH_NULL
-                     160 LOAD_FAST                2 (isDark)
-                     162 PRECALL                  0
-                     166 CALL                     0
-                     176 POP_JUMP_FORWARD_IF_FALSE    22 (to 222)
-         
-         580         178 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     190 LOAD_GLOBAL              8 (win11_dark_theme)
-                     202 PRECALL                  1
-                     206 CALL                     1
-                     216 POP_TOP
-                     218 LOAD_CONST               0 (None)
-                     220 RETURN_VALUE
-         
-         582     >>  222 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     234 LOAD_GLOBAL             10 (win11_theme)
-                     246 PRECALL                  1
-                     250 CALL                     1
-                     260 POP_TOP
-                     262 LOAD_CONST               0 (None)
-                     264 RETURN_VALUE
-         
-         583     >>  266 LOAD_FAST                1 (mode)
-                     268 LOAD_METHOD              0 (lower)
-                     290 PRECALL                  0
-                     294 CALL                     0
-                     304 LOAD_CONST               9 ('dark')
-                     306 COMPARE_OP               2 (==)
-                     312 POP_JUMP_FORWARD_IF_FALSE    22 (to 358)
-         
-         584         314 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     326 LOAD_GLOBAL              8 (win11_dark_theme)
-                     338 PRECALL                  1
-                     342 CALL                     1
-                     352 POP_TOP
-                     354 LOAD_CONST               0 (None)
-                     356 RETURN_VALUE
-         
-         586     >>  358 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     370 LOAD_GLOBAL             10 (win11_theme)
-                     382 PRECALL                  1
-                     386 CALL                     1
-                     396 POP_TOP
-                     398 LOAD_CONST               0 (None)
-                     400 RETURN_VALUE
-         
-         587     >>  402 LOAD_FAST                0 (theme)
-                     404 LOAD_CONST              10 ('gtk')
-                     406 COMPARE_OP               2 (==)
-                     412 POP_JUMP_FORWARD_IF_TRUE     6 (to 426)
-                     414 LOAD_FAST                0 (theme)
-                     416 LOAD_CONST              11 ('Gtk')
-                     418 COMPARE_OP               2 (==)
-                     424 POP_JUMP_FORWARD_IF_FALSE   176 (to 778)
-         
-         588     >>  426 LOAD_FAST                1 (mode)
-                     428 LOAD_METHOD              0 (lower)
-                     450 PRECALL                  0
-                     454 CALL                     0
-                     464 LOAD_CONST               5 ('system')
-                     466 COMPARE_OP               2 (==)
-                     472 POP_JUMP_FORWARD_IF_TRUE    24 (to 522)
-                     474 LOAD_FAST                1 (mode)
-                     476 LOAD_METHOD              0 (lower)
-                     498 PRECALL                  0
-                     502 CALL                     0
-                     512 LOAD_CONST               6 ('auto')
-                     514 COMPARE_OP               2 (==)
-                     520 POP_JUMP_FORWARD_IF_FALSE    60 (to 642)
-         
-         589     >>  522 LOAD_CONST               7 (0)
-                     524 LOAD_CONST               8 (('isDark',))
-                     526 IMPORT_NAME              1 (darkdetect)
-                     528 IMPORT_FROM              2 (isDark)
-                     530 STORE_FAST               2 (isDark)
-                     532 POP_TOP
-         
-         590         534 PUSH_NULL
-                     536 LOAD_FAST                2 (isDark)
-                     538 PRECALL                  0
-                     542 CALL                     0
-                     552 POP_JUMP_FORWARD_IF_FALSE    22 (to 598)
-         
-         591         554 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     566 LOAD_GLOBAL             12 (gtk_dark_theme)
-                     578 PRECALL                  1
-                     582 CALL                     1
-                     592 POP_TOP
-                     594 LOAD_CONST               0 (None)
-                     596 RETURN_VALUE
-         
-         593     >>  598 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     610 LOAD_GLOBAL             14 (gtk_theme)
-                     622 PRECALL                  1
-                     626 CALL                     1
-                     636 POP_TOP
-                     638 LOAD_CONST               0 (None)
-                     640 RETURN_VALUE
-         
-         594     >>  642 LOAD_FAST                1 (mode)
-                     644 LOAD_METHOD              0 (lower)
-                     666 PRECALL                  0
-                     670 CALL                     0
-                     680 LOAD_CONST               9 ('dark')
-                     682 COMPARE_OP               2 (==)
-                     688 POP_JUMP_FORWARD_IF_FALSE    22 (to 734)
-         
-         595         690 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     702 LOAD_GLOBAL             12 (gtk_dark_theme)
-                     714 PRECALL                  1
-                     718 CALL                     1
-                     728 POP_TOP
-                     730 LOAD_CONST               0 (None)
-                     732 RETURN_VALUE
-         
-         597     >>  734 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     746 LOAD_GLOBAL             14 (gtk_theme)
-                     758 PRECALL                  1
-                     762 CALL                     1
-                     772 POP_TOP
-                     774 LOAD_CONST               0 (None)
-                     776 RETURN_VALUE
-         
-         598     >>  778 LOAD_FAST                0 (theme)
-                     780 LOAD_CONST              12 ('bilibili')
-                     782 COMPARE_OP               2 (==)
-                     788 POP_JUMP_FORWARD_IF_TRUE     6 (to 802)
-                     790 LOAD_FAST                0 (theme)
-                     792 LOAD_CONST              13 ('BiliBili')
-                     794 COMPARE_OP               2 (==)
-                     800 POP_JUMP_FORWARD_IF_FALSE   176 (to 1154)
-         
-         599     >>  802 LOAD_FAST                1 (mode)
-                     804 LOAD_METHOD              0 (lower)
-                     826 PRECALL                  0
-                     830 CALL                     0
-                     840 LOAD_CONST               5 ('system')
-                     842 COMPARE_OP               2 (==)
-                     848 POP_JUMP_FORWARD_IF_TRUE    24 (to 898)
-                     850 LOAD_FAST                1 (mode)
-                     852 LOAD_METHOD              0 (lower)
-                     874 PRECALL                  0
-                     878 CALL                     0
-                     888 LOAD_CONST               6 ('auto')
-                     890 COMPARE_OP               2 (==)
-                     896 POP_JUMP_FORWARD_IF_FALSE    60 (to 1018)
-         
-         600     >>  898 LOAD_CONST               7 (0)
-                     900 LOAD_CONST               8 (('isDark',))
-                     902 IMPORT_NAME              1 (darkdetect)
-                     904 IMPORT_FROM              2 (isDark)
-                     906 STORE_FAST               2 (isDark)
-                     908 POP_TOP
-         
-         601         910 PUSH_NULL
-                     912 LOAD_FAST                2 (isDark)
-                     914 PRECALL                  0
-                     918 CALL                     0
-                     928 POP_JUMP_FORWARD_IF_FALSE    22 (to 974)
-         
-         602         930 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     942 LOAD_GLOBAL             16 (bilibili_dark_theme)
-                     954 PRECALL                  1
-                     958 CALL                     1
-                     968 POP_TOP
-                     970 LOAD_CONST               0 (None)
-                     972 RETURN_VALUE
-         
-         604     >>  974 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                     986 LOAD_GLOBAL             18 (bilibili_theme)
-                     998 PRECALL                  1
-                    1002 CALL                     1
-                    1012 POP_TOP
-                    1014 LOAD_CONST               0 (None)
-                    1016 RETURN_VALUE
-         
-         605     >> 1018 LOAD_FAST                1 (mode)
-                    1020 LOAD_METHOD              0 (lower)
-                    1042 PRECALL                  0
-                    1046 CALL                     0
-                    1056 LOAD_CONST               9 ('dark')
-                    1058 COMPARE_OP               2 (==)
-                    1064 POP_JUMP_FORWARD_IF_FALSE    22 (to 1110)
-         
-         606        1066 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1078 LOAD_GLOBAL             16 (bilibili_dark_theme)
-                    1090 PRECALL                  1
-                    1094 CALL                     1
-                    1104 POP_TOP
-                    1106 LOAD_CONST               0 (None)
-                    1108 RETURN_VALUE
-         
-         608     >> 1110 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1122 LOAD_GLOBAL             18 (bilibili_theme)
-                    1134 PRECALL                  1
-                    1138 CALL                     1
-                    1148 POP_TOP
-                    1150 LOAD_CONST               0 (None)
-                    1152 RETURN_VALUE
-         
-         610     >> 1154 LOAD_GLOBAL              7 (NULL + _set_default_theme)
-                    1166 LOAD_FAST                0 (theme)
-                    1168 PRECALL                  1
-                    1172 CALL                     1
-                    1182 POP_TOP
-                    1184 LOAD_CONST               0 (None)
-                    1186 RETURN_VALUE
+         765         148 LOAD_CONST               7 (0)
+                     150 LOAD_CONST               8 (('isDark',))
+                     152 IMPORT_NAME              1 (darkdetect)
+                     154 IMPORT_FROM              2 (isDark)
+                     156 STORE_FAST               2 (isDark)
+                     158 POP_TOP
+         
+         769         160 PUSH_NULL
+                     162 LOAD_FAST                2 (isDark)
+                     164 PRECALL                  0
+                     168 CALL                     0
+                     178 POP_JUMP_FORWARD_IF_FALSE    22 (to 224)
+         
+         770         180 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     192 LOAD_GLOBAL              8 (win11_dark_theme)
+                     204 PRECALL                  1
+                     208 CALL                     1
+                     218 POP_TOP
+                     220 LOAD_CONST               0 (None)
+                     222 RETURN_VALUE
+         
+         772     >>  224 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     236 LOAD_GLOBAL             10 (win11_theme)
+                     248 PRECALL                  1
+                     252 CALL                     1
+                     262 POP_TOP
+                     264 LOAD_CONST               0 (None)
+                     266 RETURN_VALUE
+                 >>  268 PUSH_EXC_INFO
+         
+         766         270 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                     282 CHECK_EXC_MATCH
+                     284 POP_JUMP_FORWARD_IF_FALSE    24 (to 334)
+                     286 POP_TOP
+         
+         767         288 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     300 LOAD_GLOBAL             10 (win11_theme)
+                     312 PRECALL                  1
+                     316 CALL                     1
+                     326 POP_TOP
+                     328 POP_EXCEPT
+                     330 LOAD_CONST               0 (None)
+                     332 RETURN_VALUE
+         
+         766     >>  334 RERAISE                  0
+                 >>  336 COPY                     3
+                     338 POP_EXCEPT
+                     340 RERAISE                  1
+         
+         773     >>  342 LOAD_FAST                1 (mode)
+                     344 LOAD_METHOD              0 (lower)
+                     366 PRECALL                  0
+                     370 CALL                     0
+                     380 LOAD_CONST               9 ('dark')
+                     382 COMPARE_OP               2 (==)
+                     388 POP_JUMP_FORWARD_IF_FALSE    22 (to 434)
+         
+         774         390 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     402 LOAD_GLOBAL              8 (win11_dark_theme)
+                     414 PRECALL                  1
+                     418 CALL                     1
+                     428 POP_TOP
+                     430 LOAD_CONST               0 (None)
+                     432 RETURN_VALUE
+         
+         776     >>  434 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     446 LOAD_GLOBAL             10 (win11_theme)
+                     458 PRECALL                  1
+                     462 CALL                     1
+                     472 POP_TOP
+                     474 LOAD_CONST               0 (None)
+                     476 RETURN_VALUE
+         
+         777     >>  478 LOAD_FAST                0 (theme)
+                     480 LOAD_CONST              10 ('gtk')
+                     482 COMPARE_OP               2 (==)
+                     488 POP_JUMP_FORWARD_IF_TRUE     6 (to 502)
+                     490 LOAD_FAST                0 (theme)
+                     492 LOAD_CONST              11 ('Gtk')
+                     494 COMPARE_OP               2 (==)
+                     500 POP_JUMP_FORWARD_IF_FALSE   214 (to 930)
+         
+         778     >>  502 LOAD_FAST                1 (mode)
+                     504 LOAD_METHOD              0 (lower)
+                     526 PRECALL                  0
+                     530 CALL                     0
+                     540 LOAD_CONST               5 ('system')
+                     542 COMPARE_OP               2 (==)
+                     548 POP_JUMP_FORWARD_IF_TRUE    24 (to 598)
+                     550 LOAD_FAST                1 (mode)
+                     552 LOAD_METHOD              0 (lower)
+                     574 PRECALL                  0
+                     578 CALL                     0
+                     588 LOAD_CONST               6 ('auto')
+                     590 COMPARE_OP               2 (==)
+                     596 POP_JUMP_FORWARD_IF_FALSE    98 (to 794)
+         
+         779     >>  598 NOP
+         
+         780         600 LOAD_CONST               7 (0)
+                     602 LOAD_CONST               8 (('isDark',))
+                     604 IMPORT_NAME              1 (darkdetect)
+                     606 IMPORT_FROM              2 (isDark)
+                     608 STORE_FAST               2 (isDark)
+                     610 POP_TOP
+         
+         784         612 PUSH_NULL
+                     614 LOAD_FAST                2 (isDark)
+                     616 PRECALL                  0
+                     620 CALL                     0
+                     630 POP_JUMP_FORWARD_IF_FALSE    22 (to 676)
+         
+         785         632 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     644 LOAD_GLOBAL             14 (gtk_dark_theme)
+                     656 PRECALL                  1
+                     660 CALL                     1
+                     670 POP_TOP
+                     672 LOAD_CONST               0 (None)
+                     674 RETURN_VALUE
+         
+         787     >>  676 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     688 LOAD_GLOBAL             16 (gtk_theme)
+                     700 PRECALL                  1
+                     704 CALL                     1
+                     714 POP_TOP
+                     716 LOAD_CONST               0 (None)
+                     718 RETURN_VALUE
+                 >>  720 PUSH_EXC_INFO
+         
+         781         722 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                     734 CHECK_EXC_MATCH
+                     736 POP_JUMP_FORWARD_IF_FALSE    24 (to 786)
+                     738 POP_TOP
+         
+         782         740 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     752 LOAD_GLOBAL             16 (gtk_theme)
+                     764 PRECALL                  1
+                     768 CALL                     1
+                     778 POP_TOP
+                     780 POP_EXCEPT
+                     782 LOAD_CONST               0 (None)
+                     784 RETURN_VALUE
+         
+         781     >>  786 RERAISE                  0
+                 >>  788 COPY                     3
+                     790 POP_EXCEPT
+                     792 RERAISE                  1
+         
+         789     >>  794 LOAD_FAST                1 (mode)
+                     796 LOAD_METHOD              0 (lower)
+                     818 PRECALL                  0
+                     822 CALL                     0
+                     832 LOAD_CONST               9 ('dark')
+                     834 COMPARE_OP               2 (==)
+                     840 POP_JUMP_FORWARD_IF_FALSE    22 (to 886)
+         
+         790         842 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     854 LOAD_GLOBAL             14 (gtk_dark_theme)
+                     866 PRECALL                  1
+                     870 CALL                     1
+                     880 POP_TOP
+                     882 LOAD_CONST               0 (None)
+                     884 RETURN_VALUE
+         
+         792     >>  886 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                     898 LOAD_GLOBAL             16 (gtk_theme)
+                     910 PRECALL                  1
+                     914 CALL                     1
+                     924 POP_TOP
+                     926 LOAD_CONST               0 (None)
+                     928 RETURN_VALUE
+         
+         793     >>  930 LOAD_FAST                0 (theme)
+                     932 LOAD_CONST              12 ('bilibili')
+                     934 COMPARE_OP               2 (==)
+                     940 POP_JUMP_FORWARD_IF_TRUE     6 (to 954)
+                     942 LOAD_FAST                0 (theme)
+                     944 LOAD_CONST              13 ('BiliBili')
+                     946 COMPARE_OP               2 (==)
+                     952 POP_JUMP_FORWARD_IF_FALSE   214 (to 1382)
+         
+         794     >>  954 LOAD_FAST                1 (mode)
+                     956 LOAD_METHOD              0 (lower)
+                     978 PRECALL                  0
+                     982 CALL                     0
+                     992 LOAD_CONST               5 ('system')
+                     994 COMPARE_OP               2 (==)
+                    1000 POP_JUMP_FORWARD_IF_TRUE    24 (to 1050)
+                    1002 LOAD_FAST                1 (mode)
+                    1004 LOAD_METHOD              0 (lower)
+                    1026 PRECALL                  0
+                    1030 CALL                     0
+                    1040 LOAD_CONST               6 ('auto')
+                    1042 COMPARE_OP               2 (==)
+                    1048 POP_JUMP_FORWARD_IF_FALSE    98 (to 1246)
+         
+         795     >> 1050 NOP
+         
+         796        1052 LOAD_CONST               7 (0)
+                    1054 LOAD_CONST               8 (('isDark',))
+                    1056 IMPORT_NAME              1 (darkdetect)
+                    1058 IMPORT_FROM              2 (isDark)
+                    1060 STORE_FAST               2 (isDark)
+                    1062 POP_TOP
+         
+         800        1064 PUSH_NULL
+                    1066 LOAD_FAST                2 (isDark)
+                    1068 PRECALL                  0
+                    1072 CALL                     0
+                    1082 POP_JUMP_FORWARD_IF_FALSE    22 (to 1128)
+         
+         801        1084 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1096 LOAD_GLOBAL             18 (bilibili_dark_theme)
+                    1108 PRECALL                  1
+                    1112 CALL                     1
+                    1122 POP_TOP
+                    1124 LOAD_CONST               0 (None)
+                    1126 RETURN_VALUE
+         
+         803     >> 1128 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1140 LOAD_GLOBAL             20 (bilibili_theme)
+                    1152 PRECALL                  1
+                    1156 CALL                     1
+                    1166 POP_TOP
+                    1168 LOAD_CONST               0 (None)
+                    1170 RETURN_VALUE
+                 >> 1172 PUSH_EXC_INFO
+         
+         797        1174 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                    1186 CHECK_EXC_MATCH
+                    1188 POP_JUMP_FORWARD_IF_FALSE    24 (to 1238)
+                    1190 POP_TOP
+         
+         798        1192 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1204 LOAD_GLOBAL             20 (bilibili_theme)
+                    1216 PRECALL                  1
+                    1220 CALL                     1
+                    1230 POP_TOP
+                    1232 POP_EXCEPT
+                    1234 LOAD_CONST               0 (None)
+                    1236 RETURN_VALUE
+         
+         797     >> 1238 RERAISE                  0
+                 >> 1240 COPY                     3
+                    1242 POP_EXCEPT
+                    1244 RERAISE                  1
+         
+         804     >> 1246 LOAD_FAST                1 (mode)
+                    1248 LOAD_METHOD              0 (lower)
+                    1270 PRECALL                  0
+                    1274 CALL                     0
+                    1284 LOAD_CONST               9 ('dark')
+                    1286 COMPARE_OP               2 (==)
+                    1292 POP_JUMP_FORWARD_IF_FALSE    22 (to 1338)
+         
+         805        1294 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1306 LOAD_GLOBAL             18 (bilibili_dark_theme)
+                    1318 PRECALL                  1
+                    1322 CALL                     1
+                    1332 POP_TOP
+                    1334 LOAD_CONST               0 (None)
+                    1336 RETURN_VALUE
+         
+         807     >> 1338 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1350 LOAD_GLOBAL             20 (bilibili_theme)
+                    1362 PRECALL                  1
+                    1366 CALL                     1
+                    1376 POP_TOP
+                    1378 LOAD_CONST               0 (None)
+                    1380 RETURN_VALUE
+         
+         808     >> 1382 LOAD_FAST                0 (theme)
+                    1384 LOAD_CONST              14 ('metro')
+                    1386 COMPARE_OP               2 (==)
+                    1392 POP_JUMP_FORWARD_IF_TRUE     6 (to 1406)
+                    1394 LOAD_FAST                0 (theme)
+                    1396 LOAD_CONST              15 ('Metro')
+                    1398 COMPARE_OP               2 (==)
+                    1404 POP_JUMP_FORWARD_IF_FALSE   214 (to 1834)
+         
+         809     >> 1406 LOAD_FAST                1 (mode)
+                    1408 LOAD_METHOD              0 (lower)
+                    1430 PRECALL                  0
+                    1434 CALL                     0
+                    1444 LOAD_CONST               5 ('system')
+                    1446 COMPARE_OP               2 (==)
+                    1452 POP_JUMP_FORWARD_IF_TRUE    24 (to 1502)
+                    1454 LOAD_FAST                1 (mode)
+                    1456 LOAD_METHOD              0 (lower)
+                    1478 PRECALL                  0
+                    1482 CALL                     0
+                    1492 LOAD_CONST               6 ('auto')
+                    1494 COMPARE_OP               2 (==)
+                    1500 POP_JUMP_FORWARD_IF_FALSE    98 (to 1698)
+         
+         810     >> 1502 NOP
+         
+         811        1504 LOAD_CONST               7 (0)
+                    1506 LOAD_CONST               8 (('isDark',))
+                    1508 IMPORT_NAME              1 (darkdetect)
+                    1510 IMPORT_FROM              2 (isDark)
+                    1512 STORE_FAST               2 (isDark)
+                    1514 POP_TOP
+         
+         815        1516 PUSH_NULL
+                    1518 LOAD_FAST                2 (isDark)
+                    1520 PRECALL                  0
+                    1524 CALL                     0
+                    1534 POP_JUMP_FORWARD_IF_FALSE    22 (to 1580)
+         
+         816        1536 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1548 LOAD_GLOBAL             22 (metro_dark_theme)
+                    1560 PRECALL                  1
+                    1564 CALL                     1
+                    1574 POP_TOP
+                    1576 LOAD_CONST               0 (None)
+                    1578 RETURN_VALUE
+         
+         818     >> 1580 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1592 LOAD_GLOBAL             24 (metro_theme)
+                    1604 PRECALL                  1
+                    1608 CALL                     1
+                    1618 POP_TOP
+                    1620 LOAD_CONST               0 (None)
+                    1622 RETURN_VALUE
+                 >> 1624 PUSH_EXC_INFO
+         
+         812        1626 LOAD_GLOBAL             12 (ModuleNotFoundError)
+                    1638 CHECK_EXC_MATCH
+                    1640 POP_JUMP_FORWARD_IF_FALSE    24 (to 1690)
+                    1642 POP_TOP
+         
+         813        1644 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1656 LOAD_GLOBAL             24 (metro_theme)
+                    1668 PRECALL                  1
+                    1672 CALL                     1
+                    1682 POP_TOP
+                    1684 POP_EXCEPT
+                    1686 LOAD_CONST               0 (None)
+                    1688 RETURN_VALUE
+         
+         812     >> 1690 RERAISE                  0
+                 >> 1692 COPY                     3
+                    1694 POP_EXCEPT
+                    1696 RERAISE                  1
+         
+         819     >> 1698 LOAD_FAST                1 (mode)
+                    1700 LOAD_METHOD              0 (lower)
+                    1722 PRECALL                  0
+                    1726 CALL                     0
+                    1736 LOAD_CONST               9 ('dark')
+                    1738 COMPARE_OP               2 (==)
+                    1744 POP_JUMP_FORWARD_IF_FALSE    22 (to 1790)
+         
+         820        1746 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1758 LOAD_GLOBAL             22 (metro_dark_theme)
+                    1770 PRECALL                  1
+                    1774 CALL                     1
+                    1784 POP_TOP
+                    1786 LOAD_CONST               0 (None)
+                    1788 RETURN_VALUE
+         
+         822     >> 1790 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1802 LOAD_GLOBAL             24 (metro_theme)
+                    1814 PRECALL                  1
+                    1818 CALL                     1
+                    1828 POP_TOP
+                    1830 LOAD_CONST               0 (None)
+                    1832 RETURN_VALUE
+         
+         824     >> 1834 LOAD_GLOBAL              7 (NULL + _set_default_theme)
+                    1846 LOAD_FAST                0 (theme)
+                    1848 PRECALL                  1
+                    1852 CALL                     1
+                    1862 POP_TOP
+                    1864 LOAD_CONST               0 (None)
+                    1866 RETURN_VALUE
+         ExceptionTable:
+           148 to 158 -> 268 [0]
+           268 to 326 -> 336 [1] lasti
+           334 to 334 -> 336 [1] lasti
+           600 to 610 -> 720 [0]
+           720 to 778 -> 788 [1] lasti
+           786 to 786 -> 788 [1] lasti
+           1052 to 1062 -> 1172 [0]
+           1172 to 1230 -> 1240 [1] lasti
+           1238 to 1238 -> 1240 [1] lasti
+           1504 to 1514 -> 1624 [0]
+           1624 to 1682 -> 1692 [1] lasti
+           1690 to 1690 -> 1692 [1] lasti
          consts
             None
             'win11'
             'windows11'
             'Windows11'
             'Win11'
             'system'
@@ -1663,133 +2175,163 @@
             0
             ('isDark',)
             'dark'
             'gtk'
             'Gtk'
             'bilibili'
             'BiliBili'
-         names      ('lower', 'darkdetect', 'isDark', '_set_default_theme', 'win11_dark_theme', 'win11_theme', 'gtk_dark_theme', 'gtk_theme', 'bilibili_dark_theme', 'bilibili_theme')
+            'metro'
+            'Metro'
+         names      ('lower', 'darkdetect', 'isDark', '_set_default_theme', 'win11_dark_theme', 'win11_theme', 'ModuleNotFoundError', 'gtk_dark_theme', 'gtk_theme', 'bilibili_dark_theme', 'bilibili_theme', 'metro_dark_theme', 'metro_theme')
          varnames   ('theme', 'mode', 'isDark')
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'set_default_theme'
-         firstlineno 575
+         firstlineno 761
          lnotab
-            0x0201300160010c0114012c022c0130012c022c01180160010c0114012c
-            022c0130012c022c01180160010c0114012c022c0130012c022c02
+            0x02013001600102010c0414012c022efa12012eff080730012c022c0118
+            01600102010c0414012c022efa12012eff080830012c022c011801600102
+            010c0414012c022efa12012eff080730012c022c011801600102010c0414
+            012c022efa12012eff080730012c022c02
       'win11'
       ('Adw',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code 0x970065005a0164005a026405640284015a03640384005a0464045300
-         619           0 RESUME                   0
+         833           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Adwite')
                        8 STORE_NAME               2 (__qualname__)
          
-         620          10 LOAD_CONST               5 (('auto',))
-                      12 LOAD_CONST               2 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 620>)
+         834          10 LOAD_CONST               5 (('auto',))
+                      12 LOAD_CONST               2 (<code object set_default_theme, file "D:\tkadw\tkadw\windows\theme.py", line 834>)
                       14 MAKE_FUNCTION            1 (defaults)
                       16 STORE_NAME               3 (set_default_theme)
          
-         627          18 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 627>)
+         843          18 LOAD_CONST               3 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 843>)
                       20 MAKE_FUNCTION            0
                       22 STORE_NAME               4 (default_palette)
                       24 LOAD_CONST               4 (None)
                       26 RETURN_VALUE
          consts
             'Adwite'
             'auto'
             code
                argcount  : 3
                nlocals   : 4
-               stacksize : 5
+               stacksize : 6
                flags     : 3
                code
                   0x97007401000000000000000000007c017c02a6020000ab020000000000
                   00000001007c00a0010000000000000000000000000000000000000000a6
-                  000000ab00000000000000000044005d337d037405000000000000000000
-                  007c036401a6020000ab02000000000000000072217c03a0030000000000
+                  000000ab00000000000000000044005d767d037405000000000000000000
+                  007c036401a6020000ab02000000000000000072647c03a0030000000000
                   000000000000000000000000000000740900000000000000000000a60000
-                  00ab000000000000000000a6010000ab01000000000000000001008c347c
-                  00a003000000000000000000000000000000000000000074090000000000
-                  0000000000a6000000ab000000000000000000a6010000ab010000000000
-                  000000010064005300
-               620           0 RESUME                   0
+                  00ab000000000000000000a6010000ab01000000000000000001007c03a0
+                  0500000000000000000000000000000000000000007c036a060000000000
+                  000000a00700000000000000000000000000000000000000006402a60100
+                  00ab010000000000000000ac03a6010000ab01000000000000000001007c
+                  03a00800000000000000000000000000000000000000006400a6010000ab
+                  01000000000000000001008c777c00a00300000000000000000000000000
+                  00000000000000740900000000000000000000a6000000ab000000000000
+                  000000a6010000ab010000000000000000010064005300
+               834           0 RESUME                   0
                
-               621           2 LOAD_GLOBAL              1 (NULL + set_default_theme)
+               835           2 LOAD_GLOBAL              1 (NULL + set_default_theme)
                             14 LOAD_FAST                1 (theme)
                             16 LOAD_FAST                2 (_mode)
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_TOP
                
-               622          34 LOAD_FAST                0 (self)
+               836          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (winfo_children)
                             58 PRECALL                  0
                             62 CALL                     0
                             72 GET_ITER
-                       >>   74 FOR_ITER                51 (to 178)
+                       >>   74 FOR_ITER               118 (to 312)
                             76 STORE_FAST               3 (widget)
                
-               623          78 LOAD_GLOBAL              5 (NULL + hasattr)
+               837          78 LOAD_GLOBAL              5 (NULL + hasattr)
                             90 LOAD_FAST                3 (widget)
                             92 LOAD_CONST               1 ('palette')
                             94 PRECALL                  2
                             98 CALL                     2
-                           108 POP_JUMP_FORWARD_IF_FALSE    33 (to 176)
+                           108 POP_JUMP_FORWARD_IF_FALSE   100 (to 310)
                
-               624         110 LOAD_FAST                3 (widget)
+               838         110 LOAD_FAST                3 (widget)
                            112 LOAD_METHOD              3 (palette)
                            134 LOAD_GLOBAL              9 (NULL + get_default_theme)
                            146 PRECALL                  0
                            150 CALL                     0
                            160 PRECALL                  1
                            164 CALL                     1
                            174 POP_TOP
-                       >>  176 JUMP_BACKWARD           52 (to 74)
                
-               625     >>  178 LOAD_FAST                0 (self)
-                           180 LOAD_METHOD              3 (palette)
-                           202 LOAD_GLOBAL              9 (NULL + get_default_theme)
-                           214 PRECALL                  0
-                           218 CALL                     0
-                           228 PRECALL                  1
-                           232 CALL                     1
-                           242 POP_TOP
-                           244 LOAD_CONST               0 (None)
-                           246 RETURN_VALUE
+               839         176 LOAD_FAST                3 (widget)
+                           178 LOAD_METHOD              5 (configure)
+                           200 LOAD_FAST                3 (widget)
+                           202 LOAD_ATTR                6 (master)
+                           212 LOAD_METHOD              7 (cget)
+                           234 LOAD_CONST               2 ('bg')
+                           236 PRECALL                  1
+                           240 CALL                     1
+                           250 KW_NAMES                 3
+                           252 PRECALL                  1
+                           256 CALL                     1
+                           266 POP_TOP
+               
+               840         268 LOAD_FAST                3 (widget)
+                           270 LOAD_METHOD              8 (_draw)
+                           292 LOAD_CONST               0 (None)
+                           294 PRECALL                  1
+                           298 CALL                     1
+                           308 POP_TOP
+                       >>  310 JUMP_BACKWARD          119 (to 74)
+               
+               841     >>  312 LOAD_FAST                0 (self)
+                           314 LOAD_METHOD              3 (palette)
+                           336 LOAD_GLOBAL              9 (NULL + get_default_theme)
+                           348 PRECALL                  0
+                           352 CALL                     0
+                           362 PRECALL                  1
+                           366 CALL                     1
+                           376 POP_TOP
+                           378 LOAD_CONST               0 (None)
+                           380 RETURN_VALUE
                consts
                   None
                   'palette'
-               names      ('set_default_theme', 'winfo_children', 'hasattr', 'palette', 'get_default_theme')
+                  'bg'
+                  ('background',)
+               names      ('set_default_theme', 'winfo_children', 'hasattr', 'palette', 'get_default_theme', 'configure', 'master', 'cget', '_draw')
                varnames   ('self', 'theme', '_mode', 'widget')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'set_default_theme'
-               firstlineno 620
-               lnotab 0x020120012c0120014401
+               firstlineno 834
+               lnotab 0x020120012c01200142015c012c01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               627           0 RESUME                   0
+               843           0 RESUME                   0
                
-               628           2 LOAD_FAST                0 (self)
+               844           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -1799,41 +2341,41 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 627
+               firstlineno 843
                lnotab 0x0201
             None
             ('auto',)
          names      ('__name__', '__module__', '__qualname__', 'set_default_theme', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'Adwite'
-         firstlineno 619
-         lnotab 0x0a010807
+         firstlineno 833
+         lnotab 0x0a010809
       'Adwite'
       ('AdwLabel',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         634           0 RESUME                   0
+         850           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTLabel')
                        8 STORE_NAME               2 (__qualname__)
          
-         635          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 635>)
+         851          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 851>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTLabel'
             code
@@ -1841,17 +2383,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               635           0 RESUME                   0
+               851           0 RESUME                   0
                
-               636           2 LOAD_FAST                0 (self)
+               852           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -1861,40 +2403,40 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 635
+               firstlineno 851
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTLabel'
-         firstlineno 634
+         firstlineno 850
          lnotab 0x0a01
       'AdwTLabel'
       ('AdwDrawRoundButton3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         642           0 RESUME                   0
+         858           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         643          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 643>)
+         859          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 859>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTButton'
             code
@@ -1902,17 +2444,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               643           0 RESUME                   0
+               859           0 RESUME                   0
                
-               644           2 LOAD_FAST                0 (self)
+               860           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -1922,40 +2464,40 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 643
+               firstlineno 859
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTButton'
-         firstlineno 642
+         firstlineno 858
          lnotab 0x0a01
       'AdwTButton'
       ('AdwDrawRoundEntry3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         650           0 RESUME                   0
+         866           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTEntry')
                        8 STORE_NAME               2 (__qualname__)
          
-         651          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 651>)
+         867          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 867>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTEntry'
             code
@@ -1963,17 +2505,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               651           0 RESUME                   0
+               867           0 RESUME                   0
                
-               652           2 LOAD_FAST                0 (self)
+               868           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -1983,40 +2525,40 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 651
+               firstlineno 867
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTEntry'
-         firstlineno 650
+         firstlineno 866
          lnotab 0x0a01
       'AdwTEntry'
       ('AdwDrawRoundText3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         658           0 RESUME                   0
+         874           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTText')
                        8 STORE_NAME               2 (__qualname__)
          
-         659          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 659>)
+         875          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 875>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTText'
             code
@@ -2024,17 +2566,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               659           0 RESUME                   0
+               875           0 RESUME                   0
                
-               660           2 LOAD_FAST                0 (self)
+               876           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -2044,40 +2586,40 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 659
+               firstlineno 875
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTText'
-         firstlineno 658
+         firstlineno 874
          lnotab 0x0a01
       'AdwTText'
       ('AdwDrawRoundFrame3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         666           0 RESUME                   0
+         882           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTFrame')
                        8 STORE_NAME               2 (__qualname__)
          
-         667          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 667>)
+         883          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 883>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTFrame'
             code
@@ -2085,17 +2627,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               667           0 RESUME                   0
+               883           0 RESUME                   0
                
-               668           2 LOAD_FAST                0 (self)
+               884           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -2105,40 +2647,40 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 667
+               firstlineno 883
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTFrame'
-         firstlineno 666
+         firstlineno 882
          lnotab 0x0a01
       'AdwTFrame'
       ('AdwDrawSeparator',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         674           0 RESUME                   0
+         890           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwTSeparator')
                        8 STORE_NAME               2 (__qualname__)
          
-         675          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 675>)
+         891          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\theme.py", line 891>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwTSeparator'
             code
@@ -2146,17 +2688,17 @@
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000740300
                   000000000000000000a6000000ab000000000000000000a6010000ab0100
                   00000000000000010064005300
-               675           0 RESUME                   0
+               891           0 RESUME                   0
                
-               676           2 LOAD_FAST                0 (self)
+               892           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                             26 LOAD_GLOBAL              3 (NULL + get_default_theme)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 PRECALL                  1
                             56 CALL                     1
                             66 POP_TOP
@@ -2166,34 +2708,66 @@
                   None
                names      ('palette', 'get_default_theme')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
                name       'default_palette'
-               firstlineno 675
+               firstlineno 891
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
          name       'AdwTSeparator'
-         firstlineno 674
+         firstlineno 890
          lnotab 0x0a01
       'AdwTSeparator'
       '__main__'
       ('isDark',)
+      'metro'
+      code
+         argcount  : 0
+         nlocals   : 0
+         stacksize : 3
+         flags     : 3
+         code
+            0x9700740000000000000000000000a00100000000000000000000000000
+            000000000000006401a6010000ab010000000000000000010064005300
+         901           0 RESUME                   0
+         
+         902           2 LOAD_GLOBAL              0 (root)
+                      14 LOAD_METHOD              1 (set_default_theme)
+                      36 LOAD_CONST               1 ('win11')
+                      38 PRECALL                  1
+                      42 CALL                     1
+                      52 POP_TOP
+                      54 LOAD_CONST               0 (None)
+                      56 RETURN_VALUE
+         consts
+            None
+            'win11'
+         names      ('root', 'set_default_theme')
+         varnames   ()
+         freevars   ()
+         cellvars   ()
+         filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
+         name       'toggle'
+         firstlineno 901
+         lnotab 0x0201
+      ('text', 'command')
       'x'
       5
       ('fill', 'padx', 'pady')
+      ('text',)
       None
       ('system',)
-   names      ('win11_theme', 'win11_dark_theme', 'gtk_theme', 'gtk_dark_theme', 'bilibili_theme', 'bilibili_dark_theme', 'get_default_theme', '_set_default_theme', 'set_default_theme', 'tkadw.windows.widgets.adw', 'Adw', 'Adwite', 'tkadw.windows.widgets', 'AdwLabel', 'AdwTLabel', 'tkadw.windows.canvas.button', 'AdwDrawRoundButton3', 'AdwTButton', 'tkadw.windows.canvas.entry', 'AdwDrawRoundEntry3', 'AdwTEntry', 'tkadw.windows.canvas.textbox', 'AdwDrawRoundText3', 'AdwTText', 'tkadw.windows.canvas.frame', 'AdwDrawRoundFrame3', 'AdwTFrame', 'tkadw.windows.canvas.separator', 'AdwDrawSeparator', 'AdwTSeparator', '__name__', 'darkdetect', 'isDark', 'root', 'button', 'pack', 'separator', 'entry', 'text', 'frame', 'mainloop')
+   names      ('win11_theme', 'win11_dark_theme', 'gtk_theme', 'gtk_dark_theme', 'bilibili_theme', 'bilibili_dark_theme', 'metro_theme', 'metro_dark_theme', 'get_default_theme', '_set_default_theme', 'set_default_theme', 'tkadw.windows.widgets.adw', 'Adw', 'Adwite', 'tkadw.windows.widgets', 'AdwLabel', 'AdwTLabel', 'tkadw.windows.canvas.button', 'AdwDrawRoundButton3', 'AdwTButton', 'tkadw.windows.canvas.entry', 'AdwDrawRoundEntry3', 'AdwTEntry', 'tkadw.windows.canvas.textbox', 'AdwDrawRoundText3', 'AdwTText', 'tkadw.windows.canvas.frame', 'AdwDrawRoundFrame3', 'AdwTFrame', 'tkadw.windows.canvas.separator', 'AdwDrawSeparator', 'AdwTSeparator', '__name__', 'darkdetect', 'isDark', 'root', 'toggle', 'button', 'pack', 'separator', 'entry', 'text', 'frame', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\theme.py'
    name       '<module>'
    firstlineno 1
    lnotab
@@ -2218,10 +2792,19 @@
       010201020102fc04f2041702010201020102fc0408020102020201020102
       010202020102030201020102010202020102f904f4041802010202020102
       0102010202020102030201020102010202020102f904f404180201020202
       fc04ab065f04ff0205020102fe0406020102010201020102030201020102
       0102fc040802010201020102fc04f2041702010201020102fc0408020102
       020201020102010202020102030201020102010202020102f904f4041802
       0102020201020102010202020102030201020102010202020102f904f404
-      180201020202fc04ab065e06090606082616030c031c0c0c031c050c031c
-      050c031c050c031c050c031c050c031c050c010c0214012a011401300114
-      0130011401300114013001140130012cf1
+      180201020202fc04ab065f04ff0205020102fe0406020102010201020102
+      0302010201020102fc040802010201020102fc04f2041702010201020102
+      fc0408020102020201020102010202020102030201020102010202020102
+      f904f4041802010202020102010201020202010203020102010201020202
+      0102f904f404180201020202fc04ab065f04ff0205020102fe0406020102
+      0102010201020302010201020102fc040802010201020102fc04f2041702
+      010201020102fc0408020102020201020102010202020102030201020102
+      010202020102f904f4041802010202020102010201020202010203020102
+      0102010202020102f904f404180201020202fc04ab065e06090606084216
+      030c031c0e0c031c050c031c050c031c050c031c050c031c050c031c050c
+      010c0214012a0206031a013001140130011801300118013001140130012c
+      ed
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__init__.py` & `tkadw-0.3.2/tkadw/windows/canvas/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,11 +5,13 @@
     AdwDrawRoundButton2, AdwDrawRoundDarkButton2, AdwDrawRoundAccentButton2, \
     AdwDrawRoundButton3, AdwDrawRoundDarkButton3, AdwDrawRoundAccentButton3, \
     AdwDrawCircularButton, AdwDrawCircularDarkButton
 from tkadw.windows.canvas.entry import AdwDrawEntry, AdwDrawDarkEntry, AdwDrawRoundEntry, AdwDrawRoundDarkEntry, \
     AdwDrawRoundEntry3, AdwDrawRoundDarkEntry3
 from tkadw.windows.canvas.textbox import AdwDrawText, AdwDrawDarkText, AdwDrawRoundText, AdwDrawRoundDarkText, \
     AdwDrawRoundText3, AdwDrawRoundDarkText3
+from tkadw.windows.canvas.frame import AdwDrawFrame, AdwDrawDarkFrame, AdwDrawRoundFrame, AdwDrawDarkRoundFrame, \
+    AdwDrawRoundFrame3, AdwDrawDarkRoundFrame3
 
 # 0.3加入
 from tkadw.windows.canvas.widget import AdwWidget
 # from tkadw.canvas.label import AdwDrawLabel, AdwDrawDarkLabel 已移除
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,22 +1,24 @@
 magic:    0xa70d0d0a
-moddate:  0xe1c8a464 (Wed Jul  5 01:35:29 2023 UTC)
-files sz: 974
+moddate:  0x75e0b164 (Fri Jul 14 23:55:33 2023 UTC)
+files sz: 1138
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 2
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a036d045a046d055a056d
       065a060100640064026c076d085a086d095a096d0a5a0a6d0b5a0b6d0c5a
       0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d115a116d125a126d135a136d
       145a146d155a150100640064036c166d175a176d185a186d195a196d1a5a
       1a6d1b5a1b6d1c5a1c0100640064046c1d6d1e5a1e6d1f5a1f6d205a206d
-      215a216d225a226d235a230100640064056c246d255a25010064065300
+      215a216d225a226d235a230100640064056c246d255a256d265a266d275a
+      276d285a286d295a296d2a5a2a0100640064066c2b6d2c5a2c0100640753
+      00
      0           0 RESUME                   0
    
      2           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawEngine', 'HORIZONTAL', 'VERTICAL', 'ARC', 'CIRCULAR', 'CENTRAL'))
                  6 IMPORT_NAME              0 (tkadw.windows.canvas.drawengine)
                  8 IMPORT_FROM              1 (AdwDrawEngine)
                 10 STORE_NAME               1 (AdwDrawEngine)
@@ -95,31 +97,49 @@
                150 STORE_NAME              33 (AdwDrawRoundDarkText)
                152 IMPORT_FROM             34 (AdwDrawRoundText3)
                154 STORE_NAME              34 (AdwDrawRoundText3)
                156 IMPORT_FROM             35 (AdwDrawRoundDarkText3)
                158 STORE_NAME              35 (AdwDrawRoundDarkText3)
                160 POP_TOP
    
-    14         162 LOAD_CONST               0 (0)
-               164 LOAD_CONST               5 (('AdwWidget',))
-               166 IMPORT_NAME             36 (tkadw.windows.canvas.widget)
-               168 IMPORT_FROM             37 (AdwWidget)
-               170 STORE_NAME              37 (AdwWidget)
-               172 POP_TOP
-               174 LOAD_CONST               6 (None)
-               176 RETURN_VALUE
+    12         162 LOAD_CONST               0 (0)
+               164 LOAD_CONST               5 (('AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3'))
+               166 IMPORT_NAME             36 (tkadw.windows.canvas.frame)
+               168 IMPORT_FROM             37 (AdwDrawFrame)
+               170 STORE_NAME              37 (AdwDrawFrame)
+               172 IMPORT_FROM             38 (AdwDrawDarkFrame)
+               174 STORE_NAME              38 (AdwDrawDarkFrame)
+               176 IMPORT_FROM             39 (AdwDrawRoundFrame)
+               178 STORE_NAME              39 (AdwDrawRoundFrame)
+               180 IMPORT_FROM             40 (AdwDrawDarkRoundFrame)
+               182 STORE_NAME              40 (AdwDrawDarkRoundFrame)
+               184 IMPORT_FROM             41 (AdwDrawRoundFrame3)
+               186 STORE_NAME              41 (AdwDrawRoundFrame3)
+               188 IMPORT_FROM             42 (AdwDrawDarkRoundFrame3)
+               190 STORE_NAME              42 (AdwDrawDarkRoundFrame3)
+               192 POP_TOP
+   
+    16         194 LOAD_CONST               0 (0)
+               196 LOAD_CONST               6 (('AdwWidget',))
+               198 IMPORT_NAME             43 (tkadw.windows.canvas.widget)
+               200 IMPORT_FROM             44 (AdwWidget)
+               202 STORE_NAME              44 (AdwWidget)
+               204 POP_TOP
+               206 LOAD_CONST               7 (None)
+               208 RETURN_VALUE
    consts
       0
       ('AdwDrawEngine', 'HORIZONTAL', 'VERTICAL', 'ARC', 'CIRCULAR', 'CENTRAL')
       ('AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton')
       ('AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3')
       ('AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3')
+      ('AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3')
       ('AdwWidget',)
       None
-   names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'HORIZONTAL', 'VERTICAL', 'ARC', 'CIRCULAR', 'CENTRAL', 'tkadw.windows.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.windows.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3', 'tkadw.windows.canvas.textbox', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3', 'tkadw.windows.canvas.widget', 'AdwWidget')
+   names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'HORIZONTAL', 'VERTICAL', 'ARC', 'CIRCULAR', 'CENTRAL', 'tkadw.windows.canvas.button', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawRoundButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', 'tkadw.windows.canvas.entry', 'AdwDrawEntry', 'AdwDrawDarkEntry', 'AdwDrawRoundEntry', 'AdwDrawRoundDarkEntry', 'AdwDrawRoundEntry3', 'AdwDrawRoundDarkEntry3', 'tkadw.windows.canvas.textbox', 'AdwDrawText', 'AdwDrawDarkText', 'AdwDrawRoundText', 'AdwDrawRoundDarkText', 'AdwDrawRoundText3', 'AdwDrawRoundDarkText3', 'tkadw.windows.canvas.frame', 'AdwDrawFrame', 'AdwDrawDarkFrame', 'AdwDrawRoundFrame', 'AdwDrawDarkRoundFrame', 'AdwDrawRoundFrame3', 'AdwDrawDarkRoundFrame3', 'tkadw.windows.canvas.widget', 'AdwWidget')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\__init__.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02022001400520022004
+   lnotab 0x00ff020220014005200220022004
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/button.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xe8c8a464 (Wed Jul  5 01:35:36 2023 UTC)
-files sz: 17936
+moddate:  0xdee2b064 (Fri Jul 14 05:53:34 2023 UTC)
+files sz: 18129
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -71,436 +71,449 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicButton')
                 40 LOAD_NAME                4 (AdwWidget)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicButton)
    
-   198          58 PUSH_NULL
+   210          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 198>)
+                62 LOAD_CONST               5 (<code object AdwDrawButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 210>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawButton')
                 68 LOAD_NAME                5 (AdwDrawBasicButton)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawButton)
    
-   203          86 PUSH_NULL
+   215          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 203>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 215>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkButton')
                 96 LOAD_NAME                5 (AdwDrawBasicButton)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkButton)
    
-   208         114 PUSH_NULL
+   220         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 208>)
+               118 LOAD_CONST               9 (<code object AdwDrawAccentButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 220>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawAccentButton')
                124 LOAD_NAME                5 (AdwDrawBasicButton)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawAccentButton)
    
-   237         142 PUSH_NULL
+   249         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 237>)
+               146 LOAD_CONST              11 (<code object AdwDrawBasicRoundButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 249>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawBasicRoundButton')
                152 LOAD_NAME                5 (AdwDrawBasicButton)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawBasicRoundButton)
    
-   327         170 PUSH_NULL
+   339         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 327>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 339>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundButton')
                180 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundButton)
    
-   332         198 PUSH_NULL
+   344         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 332>)
+               202 LOAD_CONST              15 (<code object AdwDrawRoundAccentButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 344>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawRoundAccentButton')
                208 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawRoundAccentButton)
    
-   361         226 PUSH_NULL
+   373         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 361>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 373>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundDarkButton')
                236 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundDarkButton)
    
-   366         254 PUSH_NULL
+   378         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 366>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 378>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundButton2')
                264 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundButton2)
    
-   395         282 PUSH_NULL
+   407         282 PUSH_NULL
                284 LOAD_BUILD_CLASS
-               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 395>)
+               286 LOAD_CONST              21 (<code object AdwDrawRoundAccentButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 407>)
                288 MAKE_FUNCTION            0
                290 LOAD_CONST              22 ('AdwDrawRoundAccentButton2')
                292 LOAD_NAME               13 (AdwDrawRoundButton2)
                294 PRECALL                  3
                298 CALL                     3
                308 STORE_NAME              14 (AdwDrawRoundAccentButton2)
    
-   424         310 PUSH_NULL
+   436         310 PUSH_NULL
                312 LOAD_BUILD_CLASS
-               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 424>)
+               314 LOAD_CONST              23 (<code object AdwDrawRoundDarkButton2, file "D:\tkadw\tkadw\windows\canvas\button.py", line 436>)
                316 MAKE_FUNCTION            0
                318 LOAD_CONST              24 ('AdwDrawRoundDarkButton2')
                320 LOAD_NAME               13 (AdwDrawRoundButton2)
                322 PRECALL                  3
                326 CALL                     3
                336 STORE_NAME              15 (AdwDrawRoundDarkButton2)
    
-   429         338 PUSH_NULL
+   441         338 PUSH_NULL
                340 LOAD_BUILD_CLASS
-               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 429>)
+               342 LOAD_CONST              25 (<code object AdwDrawRoundButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 441>)
                344 MAKE_FUNCTION            0
                346 LOAD_CONST              26 ('AdwDrawRoundButton3')
                348 LOAD_NAME                9 (AdwDrawBasicRoundButton)
                350 PRECALL                  3
                354 CALL                     3
                364 STORE_NAME              16 (AdwDrawRoundButton3)
    
-   456         366 PUSH_NULL
+   468         366 PUSH_NULL
                368 LOAD_BUILD_CLASS
-               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 456>)
+               370 LOAD_CONST              27 (<code object AdwDrawRoundAccentButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 468>)
                372 MAKE_FUNCTION            0
                374 LOAD_CONST              28 ('AdwDrawRoundAccentButton3')
                376 LOAD_NAME               16 (AdwDrawRoundButton3)
                378 PRECALL                  3
                382 CALL                     3
                392 STORE_NAME              17 (AdwDrawRoundAccentButton3)
    
-   485         394 PUSH_NULL
+   497         394 PUSH_NULL
                396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 485>)
+               398 LOAD_CONST              29 (<code object AdwDrawRoundDarkButton3, file "D:\tkadw\tkadw\windows\canvas\button.py", line 497>)
                400 MAKE_FUNCTION            0
                402 LOAD_CONST              30 ('AdwDrawRoundDarkButton3')
                404 LOAD_NAME               16 (AdwDrawRoundButton3)
                406 PRECALL                  3
                410 CALL                     3
                420 STORE_NAME              18 (AdwDrawRoundDarkButton3)
    
-   491         422 PUSH_NULL
+   503         422 PUSH_NULL
                424 LOAD_BUILD_CLASS
-               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 491>)
+               426 LOAD_CONST              31 (<code object AdwDrawBasicCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 503>)
                428 MAKE_FUNCTION            0
                430 LOAD_CONST              32 ('AdwDrawBasicCircularButton')
                432 LOAD_NAME                5 (AdwDrawBasicButton)
                434 PRECALL                  3
                438 CALL                     3
                448 STORE_NAME              19 (AdwDrawBasicCircularButton)
    
-   513         450 PUSH_NULL
+   525         450 PUSH_NULL
                452 LOAD_BUILD_CLASS
-               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 513>)
+               454 LOAD_CONST              33 (<code object AdwDrawCircularButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 525>)
                456 MAKE_FUNCTION            0
                458 LOAD_CONST              34 ('AdwDrawCircularButton')
                460 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                462 PRECALL                  3
                466 CALL                     3
                476 STORE_NAME              20 (AdwDrawCircularButton)
    
-   518         478 PUSH_NULL
+   530         478 PUSH_NULL
                480 LOAD_BUILD_CLASS
-               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 518>)
+               482 LOAD_CONST              35 (<code object AdwDrawCircularDarkButton, file "D:\tkadw\tkadw\windows\canvas\button.py", line 530>)
                484 MAKE_FUNCTION            0
                486 LOAD_CONST              36 ('AdwDrawCircularDarkButton')
                488 LOAD_NAME               19 (AdwDrawBasicCircularButton)
                490 PRECALL                  3
                494 CALL                     3
                504 STORE_NAME              21 (AdwDrawCircularDarkButton)
    
-   523         506 LOAD_NAME               22 (__name__)
+   535         506 LOAD_NAME               22 (__name__)
                508 LOAD_CONST              37 ('__main__')
                510 COMPARE_OP               2 (==)
                516 EXTENDED_ARG             1
                518 POP_JUMP_FORWARD_IF_FALSE   333 (to 1186)
    
-   524         520 LOAD_CONST               0 (0)
+   536         520 LOAD_CONST               0 (0)
                522 LOAD_CONST              38 (('Tk',))
                524 IMPORT_NAME             23 (tkinter)
                526 IMPORT_FROM             24 (Tk)
                528 STORE_NAME              24 (Tk)
                530 POP_TOP
    
-   526         532 PUSH_NULL
+   538         532 PUSH_NULL
                534 LOAD_NAME               24 (Tk)
                536 PRECALL                  0
                540 CALL                     0
                550 STORE_NAME              25 (root)
    
-   528         552 PUSH_NULL
+   540         552 PUSH_NULL
                554 LOAD_NAME                6 (AdwDrawButton)
                556 LOAD_CONST              39 ('Hello')
                558 KW_NAMES                40
                560 PRECALL                  1
                564 CALL                     1
                574 STORE_NAME              26 (button)
    
-   529         576 LOAD_NAME               26 (button)
+   541         576 LOAD_NAME               26 (button)
                578 LOAD_METHOD             27 (bind)
                600 LOAD_CONST              41 ('<<Click>>')
-               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 529>)
+               602 LOAD_CONST              42 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 541>)
                604 MAKE_FUNCTION            0
                606 PRECALL                  2
                610 CALL                     2
                620 POP_TOP
    
-   530         622 LOAD_NAME               26 (button)
+   542         622 LOAD_NAME               26 (button)
                624 LOAD_METHOD             28 (pack)
                646 LOAD_CONST              43 ('x')
                648 LOAD_CONST              44 (5)
                650 LOAD_CONST              44 (5)
                652 KW_NAMES                45
                654 PRECALL                  3
                658 CALL                     3
                668 POP_TOP
    
-   532         670 PUSH_NULL
+   544         670 PUSH_NULL
                672 LOAD_NAME               10 (AdwDrawRoundButton)
                674 LOAD_CONST              39 ('Hello')
                676 KW_NAMES                40
                678 PRECALL                  1
                682 CALL                     1
                692 STORE_NAME              29 (button4)
    
-   533         694 LOAD_NAME               29 (button4)
+   545         694 LOAD_NAME               29 (button4)
                696 LOAD_METHOD             27 (bind)
                718 LOAD_CONST              41 ('<<Click>>')
-               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 533>)
+               720 LOAD_CONST              46 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 545>)
                722 MAKE_FUNCTION            0
                724 PRECALL                  2
                728 CALL                     2
                738 POP_TOP
    
-   534         740 LOAD_NAME               29 (button4)
+   546         740 LOAD_NAME               29 (button4)
                742 LOAD_METHOD             28 (pack)
                764 LOAD_CONST              43 ('x')
                766 LOAD_CONST              44 (5)
                768 LOAD_CONST              44 (5)
                770 KW_NAMES                45
                772 PRECALL                  3
                776 CALL                     3
                786 POP_TOP
    
-   536         788 PUSH_NULL
+   548         788 PUSH_NULL
                790 LOAD_NAME               13 (AdwDrawRoundButton2)
                792 LOAD_CONST              39 ('Hello')
                794 KW_NAMES                40
                796 PRECALL                  1
                800 CALL                     1
                810 STORE_NAME              30 (button7)
    
-   537         812 LOAD_NAME               30 (button7)
+   549         812 LOAD_NAME               30 (button7)
                814 LOAD_METHOD             27 (bind)
                836 LOAD_CONST              41 ('<<Click>>')
-               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 537>)
+               838 LOAD_CONST              47 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 549>)
                840 MAKE_FUNCTION            0
                842 PRECALL                  2
                846 CALL                     2
                856 POP_TOP
    
-   538         858 LOAD_NAME               30 (button7)
+   550         858 LOAD_NAME               30 (button7)
                860 LOAD_METHOD             28 (pack)
                882 LOAD_CONST              43 ('x')
                884 LOAD_CONST              44 (5)
                886 LOAD_CONST              44 (5)
                888 KW_NAMES                45
                890 PRECALL                  3
                894 CALL                     3
                904 POP_TOP
    
-   540         906 PUSH_NULL
+   552         906 PUSH_NULL
                908 LOAD_NAME               16 (AdwDrawRoundButton3)
                910 LOAD_CONST              39 ('Hello')
                912 KW_NAMES                40
                914 PRECALL                  1
                918 CALL                     1
                928 STORE_NAME              31 (button10)
    
-   541         930 LOAD_NAME               31 (button10)
+   553         930 LOAD_NAME               31 (button10)
                932 LOAD_METHOD             27 (bind)
                954 LOAD_CONST              41 ('<<Click>>')
-               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 541>)
+               956 LOAD_CONST              48 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 553>)
                958 MAKE_FUNCTION            0
                960 PRECALL                  2
                964 CALL                     2
                974 POP_TOP
    
-   542         976 LOAD_NAME               31 (button10)
+   554         976 LOAD_NAME               31 (button10)
                978 LOAD_METHOD             28 (pack)
               1000 LOAD_CONST              43 ('x')
               1002 LOAD_CONST              44 (5)
               1004 LOAD_CONST              44 (5)
               1006 KW_NAMES                45
               1008 PRECALL                  3
               1012 CALL                     3
               1022 POP_TOP
    
-   544        1024 PUSH_NULL
+   556        1024 PUSH_NULL
               1026 LOAD_NAME               20 (AdwDrawCircularButton)
               1028 LOAD_CONST              39 ('Hello')
               1030 KW_NAMES                40
               1032 PRECALL                  1
               1036 CALL                     1
               1046 STORE_NAME              32 (button13)
    
-   545        1048 LOAD_NAME               32 (button13)
+   557        1048 LOAD_NAME               32 (button13)
               1050 LOAD_METHOD             27 (bind)
               1072 LOAD_CONST              41 ('<<Click>>')
-              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 545>)
+              1074 LOAD_CONST              49 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 557>)
               1076 MAKE_FUNCTION            0
               1078 PRECALL                  2
               1082 CALL                     2
               1092 POP_TOP
    
-   546        1094 LOAD_NAME               32 (button13)
+   558        1094 LOAD_NAME               32 (button13)
               1096 LOAD_METHOD             28 (pack)
               1118 LOAD_CONST              43 ('x')
               1120 LOAD_CONST              44 (5)
               1122 LOAD_CONST              44 (5)
               1124 KW_NAMES                45
               1126 PRECALL                  3
               1130 CALL                     3
               1140 POP_TOP
    
-   548        1142 LOAD_NAME               25 (root)
+   560        1142 LOAD_NAME               25 (root)
               1144 LOAD_METHOD             33 (mainloop)
               1166 PRECALL                  0
               1170 CALL                     0
               1180 POP_TOP
               1182 LOAD_CONST              50 (None)
               1184 RETURN_VALUE
    
-   523     >> 1186 LOAD_CONST              50 (None)
+   535     >> 1186 LOAD_CONST              50 (None)
               1188 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwWidget',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
-            0x8700970065005a0164005a02640164026403640464059c046406650366
-            02880066016407840e5a0488006601640884085a05640984005a06641464
-            0a84015a076414640b84015a086414640c84015a096414640d84015a0a64
-            14640e650b6602640f84055a0c641084005a0d641184005a0e641284005a
-            0f6414641384015a10880078015a115300
+            0x8700970065005a0164005a0264015a03640264036404640564069c0464
+            0765046602880066016408840e5a0588006601640984085a066417880066
+            01640b840c5a076418640c84015a086418640d84015a096418640e84015a
+            0a6418640f84015a0b6418641084015a0c64186411650d6602641284055a
+            0e641384005a0f641484005a10641584005a116418641684015a12880078
+            015a135300
                        0 MAKE_CELL                0 (__class__)
          
            6           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicButton')
                       10 STORE_NAME               2 (__qualname__)
          
-           7          12 LOAD_CONST               1 (120)
-                      14 LOAD_CONST               2 (40)
-                      16 LOAD_CONST               3 ('')
-                      18 LOAD_CONST               4 (None)
-                      20 LOAD_CONST               5 (('width', 'height', 'text', 'command'))
-                      22 BUILD_CONST_KEY_MAP      4
-                      24 LOAD_CONST               6 ('text')
-                      26 LOAD_NAME                3 (str)
-                      28 BUILD_TUPLE              2
-                      30 LOAD_CLOSURE             0 (__class__)
-                      32 BUILD_TUPLE              1
-                      34 LOAD_CONST               7 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 7>)
-                      36 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
-                      38 STORE_NAME               4 (__init__)
-         
-          33          40 LOAD_CLOSURE             0 (__class__)
-                      42 BUILD_TUPLE              1
-                      44 LOAD_CONST               8 (<code object configure, file "D:\tkadw\tkadw\windows\canvas\button.py", line 33>)
-                      46 MAKE_FUNCTION            8 (closure)
-                      48 STORE_NAME               5 (configure)
-         
-          43          50 LOAD_CONST               9 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 43>)
-                      52 MAKE_FUNCTION            0
-                      54 STORE_NAME               6 (_draw)
-         
-          62          56 LOAD_CONST              20 ((None,))
-                      58 LOAD_CONST              10 (<code object _click, file "D:\tkadw\tkadw\windows\canvas\button.py", line 62>)
-                      60 MAKE_FUNCTION            1 (defaults)
-                      62 STORE_NAME               7 (_click)
-         
-          73          64 LOAD_CONST              20 ((None,))
-                      66 LOAD_CONST              11 (<code object _unclick, file "D:\tkadw\tkadw\windows\canvas\button.py", line 73>)
-                      68 MAKE_FUNCTION            1 (defaults)
-                      70 STORE_NAME               8 (_unclick)
-         
-          84          72 LOAD_CONST              20 ((None,))
-                      74 LOAD_CONST              12 (<code object _hover, file "D:\tkadw\tkadw\windows\canvas\button.py", line 84>)
-                      76 MAKE_FUNCTION            1 (defaults)
-                      78 STORE_NAME               9 (_hover)
-         
-          93          80 LOAD_CONST              20 ((None,))
-                      82 LOAD_CONST              13 (<code object _hover_release, file "D:\tkadw\tkadw\windows\canvas\button.py", line 93>)
-                      84 MAKE_FUNCTION            1 (defaults)
-                      86 STORE_NAME              10 (_hover_release)
-         
-         102          88 LOAD_CONST              20 ((None,))
-                      90 LOAD_CONST              14 ('font')
-                      92 LOAD_NAME               11 (Font)
-                      94 BUILD_TUPLE              2
-                      96 LOAD_CONST              15 (<code object font, file "D:\tkadw\tkadw\windows\canvas\button.py", line 102>)
-                      98 MAKE_FUNCTION            5 (defaults, annotations)
-                     100 STORE_NAME              12 (font)
-         
-         108         102 LOAD_CONST              16 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 108>)
-                     104 MAKE_FUNCTION            0
-                     106 STORE_NAME              13 (default_palette)
-         
-         111         108 LOAD_CONST              17 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\button.py", line 111>)
-                     110 MAKE_FUNCTION            0
-                     112 STORE_NAME              14 (palette_light)
-         
-         137         114 LOAD_CONST              18 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\button.py", line 137>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              15 (palette_dark)
-         
-         163         120 LOAD_CONST              20 ((None,))
-                     122 LOAD_CONST              19 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 163>)
-                     124 MAKE_FUNCTION            1 (defaults)
-                     126 STORE_NAME              16 (palette)
-                     128 LOAD_CLOSURE             0 (__class__)
-                     130 COPY                     1
-                     132 STORE_NAME              17 (__classcell__)
-                     134 RETURN_VALUE
+           8          12 LOAD_CONST               1 ('\n    自绘基础按钮\n    ')
+                      14 STORE_NAME               3 (__doc__)
+         
+          12          16 LOAD_CONST               2 (120)
+                      18 LOAD_CONST               3 (40)
+                      20 LOAD_CONST               4 ('')
+                      22 LOAD_CONST               5 (None)
+                      24 LOAD_CONST               6 (('width', 'height', 'text', 'command'))
+                      26 BUILD_CONST_KEY_MAP      4
+                      28 LOAD_CONST               7 ('text')
+                      30 LOAD_NAME                4 (str)
+                      32 BUILD_TUPLE              2
+                      34 LOAD_CLOSURE             0 (__class__)
+                      36 BUILD_TUPLE              1
+                      38 LOAD_CONST               8 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 12>)
+                      40 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
+                      42 STORE_NAME               5 (__init__)
+         
+          38          44 LOAD_CLOSURE             0 (__class__)
+                      46 BUILD_TUPLE              1
+                      48 LOAD_CONST               9 (<code object configure, file "D:\tkadw\tkadw\windows\canvas\button.py", line 38>)
+                      50 MAKE_FUNCTION            8 (closure)
+                      52 STORE_NAME               6 (configure)
+         
+          48          54 LOAD_CONST              23 (('return', None))
+                      56 LOAD_CLOSURE             0 (__class__)
+                      58 BUILD_TUPLE              1
+                      60 LOAD_CONST              11 (<code object update, file "D:\tkadw\tkadw\windows\canvas\button.py", line 48>)
+                      62 MAKE_FUNCTION           12 (annotations, closure)
+                      64 STORE_NAME               7 (update)
+         
+          55          66 LOAD_CONST              24 ((None,))
+                      68 LOAD_CONST              12 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 55>)
+                      70 MAKE_FUNCTION            1 (defaults)
+                      72 STORE_NAME               8 (_draw)
+         
+          74          74 LOAD_CONST              24 ((None,))
+                      76 LOAD_CONST              13 (<code object _click, file "D:\tkadw\tkadw\windows\canvas\button.py", line 74>)
+                      78 MAKE_FUNCTION            1 (defaults)
+                      80 STORE_NAME               9 (_click)
+         
+          85          82 LOAD_CONST              24 ((None,))
+                      84 LOAD_CONST              14 (<code object _unclick, file "D:\tkadw\tkadw\windows\canvas\button.py", line 85>)
+                      86 MAKE_FUNCTION            1 (defaults)
+                      88 STORE_NAME              10 (_unclick)
+         
+          96          90 LOAD_CONST              24 ((None,))
+                      92 LOAD_CONST              15 (<code object _hover, file "D:\tkadw\tkadw\windows\canvas\button.py", line 96>)
+                      94 MAKE_FUNCTION            1 (defaults)
+                      96 STORE_NAME              11 (_hover)
+         
+         105          98 LOAD_CONST              24 ((None,))
+                     100 LOAD_CONST              16 (<code object _hover_release, file "D:\tkadw\tkadw\windows\canvas\button.py", line 105>)
+                     102 MAKE_FUNCTION            1 (defaults)
+                     104 STORE_NAME              12 (_hover_release)
+         
+         114         106 LOAD_CONST              24 ((None,))
+                     108 LOAD_CONST              17 ('font')
+                     110 LOAD_NAME               13 (Font)
+                     112 BUILD_TUPLE              2
+                     114 LOAD_CONST              18 (<code object font, file "D:\tkadw\tkadw\windows\canvas\button.py", line 114>)
+                     116 MAKE_FUNCTION            5 (defaults, annotations)
+                     118 STORE_NAME              14 (font)
+         
+         120         120 LOAD_CONST              19 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 120>)
+                     122 MAKE_FUNCTION            0
+                     124 STORE_NAME              15 (default_palette)
+         
+         123         126 LOAD_CONST              20 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\button.py", line 123>)
+                     128 MAKE_FUNCTION            0
+                     130 STORE_NAME              16 (palette_light)
+         
+         149         132 LOAD_CONST              21 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\button.py", line 149>)
+                     134 MAKE_FUNCTION            0
+                     136 STORE_NAME              17 (palette_dark)
+         
+         175         138 LOAD_CONST              24 ((None,))
+                     140 LOAD_CONST              22 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 175>)
+                     142 MAKE_FUNCTION            1 (defaults)
+                     144 STORE_NAME              18 (palette)
+                     146 LOAD_CLOSURE             0 (__class__)
+                     148 COPY                     1
+                     150 STORE_NAME              19 (__classcell__)
+                     152 RETURN_VALUE
          consts
             'AdwDrawBasicButton'
+            '\n    自绘基础按钮\n    '
             120
             40
             ''
             None
             ('width', 'height', 'text', 'command')
             'text'
             code
@@ -528,17 +541,17 @@
                   000000000000000100890481197c00a00e00000000000000000000000000
                   00000000000000640a88046601640b8408a6020000ab0200000000000000
                   0001007c00a01300000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                4 (command)
                
-                 7           4 RESUME                   0
+                12           4 RESUME                   0
                
-                 8           6 PUSH_NULL
+                13           6 PUSH_NULL
                              8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_ATTR                1 (__init__)
                             44 LOAD_FAST                5 (args)
                             46 LOAD_FAST                1 (width)
                             48 LOAD_FAST                2 (height)
@@ -547,110 +560,110 @@
                             54 LOAD_CONST               2 (('width', 'height', 'bd', 'highlightthickness'))
                             56 BUILD_CONST_KEY_MAP      4
                             58 LOAD_FAST                6 (kwargs)
                             60 DICT_MERGE               1
                             62 CALL_FUNCTION_EX         1
                             64 POP_TOP
                
-                10          66 LOAD_FAST                0 (self)
+                15          66 LOAD_FAST                0 (self)
                             68 LOAD_METHOD              2 (default_palette)
                             90 PRECALL                  0
                             94 CALL                     0
                            104 POP_TOP
                
-                12         106 LOAD_FAST                3 (text)
+                17         106 LOAD_FAST                3 (text)
                            108 LOAD_FAST                0 (self)
                            110 STORE_ATTR               3 (text)
                
-                14         120 LOAD_FAST                0 (self)
+                19         120 LOAD_FAST                0 (self)
                            122 LOAD_ATTR                4 (button_back)
                            132 LOAD_FAST                0 (self)
                            134 STORE_ATTR               5 (_button_back)
                
-                15         144 LOAD_FAST                0 (self)
+                20         144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                6 (button_border)
                            156 LOAD_FAST                0 (self)
                            158 STORE_ATTR               7 (_button_border)
                
-                16         168 LOAD_FAST                0 (self)
+                21         168 LOAD_FAST                0 (self)
                            170 LOAD_ATTR                8 (button_border_width)
                            180 LOAD_FAST                0 (self)
                            182 STORE_ATTR               9 (_button_border_width)
                
-                17         192 LOAD_FAST                0 (self)
+                22         192 LOAD_FAST                0 (self)
                            194 LOAD_ATTR               10 (button_text_back)
                            204 LOAD_FAST                0 (self)
                            206 STORE_ATTR              11 (_button_text_back)
                
-                19         216 LOAD_GLOBAL             25 (NULL + nametofont)
+                24         216 LOAD_GLOBAL             25 (NULL + nametofont)
                            228 LOAD_CONST               3 ('TkDefaultFont')
                            230 PRECALL                  1
                            234 CALL                     1
                            244 LOAD_FAST                0 (self)
                            246 STORE_ATTR              13 (button_text_font)
                
-                22         256 LOAD_FAST                0 (self)
+                27         256 LOAD_FAST                0 (self)
                            258 LOAD_METHOD             14 (bind)
                            280 LOAD_CONST               4 ('<Button>')
                            282 LOAD_FAST                0 (self)
                            284 LOAD_ATTR               15 (_click)
                            294 LOAD_CONST               5 ('+')
                            296 KW_NAMES                 6
                            298 PRECALL                  3
                            302 CALL                     3
                            312 POP_TOP
                
-                23         314 LOAD_FAST                0 (self)
+                28         314 LOAD_FAST                0 (self)
                            316 LOAD_METHOD             14 (bind)
                            338 LOAD_CONST               7 ('<ButtonRelease>')
                            340 LOAD_FAST                0 (self)
                            342 LOAD_ATTR               16 (_unclick)
                            352 LOAD_CONST               5 ('+')
                            354 KW_NAMES                 6
                            356 PRECALL                  3
                            360 CALL                     3
                            370 POP_TOP
                
-                24         372 LOAD_FAST                0 (self)
+                29         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (bind)
                            396 LOAD_CONST               8 ('<Enter>')
                            398 LOAD_FAST                0 (self)
                            400 LOAD_ATTR               17 (_hover)
                            410 LOAD_CONST               5 ('+')
                            412 KW_NAMES                 6
                            414 PRECALL                  3
                            418 CALL                     3
                            428 POP_TOP
                
-                25         430 LOAD_FAST                0 (self)
+                30         430 LOAD_FAST                0 (self)
                            432 LOAD_METHOD             14 (bind)
                            454 LOAD_CONST               9 ('<Leave>')
                            456 LOAD_FAST                0 (self)
                            458 LOAD_ATTR               18 (_hover_release)
                            468 LOAD_CONST               5 ('+')
                            470 KW_NAMES                 6
                            472 PRECALL                  3
                            476 CALL                     3
                            486 POP_TOP
                
-                28         488 LOAD_DEREF               4 (command)
+                33         488 LOAD_DEREF               4 (command)
                            490 POP_JUMP_FORWARD_IF_NONE    25 (to 542)
                
-                29         492 LOAD_FAST                0 (self)
+                34         492 LOAD_FAST                0 (self)
                            494 LOAD_METHOD             14 (bind)
                            516 LOAD_CONST              10 ('<<Click>>')
                            518 LOAD_CLOSURE             4 (command)
                            520 BUILD_TUPLE              1
-                           522 LOAD_CONST              11 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 29>)
+                           522 LOAD_CONST              11 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 34>)
                            524 MAKE_FUNCTION            8 (closure)
                            526 PRECALL                  2
                            530 CALL                     2
                            540 POP_TOP
                
-                31     >>  542 LOAD_FAST                0 (self)
+                36     >>  542 LOAD_FAST                0 (self)
                            544 LOAD_METHOD             19 (_draw)
                            566 LOAD_CONST               0 (None)
                            568 PRECALL                  1
                            572 CALL                     1
                            582 POP_TOP
                            584 LOAD_CONST               0 (None)
                            586 RETURN_VALUE
@@ -670,37 +683,37 @@
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code 0x9501970002008901a6000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      29           2 RESUME                   0
+                      34           2 RESUME                   0
                                    4 PUSH_NULL
                                    6 LOAD_DEREF               1 (command)
                                    8 PRECALL                  0
                                   12 CALL                     0
                                   22 RETURN_VALUE
                      consts
                         None
                      names      ()
                      varnames   ('event',)
                      freevars   ('command',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                      name       '<lambda>'
-                     firstlineno 29
+                     firstlineno 34
                      lnotab 0x
                names      ('super', '__init__', 'default_palette', 'text', 'button_back', '_button_back', 'button_border', '_button_border', 'button_border_width', '_button_border_width', 'button_text_back', '_button_text_back', 'nametofont', 'button_text_font', 'bind', '_click', '_unclick', '_hover', '_hover_release', '_draw')
                varnames   ('self', 'width', 'height', 'text', 'command', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('command',)
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '__init__'
-               firstlineno 7
+               firstlineno 12
                lnotab
                   0x06013c0228020e02180118011801180228033a013a013a013a03040132
                   02
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
@@ -715,65 +728,65 @@
                   008900a00400000000000000000000000000000000000000006400a60100
                   00ab0100000000000000000100640053000200740b000000000000000000
                   00a6000000ab0000000000000000006a060000000000000000640569007c
                   01a4018e01010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
-                33           4 RESUME                   0
+                38           4 RESUME                   0
                
-                34           6 LOAD_CONST               1 ('command')
+                39           6 LOAD_CONST               1 ('command')
                              8 LOAD_FAST                1 (kwargs)
                             10 CONTAINS_OP              0
                             12 POP_JUMP_FORWARD_IF_FALSE    53 (to 120)
                
-                35          14 LOAD_FAST                1 (kwargs)
+                40          14 LOAD_FAST                1 (kwargs)
                             16 LOAD_METHOD              0 (pop)
                             38 LOAD_CONST               1 ('command')
                             40 PRECALL                  1
                             44 CALL                     1
                             54 LOAD_DEREF               0 (self)
                             56 STORE_ATTR               1 (command)
                
-                36          66 LOAD_DEREF               0 (self)
+                41          66 LOAD_DEREF               0 (self)
                             68 LOAD_METHOD              2 (bind)
                             90 LOAD_CONST               2 ('<<Click>>')
                             92 LOAD_CLOSURE             0 (self)
                             94 BUILD_TUPLE              1
-                            96 LOAD_CONST               3 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 36>)
+                            96 LOAD_CONST               3 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\button.py", line 41>)
                             98 MAKE_FUNCTION            8 (closure)
                            100 PRECALL                  2
                            104 CALL                     2
                            114 POP_TOP
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-                37     >>  120 LOAD_CONST               4 ('text')
+                42     >>  120 LOAD_CONST               4 ('text')
                            122 LOAD_FAST                1 (kwargs)
                            124 CONTAINS_OP              0
                            126 POP_JUMP_FORWARD_IF_FALSE    49 (to 226)
                
-                38         128 LOAD_FAST                1 (kwargs)
+                43         128 LOAD_FAST                1 (kwargs)
                            130 LOAD_METHOD              0 (pop)
                            152 LOAD_CONST               4 ('text')
                            154 PRECALL                  1
                            158 CALL                     1
                            168 LOAD_DEREF               0 (self)
                            170 STORE_ATTR               3 (text)
                
-                39         180 LOAD_DEREF               0 (self)
+                44         180 LOAD_DEREF               0 (self)
                            182 LOAD_METHOD              4 (_draw)
                            204 LOAD_CONST               0 (None)
                            206 PRECALL                  1
                            210 CALL                     1
                            220 POP_TOP
                            222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                
-                41     >>  226 PUSH_NULL
+                46     >>  226 PUSH_NULL
                            228 LOAD_GLOBAL             11 (NULL + super)
                            240 PRECALL                  0
                            244 CALL                     0
                            254 LOAD_ATTR                6 (configure)
                            264 LOAD_CONST               5 (())
                            266 BUILD_MAP                0
                            268 LOAD_FAST                1 (kwargs)
@@ -792,40 +805,82 @@
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      36           2 RESUME                   0
+                      41           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (command)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('command',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                      name       '<lambda>'
-                     firstlineno 36
+                     firstlineno 41
                      lnotab 0x
                   'text'
                   ()
                names      ('pop', 'command', 'bind', 'text', '_draw', 'super', 'configure')
                varnames   ('self', 'kwargs')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'configure'
-               firstlineno 33
+               firstlineno 38
                lnotab 0x0601080134013601080134012e02
+            'return'
+            code
+               argcount  : 1
+               nlocals   : 1
+               stacksize : 3
+               flags     : 3
+               code
+                  0x95019700740100000000000000000000a6000000ab0000000000000000
+                  00a0010000000000000000000000000000000000000000a6000000ab0000
+                  0000000000000001007c00a0020000000000000000000000000000000000
+                  0000006401a6010000ab010000000000000000010064015300
+                             0 COPY_FREE_VARS           1
+               
+                48           2 RESUME                   0
+               
+                52           4 LOAD_GLOBAL              1 (NULL + super)
+                            16 PRECALL                  0
+                            20 CALL                     0
+                            30 LOAD_METHOD              1 (update)
+                            52 PRECALL                  0
+                            56 CALL                     0
+                            66 POP_TOP
+               
+                53          68 LOAD_FAST                0 (self)
+                            70 LOAD_METHOD              2 (_draw)
+                            92 LOAD_CONST               1 (None)
+                            94 PRECALL                  1
+                            98 CALL                     1
+                           108 POP_TOP
+                           110 LOAD_CONST               1 (None)
+                           112 RETURN_VALUE
+               consts
+                  '\n        多执行一道绘制\n        '
+                  None
+               names      ('super', 'update', '_draw')
+               varnames   ('self',)
+               freevars   ('__class__',)
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
+               name       'update'
+               firstlineno 48
+               lnotab 0x04044001
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000006401a6
@@ -840,94 +895,94 @@
                   000000000000007c005f0700000000000000007c00a00800000000000000
                   000000000000000000000000007c00a00300000000000000000000000000
                   00000000000000a6000000ab00000000000000000064047a0b00007c00a0
                   040000000000000000000000000000000000000000a6000000ab00000000
                   000000000064047a0b00007c006a0900000000000000007c006a0a000000
                   00000000007c006a0b0000000000000000ac05a6050000ab050000000000
                   0000007c005f0c000000000000000064005300
-                43           0 RESUME                   0
+                55           0 RESUME                   0
                
-                44           2 LOAD_FAST                0 (self)
+                56           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-                47          44 LOAD_FAST                0 (self)
+                59          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-                48          68 LOAD_FAST                0 (self)
+                60          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (_button_border_width)
                             80 LOAD_CONST               2 (1)
                             82 BINARY_OP               10 (-)
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (_button_border_width)
                             98 LOAD_CONST               2 (1)
                            100 BINARY_OP               10 (-)
                
-                49         104 LOAD_FAST                0 (self)
+                61         104 LOAD_FAST                0 (self)
                            106 LOAD_METHOD              3 (winfo_width)
                            128 PRECALL                  0
                            132 CALL                     0
                            142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (_button_border_width)
                            154 BINARY_OP               10 (-)
                            158 LOAD_CONST               2 (1)
                            160 BINARY_OP                0 (+)
                
-                50         164 LOAD_FAST                0 (self)
+                62         164 LOAD_FAST                0 (self)
                            166 LOAD_METHOD              4 (winfo_height)
                            188 PRECALL                  0
                            192 CALL                     0
                            202 LOAD_FAST                0 (self)
                            204 LOAD_ATTR                2 (_button_border_width)
                            214 BINARY_OP               10 (-)
                            218 LOAD_CONST               2 (1)
                            220 BINARY_OP                0 (+)
                
-                51         224 LOAD_FAST                0 (self)
+                63         224 LOAD_FAST                0 (self)
                            226 LOAD_ATTR                2 (_button_border_width)
                
-                52         236 LOAD_FAST                0 (self)
+                64         236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                5 (_button_border)
                            248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                6 (_button_back)
                
-                47         260 KW_NAMES                 3
+                59         260 KW_NAMES                 3
                            262 PRECALL                  7
                            266 CALL                     7
                            276 LOAD_FAST                0 (self)
                            278 STORE_ATTR               7 (button_frame)
                
-                56         288 LOAD_FAST                0 (self)
+                68         288 LOAD_FAST                0 (self)
                            290 LOAD_METHOD              8 (create_text)
                
-                57         312 LOAD_FAST                0 (self)
+                69         312 LOAD_FAST                0 (self)
                            314 LOAD_METHOD              3 (winfo_width)
                            336 PRECALL                  0
                            340 CALL                     0
                            350 LOAD_CONST               4 (2)
                            352 BINARY_OP               11 (/)
                            356 LOAD_FAST                0 (self)
                            358 LOAD_METHOD              4 (winfo_height)
                            380 PRECALL                  0
                            384 CALL                     0
                            394 LOAD_CONST               4 (2)
                            396 BINARY_OP               11 (/)
                
-                58         400 LOAD_FAST                0 (self)
+                70         400 LOAD_FAST                0 (self)
                            402 LOAD_ATTR                9 (text)
                            412 LOAD_FAST                0 (self)
                            414 LOAD_ATTR               10 (_button_text_back)
                
-                59         424 LOAD_FAST                0 (self)
+                71         424 LOAD_FAST                0 (self)
                            426 LOAD_ATTR               11 (button_text_font)
                
-                56         436 KW_NAMES                 5
+                68         436 KW_NAMES                 5
                            438 PRECALL                  5
                            442 CALL                     5
                            452 LOAD_FAST                0 (self)
                            454 STORE_ATTR              12 (button_text)
                            464 LOAD_CONST               0 (None)
                            466 RETURN_VALUE
                consts
@@ -939,62 +994,62 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_rectangle', '_button_border_width', 'winfo_width', 'winfo_height', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
-               firstlineno 43
+               firstlineno 55
                lnotab 0x02012a03180124013c013c010c0118fb1c091801580118010cfd
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   006a0700000000000000007c005f0800000000000000007c00a009000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0001007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-                62           0 RESUME                   0
+                74           0 RESUME                   0
                
-                63           2 LOAD_CONST               1 (True)
+                75           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                64          16 LOAD_FAST                0 (self)
+                76          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_pressed_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                65          40 LOAD_FAST                0 (self)
+                77          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_pressed_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                66          64 LOAD_FAST                0 (self)
+                78          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_pressed_border_width)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_border_width)
                
-                67          88 LOAD_FAST                0 (self)
+                79          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                7 (button_pressed_text_back)
                            100 LOAD_FAST                0 (self)
                            102 STORE_ATTR               8 (_button_text_back)
                
-                69         112 LOAD_FAST                0 (self)
+                81         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              9 (focus_set)
                            136 PRECALL                  0
                            140 CALL                     0
                            150 POP_TOP
                
-                71         152 LOAD_FAST                0 (self)
+                83         152 LOAD_FAST                0 (self)
                            154 LOAD_METHOD             10 (_draw)
                            176 LOAD_CONST               0 (None)
                            178 PRECALL                  1
                            182 CALL                     1
                            192 POP_TOP
                            194 LOAD_CONST               0 (None)
                            196 RETURN_VALUE
@@ -1003,123 +1058,123 @@
                   True
                names      ('hover', 'button_pressed_back', '_button_back', 'button_pressed_border', '_button_border', 'button_pressed_border_width', '_button_border_width', 'button_pressed_text_back', '_button_text_back', 'focus_set', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_click'
-               firstlineno 62
+               firstlineno 74
                lnotab 0x02010e0118011801180118022802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000725c7c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   006a0700000000000000007c005f0800000000000000007c00a009000000
                   00000000000000000000000000000000006400a6010000ab010000000000
                   00000001007c00a00a000000000000000000000000000000000000000064
                   01a6010000ab01000000000000000001006400530064005300
-                73           0 RESUME                   0
+                85           0 RESUME                   0
                
-                74           2 LOAD_FAST                0 (self)
+                86           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (hover)
                             14 POP_JUMP_FORWARD_IF_FALSE    92 (to 200)
                
-                75          16 LOAD_FAST                0 (self)
+                87          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                76          40 LOAD_FAST                0 (self)
+                88          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                77          64 LOAD_FAST                0 (self)
+                89          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_active_border_width)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_border_width)
                
-                78          88 LOAD_FAST                0 (self)
+                90          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                7 (button_active_text_back)
                            100 LOAD_FAST                0 (self)
                            102 STORE_ATTR               8 (_button_text_back)
                
-                80         112 LOAD_FAST                0 (self)
+                92         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              9 (_draw)
                            136 LOAD_CONST               0 (None)
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                
-                82         154 LOAD_FAST                0 (self)
+                94         154 LOAD_FAST                0 (self)
                            156 LOAD_METHOD             10 (event_generate)
                            178 LOAD_CONST               1 ('<<Click>>')
                            180 PRECALL                  1
                            184 CALL                     1
                            194 POP_TOP
                            196 LOAD_CONST               0 (None)
                            198 RETURN_VALUE
                
-                74     >>  200 LOAD_CONST               0 (None)
+                86     >>  200 LOAD_CONST               0 (None)
                            202 RETURN_VALUE
                consts
                   None
                   '<<Click>>'
                names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_border_width', '_button_border_width', 'button_active_text_back', '_button_text_back', '_draw', 'event_generate')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_unclick'
-               firstlineno 73
+               firstlineno 85
                lnotab 0x02010e0118011801180118022a022ef8
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   006a0700000000000000007c005f0800000000000000007c00a009000000
                   00000000000000000000000000000000006400a6010000ab010000000000
                   000000010064005300
-                84           0 RESUME                   0
+                96           0 RESUME                   0
                
-                85           2 LOAD_CONST               1 (True)
+                97           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                86          16 LOAD_FAST                0 (self)
+                98          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_active_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                87          40 LOAD_FAST                0 (self)
+                99          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_active_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                88          64 LOAD_FAST                0 (self)
+               100          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_active_border_width)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_border_width)
                
-                89          88 LOAD_FAST                0 (self)
+               101          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                7 (button_active_text_back)
                            100 LOAD_FAST                0 (self)
                            102 STORE_ATTR               8 (_button_text_back)
                
-                91         112 LOAD_FAST                0 (self)
+               103         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              9 (_draw)
                            136 LOAD_CONST               0 (None)
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                            154 LOAD_CONST               0 (None)
                            156 RETURN_VALUE
@@ -1128,55 +1183,55 @@
                   True
                names      ('hover', 'button_active_back', '_button_back', 'button_active_border', '_button_border', 'button_active_border_width', '_button_border_width', 'button_active_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_hover'
-               firstlineno 84
+               firstlineno 96
                lnotab 0x02010e011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x970064017c005f0000000000000000007c006a0100000000000000007c
                   005f0200000000000000007c006a0300000000000000007c005f04000000
                   00000000007c006a0500000000000000007c005f0600000000000000007c
                   006a0700000000000000007c005f0800000000000000007c00a009000000
                   00000000000000000000000000000000006400a6010000ab010000000000
                   000000010064005300
-                93           0 RESUME                   0
+               105           0 RESUME                   0
                
-                94           2 LOAD_CONST               1 (False)
+               106           2 LOAD_CONST               1 (False)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                
-                95          16 LOAD_FAST                0 (self)
+               107          16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (button_back)
                             28 LOAD_FAST                0 (self)
                             30 STORE_ATTR               2 (_button_back)
                
-                96          40 LOAD_FAST                0 (self)
+               108          40 LOAD_FAST                0 (self)
                             42 LOAD_ATTR                3 (button_border)
                             52 LOAD_FAST                0 (self)
                             54 STORE_ATTR               4 (_button_border)
                
-                97          64 LOAD_FAST                0 (self)
+               109          64 LOAD_FAST                0 (self)
                             66 LOAD_ATTR                5 (button_border_width)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               6 (_button_border_width)
                
-                98          88 LOAD_FAST                0 (self)
+               110          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                7 (button_text_back)
                            100 LOAD_FAST                0 (self)
                            102 STORE_ATTR               8 (_button_text_back)
                
-               100         112 LOAD_FAST                0 (self)
+               112         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              9 (_draw)
                            136 LOAD_CONST               0 (None)
                            138 PRECALL                  1
                            142 CALL                     1
                            152 POP_TOP
                            154 LOAD_CONST               0 (None)
                            156 RETURN_VALUE
@@ -1185,128 +1240,128 @@
                   False
                names      ('hover', 'button_back', '_button_back', 'button_border', '_button_border', 'button_border_width', '_button_border_width', 'button_text_back', '_button_text_back', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_hover_release'
-               firstlineno 93
+               firstlineno 105
                lnotab 0x02010e011801180118011802
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               102           0 RESUME                   0
+               114           0 RESUME                   0
                
-               103           2 LOAD_FAST                1 (font)
+               115           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               104           6 LOAD_FAST                0 (self)
+               116           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_text_font)
                             18 RETURN_VALUE
                
-               106     >>   20 LOAD_FAST                1 (font)
+               118     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'font'
-               firstlineno 102
+               firstlineno 114
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               108           0 RESUME                   0
+               120           0 RESUME                   0
                
-               109           2 LOAD_FAST                0 (self)
+               121           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 108
+               firstlineno 120
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664076408640564099c046406640a640b640564099c
                   04640c9c066901a6010000ab010000000000000000010064005300
-               111           0 RESUME                   0
+               123           0 RESUME                   0
                
-               112           2 LOAD_FAST                0 (self)
+               124           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               114          26 LOAD_CONST               1 ('button')
+               126          26 LOAD_CONST               1 ('button')
                
-               115          28 LOAD_CONST               2 ('#fdfdfd')
+               127          28 LOAD_CONST               2 ('#fdfdfd')
                
-               116          30 LOAD_CONST               3 ('#eaeaea')
+               128          30 LOAD_CONST               3 ('#eaeaea')
                
-               117          32 LOAD_CONST               4 ('#1a1a1a')
+               129          32 LOAD_CONST               4 ('#1a1a1a')
                
-               118          34 LOAD_CONST               5 (1)
+               130          34 LOAD_CONST               5 (1)
                
-               121          36 LOAD_CONST               6 ('#f9f9f9')
+               133          36 LOAD_CONST               6 ('#f9f9f9')
                
-               122          38 LOAD_CONST               7 ('#aaaaaa')
+               134          38 LOAD_CONST               7 ('#aaaaaa')
                
-               123          40 LOAD_CONST               8 ('#5f5f5f')
+               135          40 LOAD_CONST               8 ('#5f5f5f')
                
-               124          42 LOAD_CONST               5 (1)
+               136          42 LOAD_CONST               5 (1)
                
-               120          44 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+               132          44 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
                             46 BUILD_CONST_KEY_MAP      4
                
-               128          48 LOAD_CONST               6 ('#f9f9f9')
+               140          48 LOAD_CONST               6 ('#f9f9f9')
                
-               129          50 LOAD_CONST              10 ('#e2e2e2')
+               141          50 LOAD_CONST              10 ('#e2e2e2')
                
-               130          52 LOAD_CONST              11 ('#8a8a8a')
+               142          52 LOAD_CONST              11 ('#8a8a8a')
                
-               131          54 LOAD_CONST               5 (1)
+               143          54 LOAD_CONST               5 (1)
                
-               127          56 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+               139          56 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
                             58 BUILD_CONST_KEY_MAP      4
                
-               114          60 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               126          60 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             62 BUILD_CONST_KEY_MAP      6
                
-               113          64 BUILD_MAP                1
+               125          64 BUILD_MAP                1
                
-               112          66 PRECALL                  1
+               124          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'button'
@@ -1323,70 +1378,70 @@
                   ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 111
+               firstlineno 123
                lnotab
                   0x020118020201020102010201020302010201020102fc04080201020102
                   0102fc04f304ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664036407640564089c0464096403640a640564089c
                   04640b9c066901a6010000ab010000000000000000010064005300
-               137           0 RESUME                   0
+               149           0 RESUME                   0
                
-               138           2 LOAD_FAST                0 (self)
+               150           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               140          26 LOAD_CONST               1 ('button')
+               152          26 LOAD_CONST               1 ('button')
                
-               141          28 LOAD_CONST               2 ('#353535')
+               153          28 LOAD_CONST               2 ('#353535')
                
-               142          30 LOAD_CONST               3 ('#454545')
+               154          30 LOAD_CONST               3 ('#454545')
                
-               143          32 LOAD_CONST               4 ('#ffffff')
+               155          32 LOAD_CONST               4 ('#ffffff')
                
-               144          34 LOAD_CONST               5 (1)
+               156          34 LOAD_CONST               5 (1)
                
-               147          36 LOAD_CONST               6 ('#3a3a3a')
+               159          36 LOAD_CONST               6 ('#3a3a3a')
                
-               148          38 LOAD_CONST               3 ('#454545')
+               160          38 LOAD_CONST               3 ('#454545')
                
-               149          40 LOAD_CONST               7 ('#cecece')
+               161          40 LOAD_CONST               7 ('#cecece')
                
-               150          42 LOAD_CONST               5 (1)
+               162          42 LOAD_CONST               5 (1)
                
-               146          44 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               158          44 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             46 BUILD_CONST_KEY_MAP      4
                
-               154          48 LOAD_CONST               9 ('#2f2f2f')
+               166          48 LOAD_CONST               9 ('#2f2f2f')
                
-               155          50 LOAD_CONST               3 ('#454545')
+               167          50 LOAD_CONST               3 ('#454545')
                
-               156          52 LOAD_CONST              10 ('#9a9a9a')
+               168          52 LOAD_CONST              10 ('#9a9a9a')
                
-               157          54 LOAD_CONST               5 (1)
+               169          54 LOAD_CONST               5 (1)
                
-               153          56 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               165          56 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             58 BUILD_CONST_KEY_MAP      4
                
-               140          60 LOAD_CONST              11 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               152          60 LOAD_CONST              11 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             62 BUILD_CONST_KEY_MAP      6
                
-               139          64 BUILD_MAP                1
+               151          64 BUILD_MAP                1
                
-               138          66 PRECALL                  1
+               150          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'button'
@@ -1402,15 +1457,15 @@
                   ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 137
+               firstlineno 149
                lnotab
                   0x020118020201020102010201020302010201020102fc04080201020102
                   0102fc04f304ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -1440,203 +1495,203 @@
                   000000000000007c005f0d00000000000000007c006a0100000000000000
                   007c005f0e00000000000000007c006a0300000000000000007c005f0f00
                   000000000000007c006a0200000000000000007c005f1000000000000000
                   0009007c00a01100000000000000000000000000000000000000006400a6
                   010000ab0100000000000000000100640053002300742400000000000000
                   00000024007204010059006400530077007803590077017c006a0c000000
                   00000000005300
-               163           0 RESUME                   0
+               175           0 RESUME                   0
                
-               164           2 LOAD_FAST                1 (dict)
+               176           2 LOAD_FAST                1 (dict)
                              4 EXTENDED_ARG             1
                              6 POP_JUMP_FORWARD_IF_NONE   397 (to 802)
                
-               165           8 LOAD_CONST               1 ('button')
+               177           8 LOAD_CONST               1 ('button')
                             10 LOAD_FAST                1 (dict)
                             12 CONTAINS_OP              0
                             14 EXTENDED_ARG             1
                             16 POP_JUMP_FORWARD_IF_FALSE   296 (to 610)
                
-               166          18 LOAD_FAST                1 (dict)
+               178          18 LOAD_FAST                1 (dict)
                             20 LOAD_CONST               1 ('button')
                             22 BINARY_SUBSCR
                             32 LOAD_CONST               2 ('back')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               0 (button_back)
                
-               167          56 LOAD_FAST                1 (dict)
+               179          56 LOAD_FAST                1 (dict)
                             58 LOAD_CONST               1 ('button')
                             60 BINARY_SUBSCR
                             70 LOAD_CONST               3 ('border')
                             72 BINARY_SUBSCR
                             82 LOAD_FAST                0 (self)
                             84 STORE_ATTR               1 (button_border)
                
-               168          94 LOAD_FAST                1 (dict)
+               180          94 LOAD_FAST                1 (dict)
                             96 LOAD_CONST               1 ('button')
                             98 BINARY_SUBSCR
                            108 LOAD_CONST               4 ('text_back')
                            110 BINARY_SUBSCR
                            120 LOAD_FAST                0 (self)
                            122 STORE_ATTR               2 (button_text_back)
                
-               169         132 LOAD_FAST                1 (dict)
+               181         132 LOAD_FAST                1 (dict)
                            134 LOAD_CONST               1 ('button')
                            136 BINARY_SUBSCR
                            146 LOAD_CONST               5 ('border_width')
                            148 BINARY_SUBSCR
                            158 LOAD_FAST                0 (self)
                            160 STORE_ATTR               3 (button_border_width)
                
-               171         170 LOAD_CONST               6 ('active')
+               183         170 LOAD_CONST               6 ('active')
                            172 LOAD_FAST                1 (dict)
                            174 LOAD_CONST               1 ('button')
                            176 BINARY_SUBSCR
                            186 CONTAINS_OP              0
                            188 POP_JUMP_FORWARD_IF_FALSE   100 (to 390)
                
-               172         190 LOAD_FAST                1 (dict)
+               184         190 LOAD_FAST                1 (dict)
                            192 LOAD_CONST               1 ('button')
                            194 BINARY_SUBSCR
                            204 LOAD_CONST               6 ('active')
                            206 BINARY_SUBSCR
                            216 LOAD_CONST               2 ('back')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               4 (button_active_back)
                
-               173         240 LOAD_FAST                1 (dict)
+               185         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST               1 ('button')
                            244 BINARY_SUBSCR
                            254 LOAD_CONST               6 ('active')
                            256 BINARY_SUBSCR
                            266 LOAD_CONST               3 ('border')
                            268 BINARY_SUBSCR
                            278 LOAD_FAST                0 (self)
                            280 STORE_ATTR               5 (button_active_border)
                
-               174         290 LOAD_FAST                1 (dict)
+               186         290 LOAD_FAST                1 (dict)
                            292 LOAD_CONST               1 ('button')
                            294 BINARY_SUBSCR
                            304 LOAD_CONST               6 ('active')
                            306 BINARY_SUBSCR
                            316 LOAD_CONST               4 ('text_back')
                            318 BINARY_SUBSCR
                            328 LOAD_FAST                0 (self)
                            330 STORE_ATTR               6 (button_active_text_back)
                
-               175         340 LOAD_FAST                1 (dict)
+               187         340 LOAD_FAST                1 (dict)
                            342 LOAD_CONST               1 ('button')
                            344 BINARY_SUBSCR
                            354 LOAD_CONST               6 ('active')
                            356 BINARY_SUBSCR
                            366 LOAD_CONST               5 ('border_width')
                            368 BINARY_SUBSCR
                            378 LOAD_FAST                0 (self)
                            380 STORE_ATTR               7 (button_active_border_width)
                
-               177     >>  390 LOAD_CONST               7 ('pressed')
+               189     >>  390 LOAD_CONST               7 ('pressed')
                            392 LOAD_FAST                1 (dict)
                            394 LOAD_CONST               1 ('button')
                            396 BINARY_SUBSCR
                            406 CONTAINS_OP              0
                            408 POP_JUMP_FORWARD_IF_FALSE   100 (to 610)
                
-               178         410 LOAD_FAST                1 (dict)
+               190         410 LOAD_FAST                1 (dict)
                            412 LOAD_CONST               1 ('button')
                            414 BINARY_SUBSCR
                            424 LOAD_CONST               7 ('pressed')
                            426 BINARY_SUBSCR
                            436 LOAD_CONST               2 ('back')
                            438 BINARY_SUBSCR
                            448 LOAD_FAST                0 (self)
                            450 STORE_ATTR               8 (button_pressed_back)
                
-               179         460 LOAD_FAST                1 (dict)
+               191         460 LOAD_FAST                1 (dict)
                            462 LOAD_CONST               1 ('button')
                            464 BINARY_SUBSCR
                            474 LOAD_CONST               7 ('pressed')
                            476 BINARY_SUBSCR
                            486 LOAD_CONST               3 ('border')
                            488 BINARY_SUBSCR
                            498 LOAD_FAST                0 (self)
                            500 STORE_ATTR               9 (button_pressed_border)
                
-               180         510 LOAD_FAST                1 (dict)
+               192         510 LOAD_FAST                1 (dict)
                            512 LOAD_CONST               1 ('button')
                            514 BINARY_SUBSCR
                            524 LOAD_CONST               7 ('pressed')
                            526 BINARY_SUBSCR
                            536 LOAD_CONST               4 ('text_back')
                            538 BINARY_SUBSCR
                            548 LOAD_FAST                0 (self)
                            550 STORE_ATTR              10 (button_pressed_text_back)
                
-               181         560 LOAD_FAST                1 (dict)
+               193         560 LOAD_FAST                1 (dict)
                            562 LOAD_CONST               1 ('button')
                            564 BINARY_SUBSCR
                            574 LOAD_CONST               7 ('pressed')
                            576 BINARY_SUBSCR
                            586 LOAD_CONST               5 ('border_width')
                            588 BINARY_SUBSCR
                            598 LOAD_FAST                0 (self)
                            600 STORE_ATTR              11 (button_pressed_border_width)
                
-               183     >>  610 LOAD_FAST                1 (dict)
+               195     >>  610 LOAD_FAST                1 (dict)
                            612 LOAD_FAST                0 (self)
                            614 STORE_ATTR              12 (_palette)
                
-               185         624 LOAD_FAST                0 (self)
+               197         624 LOAD_FAST                0 (self)
                            626 LOAD_ATTR                0 (button_back)
                            636 LOAD_FAST                0 (self)
                            638 STORE_ATTR              13 (_button_back)
                
-               186         648 LOAD_FAST                0 (self)
+               198         648 LOAD_FAST                0 (self)
                            650 LOAD_ATTR                1 (button_border)
                            660 LOAD_FAST                0 (self)
                            662 STORE_ATTR              14 (_button_border)
                
-               187         672 LOAD_FAST                0 (self)
+               199         672 LOAD_FAST                0 (self)
                            674 LOAD_ATTR                3 (button_border_width)
                            684 LOAD_FAST                0 (self)
                            686 STORE_ATTR              15 (_button_border_width)
                
-               188         696 LOAD_FAST                0 (self)
+               200         696 LOAD_FAST                0 (self)
                            698 LOAD_ATTR                2 (button_text_back)
                            708 LOAD_FAST                0 (self)
                            710 STORE_ATTR              16 (_button_text_back)
                
-               190         720 NOP
+               202         720 NOP
                
-               191         722 LOAD_FAST                0 (self)
+               203         722 LOAD_FAST                0 (self)
                            724 LOAD_METHOD             17 (_draw)
                            746 LOAD_CONST               0 (None)
                            748 PRECALL                  1
                            752 CALL                     1
                            762 POP_TOP
                            764 LOAD_CONST               0 (None)
                            766 RETURN_VALUE
                        >>  768 PUSH_EXC_INFO
                
-               192         770 LOAD_GLOBAL             36 (AttributeError)
+               204         770 LOAD_GLOBAL             36 (AttributeError)
                            782 CHECK_EXC_MATCH
                            784 POP_JUMP_FORWARD_IF_FALSE     4 (to 794)
                            786 POP_TOP
                
-               193         788 POP_EXCEPT
+               205         788 POP_EXCEPT
                            790 LOAD_CONST               0 (None)
                            792 RETURN_VALUE
                
-               192     >>  794 RERAISE                  0
+               204     >>  794 RERAISE                  0
                        >>  796 COPY                     3
                            798 POP_EXCEPT
                            800 RERAISE                  1
                
-               195     >>  802 LOAD_FAST                0 (self)
+               207     >>  802 LOAD_FAST                0 (self)
                            804 LOAD_ATTR               12 (_palette)
                            814 RETURN_VALUE
                ExceptionTable:
                  722 to 762 -> 768 [0]
                  768 to 786 -> 796 [1] lasti
                  794 to 794 -> 796 [1] lasti
                consts
@@ -1650,153 +1705,154 @@
                   'pressed'
                names      ('button_back', 'button_border', 'button_text_back', 'button_border_width', 'button_active_back', 'button_active_border', 'button_active_text_back', 'button_active_border_width', 'button_pressed_back', 'button_pressed_border', 'button_pressed_text_back', 'button_pressed_border_width', '_palette', '_button_back', '_button_border', '_button_border_width', '_button_text_back', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette'
-               firstlineno 163
+               firstlineno 175
                lnotab
                   0x020106010a012601260126012602140132013201320132021401320132
                   01320132020e02180118011801180202013001120106ff0803
+            ('return', None)
             (None,)
-         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'configure', '_draw', '_click', '_unclick', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', '__init__', 'configure', 'update', '_draw', '_click', '_unclick', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawBasicButton'
          firstlineno 6
-         lnotab 0x0c011c1a0a0a0613080b080b080908090e060603061a061a
+         lnotab 0x0c0204041c1a0a0a0c070813080b080b080908090e060603061a061a
       'AdwDrawBasicButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         198           0 RESUME                   0
+         210           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         199          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 199>)
+         211          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 211>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               199           0 RESUME                   0
+               211           0 RESUME                   0
                
-               200           2 LOAD_FAST                0 (self)
+               212           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 199
+               firstlineno 211
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawButton'
-         firstlineno 198
+         firstlineno 210
          lnotab 0x0a01
       'AdwDrawButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         203           0 RESUME                   0
+         215           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         204          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 204>)
+         216          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 216>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               204           0 RESUME                   0
+               216           0 RESUME                   0
                
-               205           2 LOAD_FAST                0 (self)
+               217           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 204
+               firstlineno 216
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawDarkButton'
-         firstlineno 203
+         firstlineno 215
          lnotab 0x0a01
       'AdwDrawDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         208           0 RESUME                   0
+         220           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         209          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 209>)
+         221          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 221>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawAccentButton'
             code
@@ -1804,57 +1860,57 @@
                nlocals   : 1
                stacksize : 13
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664036404640564079c04640864086409640564079c
                   04640a9c066901a6010000ab010000000000000000010064005300
-               209           0 RESUME                   0
+               221           0 RESUME                   0
                
-               210           2 LOAD_FAST                0 (self)
+               222           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               212          26 LOAD_CONST               1 ('button')
+               224          26 LOAD_CONST               1 ('button')
                
-               213          28 LOAD_CONST               2 ('#0067c0')
+               225          28 LOAD_CONST               2 ('#0067c0')
                
-               214          30 LOAD_CONST               3 ('#1473c5')
+               226          30 LOAD_CONST               3 ('#1473c5')
                
-               215          32 LOAD_CONST               4 ('#ffffff')
+               227          32 LOAD_CONST               4 ('#ffffff')
                
-               216          34 LOAD_CONST               5 (1)
+               228          34 LOAD_CONST               5 (1)
                
-               219          36 LOAD_CONST               6 ('#1975c5')
+               231          36 LOAD_CONST               6 ('#1975c5')
                
-               220          38 LOAD_CONST               3 ('#1473c5')
+               232          38 LOAD_CONST               3 ('#1473c5')
                
-               221          40 LOAD_CONST               4 ('#ffffff')
+               233          40 LOAD_CONST               4 ('#ffffff')
                
-               222          42 LOAD_CONST               5 (1)
+               234          42 LOAD_CONST               5 (1)
                
-               218          44 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
+               230          44 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
                             46 BUILD_CONST_KEY_MAP      4
                
-               226          48 LOAD_CONST               8 ('#3284cb')
+               238          48 LOAD_CONST               8 ('#3284cb')
                
-               227          50 LOAD_CONST               8 ('#3284cb')
+               239          50 LOAD_CONST               8 ('#3284cb')
                
-               228          52 LOAD_CONST               9 ('#fdfdfd')
+               240          52 LOAD_CONST               9 ('#fdfdfd')
                
-               229          54 LOAD_CONST               5 (1)
+               241          54 LOAD_CONST               5 (1)
                
-               225          56 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
+               237          56 LOAD_CONST               7 (('back', 'border', 'text_back', 'border_width'))
                             58 BUILD_CONST_KEY_MAP      4
                
-               212          60 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               224          60 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             62 BUILD_CONST_KEY_MAP      6
                
-               211          64 BUILD_MAP                1
+               223          64 BUILD_MAP                1
                
-               210          66 PRECALL                  1
+               222          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'button'
@@ -1869,75 +1925,75 @@
                   ('back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 209
+               firstlineno 221
                lnotab
                   0x020118020201020102010201020302010201020102fc04080201020102
                   0102fc04f304ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawAccentButton'
-         firstlineno 208
+         firstlineno 220
          lnotab 0x0a01
       'AdwDrawAccentButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0384005a05640484005a06640584005a07640684005a0864098800660164
             0884095a09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         237           2 RESUME                   0
+         249           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         238          12 LOAD_CLOSURE             0 (__class__)
+         250          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 238>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 250>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         241          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\button.py", line 241>)
+         253          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\button.py", line 253>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         244          28 LOAD_CONST               3 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 244>)
+         256          28 LOAD_CONST               3 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 256>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               5 (_draw)
          
-         264          34 LOAD_CONST               4 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 264>)
+         276          34 LOAD_CONST               4 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 276>)
                       36 MAKE_FUNCTION            0
                       38 STORE_NAME               6 (default_palette)
          
-         267          40 LOAD_CONST               5 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\button.py", line 267>)
+         279          40 LOAD_CONST               5 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\button.py", line 279>)
                       42 MAKE_FUNCTION            0
                       44 STORE_NAME               7 (palette_light)
          
-         294          46 LOAD_CONST               6 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\button.py", line 294>)
+         306          46 LOAD_CONST               6 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\button.py", line 306>)
                       48 MAKE_FUNCTION            0
                       50 STORE_NAME               8 (palette_dark)
          
-         321          52 LOAD_CONST               9 ((None,))
+         333          52 LOAD_CONST               9 ((None,))
                       54 LOAD_CLOSURE             0 (__class__)
                       56 BUILD_TUPLE              1
-                      58 LOAD_CONST               8 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 321>)
+                      58 LOAD_CONST               8 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 333>)
                       60 MAKE_FUNCTION            9 (defaults, closure)
                       62 STORE_NAME               9 (palette)
                       64 LOAD_CLOSURE             0 (__class__)
                       66 COPY                     1
                       68 STORE_NAME              10 (__classcell__)
                       70 RETURN_VALUE
          consts
@@ -1948,17 +2004,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               238           2 RESUME                   0
+               250           2 RESUME                   0
                
-               239           4 PUSH_NULL
+               251           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -1971,29 +2027,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '__init__'
-               firstlineno 238
+               firstlineno 250
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               241           0 RESUME                   0
+               253           0 RESUME                   0
                
-               242           2 LOAD_FAST                0 (self)
+               254           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -2011,15 +2067,15 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_other'
-               firstlineno 241
+               firstlineno 253
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2036,101 +2092,101 @@
                   007c005f0800000000000000007c00a00900000000000000000000000000
                   000000000000007c00a00300000000000000000000000000000000000000
                   00a6000000ab00000000000000000064037a0b00007c00a0040000000000
                   000000000000000000000000000000a6000000ab00000000000000000064
                   037a0b00007c006a0a00000000000000007c006a0b00000000000000007c
                   006a0c0000000000000000ac05a6050000ab0500000000000000007c005f
                   0d000000000000000064005300
-               244           0 RESUME                   0
+               256           0 RESUME                   0
                
-               245           2 LOAD_FAST                0 (self)
+               257           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               248          44 LOAD_FAST                0 (self)
+               260          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               249          68 LOAD_FAST                0 (self)
+               261          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (_button_border_width)
                             80 LOAD_CONST               2 (1)
                             82 BINARY_OP               10 (-)
                
-               250          86 LOAD_FAST                0 (self)
+               262          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (_button_border_width)
                             98 LOAD_CONST               2 (1)
                            100 BINARY_OP               10 (-)
                
-               251         104 LOAD_FAST                0 (self)
+               263         104 LOAD_FAST                0 (self)
                            106 LOAD_METHOD              3 (winfo_width)
                            128 PRECALL                  0
                            132 CALL                     0
                            142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (_button_border_width)
                            154 LOAD_CONST               3 (2)
                            156 BINARY_OP                5 (*)
                            160 BINARY_OP               10 (-)
                            164 LOAD_CONST               2 (1)
                            166 BINARY_OP                0 (+)
                
-               252         170 LOAD_FAST                0 (self)
+               264         170 LOAD_FAST                0 (self)
                            172 LOAD_METHOD              4 (winfo_height)
                            194 PRECALL                  0
                            198 CALL                     0
                            208 LOAD_FAST                0 (self)
                            210 LOAD_ATTR                2 (_button_border_width)
                            220 LOAD_CONST               3 (2)
                            222 BINARY_OP                5 (*)
                            226 BINARY_OP               10 (-)
                            230 LOAD_CONST               2 (1)
                            232 BINARY_OP                0 (+)
                            236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                5 (button_radius)
                
-               253         248 LOAD_FAST                0 (self)
+               265         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                2 (_button_border_width)
                
-               254         260 LOAD_FAST                0 (self)
+               266         260 LOAD_FAST                0 (self)
                            262 LOAD_ATTR                6 (_button_border)
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                7 (_button_back)
                
-               248         284 KW_NAMES                 4
+               260         284 KW_NAMES                 4
                            286 PRECALL                  8
                            290 CALL                     8
                            300 LOAD_FAST                0 (self)
                            302 STORE_ATTR               8 (button_frame)
                
-               258         312 LOAD_FAST                0 (self)
+               270         312 LOAD_FAST                0 (self)
                            314 LOAD_METHOD              9 (create_text)
                
-               259         336 LOAD_FAST                0 (self)
+               271         336 LOAD_FAST                0 (self)
                            338 LOAD_METHOD              3 (winfo_width)
                            360 PRECALL                  0
                            364 CALL                     0
                            374 LOAD_CONST               3 (2)
                            376 BINARY_OP               11 (/)
                            380 LOAD_FAST                0 (self)
                            382 LOAD_METHOD              4 (winfo_height)
                            404 PRECALL                  0
                            408 CALL                     0
                            418 LOAD_CONST               3 (2)
                            420 BINARY_OP               11 (/)
                
-               260         424 LOAD_FAST                0 (self)
+               272         424 LOAD_FAST                0 (self)
                            426 LOAD_ATTR               10 (text)
                            436 LOAD_FAST                0 (self)
                            438 LOAD_ATTR               11 (_button_text_back)
                
-               261         448 LOAD_FAST                0 (self)
+               273         448 LOAD_FAST                0 (self)
                            450 LOAD_ATTR               12 (button_text_font)
                
-               258         460 KW_NAMES                 5
+               270         460 KW_NAMES                 5
                            462 PRECALL                  5
                            466 CALL                     5
                            476 LOAD_FAST                0 (self)
                            478 STORE_ATTR              13 (button_text)
                            488 LOAD_CONST               0 (None)
                            490 RETURN_VALUE
                consts
@@ -2142,97 +2198,97 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect2', '_button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
-               firstlineno 244
+               firstlineno 256
                lnotab 0x02012a0318011201120142014e010c0118fa1c0a1801580118010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               264           0 RESUME                   0
+               276           0 RESUME                   0
                
-               265           2 LOAD_FAST                0 (self)
+               277           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 264
+               firstlineno 276
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096406640a9c046407640b640c640664
                   0a9c04640d9c076901a6010000ab010000000000000000010064005300
-               267           0 RESUME                   0
+               279           0 RESUME                   0
                
-               268           2 LOAD_FAST                0 (self)
+               280           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               270          26 LOAD_CONST               1 ('button')
+               282          26 LOAD_CONST               1 ('button')
                
-               271          28 LOAD_CONST               2 (8)
+               283          28 LOAD_CONST               2 (8)
                
-               272          30 LOAD_CONST               3 ('#fdfdfd')
+               284          30 LOAD_CONST               3 ('#fdfdfd')
                
-               273          32 LOAD_CONST               4 ('#eaeaea')
+               285          32 LOAD_CONST               4 ('#eaeaea')
                
-               274          34 LOAD_CONST               5 ('#1a1a1a')
+               286          34 LOAD_CONST               5 ('#1a1a1a')
                
-               275          36 LOAD_CONST               6 (1)
+               287          36 LOAD_CONST               6 (1)
                
-               278          38 LOAD_CONST               7 ('#f9f9f9')
+               290          38 LOAD_CONST               7 ('#f9f9f9')
                
-               279          40 LOAD_CONST               8 ('#454545')
+               291          40 LOAD_CONST               8 ('#454545')
                
-               280          42 LOAD_CONST               9 ('#5f5f5f')
+               292          42 LOAD_CONST               9 ('#5f5f5f')
                
-               281          44 LOAD_CONST               6 (1)
+               293          44 LOAD_CONST               6 (1)
                
-               277          46 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
+               289          46 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
                             48 BUILD_CONST_KEY_MAP      4
                
-               285          50 LOAD_CONST               7 ('#f9f9f9')
+               297          50 LOAD_CONST               7 ('#f9f9f9')
                
-               286          52 LOAD_CONST              11 ('#e2e2e2')
+               298          52 LOAD_CONST              11 ('#e2e2e2')
                
-               287          54 LOAD_CONST              12 ('#8a8a8a')
+               299          54 LOAD_CONST              12 ('#8a8a8a')
                
-               288          56 LOAD_CONST               6 (1)
+               300          56 LOAD_CONST               6 (1)
                
-               284          58 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
+               296          58 LOAD_CONST              10 (('back', 'border', 'text_back', 'border_width'))
                             60 BUILD_CONST_KEY_MAP      4
                
-               270          62 LOAD_CONST              13 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               282          62 LOAD_CONST              13 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             64 BUILD_CONST_KEY_MAP      7
                
-               269          66 BUILD_MAP                1
+               281          66 BUILD_MAP                1
                
-               268          68 PRECALL                  1
+               280          68 PRECALL                  1
                             72 CALL                     1
                             82 POP_TOP
                             84 LOAD_CONST               0 (None)
                             86 RETURN_VALUE
                consts
                   None
                   'button'
@@ -2250,72 +2306,72 @@
                   ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette_light'
-               firstlineno 267
+               firstlineno 279
                lnotab
                   0x0201180202010201020102010201020302010201020102fc0408020102
                   01020102fc04f204ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764046408640664099c04640a6404640b640664
                   099c04640c9c076901a6010000ab010000000000000000010064005300
-               294           0 RESUME                   0
+               306           0 RESUME                   0
                
-               295           2 LOAD_FAST                0 (self)
+               307           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               297          26 LOAD_CONST               1 ('button')
+               309          26 LOAD_CONST               1 ('button')
                
-               298          28 LOAD_CONST               2 (8)
+               310          28 LOAD_CONST               2 (8)
                
-               299          30 LOAD_CONST               3 ('#353535')
+               311          30 LOAD_CONST               3 ('#353535')
                
-               300          32 LOAD_CONST               4 ('#454545')
+               312          32 LOAD_CONST               4 ('#454545')
                
-               301          34 LOAD_CONST               5 ('#ffffff')
+               313          34 LOAD_CONST               5 ('#ffffff')
                
-               302          36 LOAD_CONST               6 (1)
+               314          36 LOAD_CONST               6 (1)
                
-               305          38 LOAD_CONST               7 ('#3a3a3a')
+               317          38 LOAD_CONST               7 ('#3a3a3a')
                
-               306          40 LOAD_CONST               4 ('#454545')
+               318          40 LOAD_CONST               4 ('#454545')
                
-               307          42 LOAD_CONST               8 ('#cecece')
+               319          42 LOAD_CONST               8 ('#cecece')
                
-               308          44 LOAD_CONST               6 (1)
+               320          44 LOAD_CONST               6 (1)
                
-               304          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+               316          46 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
                             48 BUILD_CONST_KEY_MAP      4
                
-               312          50 LOAD_CONST              10 ('#2f2f2f')
+               324          50 LOAD_CONST              10 ('#2f2f2f')
                
-               313          52 LOAD_CONST               4 ('#454545')
+               325          52 LOAD_CONST               4 ('#454545')
                
-               314          54 LOAD_CONST              11 ('#9a9a9a')
+               326          54 LOAD_CONST              11 ('#9a9a9a')
                
-               315          56 LOAD_CONST               6 (1)
+               327          56 LOAD_CONST               6 (1)
                
-               311          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
+               323          58 LOAD_CONST               9 (('back', 'border', 'text_back', 'border_width'))
                             60 BUILD_CONST_KEY_MAP      4
                
-               297          62 LOAD_CONST              12 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               309          62 LOAD_CONST              12 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             64 BUILD_CONST_KEY_MAP      7
                
-               296          66 BUILD_MAP                1
+               308          66 BUILD_MAP                1
                
-               295          68 PRECALL                  1
+               307          68 PRECALL                  1
                             72 CALL                     1
                             82 POP_TOP
                             84 LOAD_CONST               0 (None)
                             86 RETURN_VALUE
                consts
                   None
                   'button'
@@ -2332,15 +2388,15 @@
                   ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette_dark'
-               firstlineno 294
+               firstlineno 306
                lnotab
                   0x0201180202010201020102010201020302010201020102fc0408020102
                   01020102fc04f204ff02ff
             None
             code
                argcount  : 2
                nlocals   : 2
@@ -2350,133 +2406,133 @@
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000010064017c01760072157c01640119000000000000
                   0000006402190000000000000000007c005f020000000000000000640053
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               321           2 RESUME                   0
+               333           2 RESUME                   0
                
-               322           4 LOAD_GLOBAL              1 (NULL + super)
+               334           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (palette)
                             52 LOAD_FAST                1 (dict)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-               323          70 LOAD_CONST               1 ('button')
+               335          70 LOAD_CONST               1 ('button')
                             72 LOAD_FAST                1 (dict)
                             74 CONTAINS_OP              0
                             76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
                
-               324          78 LOAD_FAST                1 (dict)
+               336          78 LOAD_FAST                1 (dict)
                             80 LOAD_CONST               1 ('button')
                             82 BINARY_SUBSCR
                             92 LOAD_CONST               2 ('radius')
                             94 BINARY_SUBSCR
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               2 (button_radius)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-               323     >>  120 LOAD_CONST               0 (None)
+               335     >>  120 LOAD_CONST               0 (None)
                            122 RETURN_VALUE
                consts
                   None
                   'button'
                   'radius'
                names      ('super', 'palette', 'button_radius')
                varnames   ('self', 'dict')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'palette'
-               firstlineno 321
+               firstlineno 333
                lnotab 0x0401420108012aff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawBasicRoundButton'
-         firstlineno 237
+         firstlineno 249
          lnotab 0x0c010a03060306140603061b061b
       'AdwDrawBasicRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         327           0 RESUME                   0
+         339           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         328          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 328>)
+         340          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 340>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               328           0 RESUME                   0
+               340           0 RESUME                   0
                
-               329           2 LOAD_FAST                0 (self)
+               341           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 328
+               firstlineno 340
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundButton'
-         firstlineno 327
+         firstlineno 339
          lnotab 0x0a01
       'AdwDrawRoundButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         332           0 RESUME                   0
+         344           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         333          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 333>)
+         345          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 345>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton'
             code
@@ -2484,59 +2540,59 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764046405640664089c0464096409640a640664
                   089c04640b9c076901a6010000ab010000000000000000010064005300
-               333           0 RESUME                   0
+               345           0 RESUME                   0
                
-               334           2 LOAD_FAST                0 (self)
+               346           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               336          26 LOAD_CONST               1 ('button')
+               348          26 LOAD_CONST               1 ('button')
                
-               337          28 LOAD_CONST               2 (8)
+               349          28 LOAD_CONST               2 (8)
                
-               338          30 LOAD_CONST               3 ('#0067c0')
+               350          30 LOAD_CONST               3 ('#0067c0')
                
-               339          32 LOAD_CONST               4 ('#1473c5')
+               351          32 LOAD_CONST               4 ('#1473c5')
                
-               340          34 LOAD_CONST               5 ('#ffffff')
+               352          34 LOAD_CONST               5 ('#ffffff')
                
-               341          36 LOAD_CONST               6 (1)
+               353          36 LOAD_CONST               6 (1)
                
-               344          38 LOAD_CONST               7 ('#1975c5')
+               356          38 LOAD_CONST               7 ('#1975c5')
                
-               345          40 LOAD_CONST               4 ('#1473c5')
+               357          40 LOAD_CONST               4 ('#1473c5')
                
-               346          42 LOAD_CONST               5 ('#ffffff')
+               358          42 LOAD_CONST               5 ('#ffffff')
                
-               347          44 LOAD_CONST               6 (1)
+               359          44 LOAD_CONST               6 (1)
                
-               343          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               355          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             48 BUILD_CONST_KEY_MAP      4
                
-               351          50 LOAD_CONST               9 ('#3284cb')
+               363          50 LOAD_CONST               9 ('#3284cb')
                
-               352          52 LOAD_CONST               9 ('#3284cb')
+               364          52 LOAD_CONST               9 ('#3284cb')
                
-               353          54 LOAD_CONST              10 ('#fdfdfd')
+               365          54 LOAD_CONST              10 ('#fdfdfd')
                
-               354          56 LOAD_CONST               6 (1)
+               366          56 LOAD_CONST               6 (1)
                
-               350          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               362          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             60 BUILD_CONST_KEY_MAP      4
                
-               336          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               348          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             64 BUILD_CONST_KEY_MAP      7
                
-               335          66 BUILD_MAP                1
+               347          66 BUILD_MAP                1
                
-               334          68 PRECALL                  1
+               346          68 PRECALL                  1
                             72 CALL                     1
                             82 POP_TOP
                             84 LOAD_CONST               0 (None)
                             86 RETURN_VALUE
                consts
                   None
                   'button'
@@ -2552,101 +2608,101 @@
                   ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 333
+               firstlineno 345
                lnotab
                   0x0201180202010201020102010201020302010201020102fc0408020102
                   01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton'
-         firstlineno 332
+         firstlineno 344
          lnotab 0x0a01
       'AdwDrawRoundAccentButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         361           0 RESUME                   0
+         373           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         362          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 362>)
+         374          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 374>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               362           0 RESUME                   0
+               374           0 RESUME                   0
                
-               363           2 LOAD_FAST                0 (self)
+               375           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 362
+               firstlineno 374
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton'
-         firstlineno 361
+         firstlineno 373
          lnotab 0x0a01
       'AdwDrawRoundDarkButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         366           0 RESUME                   0
+         378           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         368          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 368>)
+         380          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 380>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         391          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 391>)
+         403          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 403>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton2'
             code
@@ -2667,100 +2723,100 @@
                   080000000000000000010064027c005f0800000000000000007c00a00900
                   000000000000000000000000000000000000007c00a00300000000000000
                   00000000000000000000000000a6000000ab00000000000000000064047a
                   0b00007c00a0040000000000000000000000000000000000000000a60000
                   00ab00000000000000000064047a0b00007c006a0a00000000000000007c
                   006a0b00000000000000007c006a0c0000000000000000ac06a6050000ab
                   0500000000000000007c005f0d000000000000000064005300
-               368           0 RESUME                   0
+               380           0 RESUME                   0
                
-               369           2 LOAD_FAST                0 (self)
+               381           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               372          44 LOAD_FAST                0 (self)
+               384          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect3)
                
-               373          68 LOAD_CONST               2 ('button_frame')
+               385          68 LOAD_CONST               2 ('button_frame')
                
-               374          70 LOAD_FAST                0 (self)
+               386          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                2 (_button_border_width)
                             82 LOAD_CONST               3 (1)
                             84 BINARY_OP               10 (-)
                
-               375          88 LOAD_FAST                0 (self)
+               387          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                2 (_button_border_width)
                            100 LOAD_CONST               3 (1)
                            102 BINARY_OP               10 (-)
                
-               376         106 LOAD_FAST                0 (self)
+               388         106 LOAD_FAST                0 (self)
                            108 LOAD_METHOD              3 (winfo_width)
                            130 PRECALL                  0
                            134 CALL                     0
                            144 LOAD_FAST                0 (self)
                            146 LOAD_ATTR                2 (_button_border_width)
                            156 LOAD_CONST               4 (2)
                            158 BINARY_OP                5 (*)
                            162 BINARY_OP               10 (-)
                
-               377         166 LOAD_FAST                0 (self)
+               389         166 LOAD_FAST                0 (self)
                            168 LOAD_METHOD              4 (winfo_height)
                            190 PRECALL                  0
                            194 CALL                     0
                            204 LOAD_FAST                0 (self)
                            206 LOAD_ATTR                2 (_button_border_width)
                            216 LOAD_CONST               4 (2)
                            218 BINARY_OP                5 (*)
                            222 BINARY_OP               10 (-)
                
-               378         226 LOAD_FAST                0 (self)
+               390         226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                5 (button_radius)
                
-               379         238 LOAD_FAST                0 (self)
+               391         238 LOAD_FAST                0 (self)
                            240 LOAD_ATTR                6 (_button_border)
                            250 LOAD_FAST                0 (self)
                            252 LOAD_ATTR                7 (_button_back)
                
-               372         262 KW_NAMES                 5
+               384         262 KW_NAMES                 5
                            264 PRECALL                  8
                            268 CALL                     8
                            278 POP_TOP
                
-               382         280 LOAD_CONST               2 ('button_frame')
+               394         280 LOAD_CONST               2 ('button_frame')
                            282 LOAD_FAST                0 (self)
                            284 STORE_ATTR               8 (button_frame)
                
-               385         294 LOAD_FAST                0 (self)
+               397         294 LOAD_FAST                0 (self)
                            296 LOAD_METHOD              9 (create_text)
                
-               386         318 LOAD_FAST                0 (self)
+               398         318 LOAD_FAST                0 (self)
                            320 LOAD_METHOD              3 (winfo_width)
                            342 PRECALL                  0
                            346 CALL                     0
                            356 LOAD_CONST               4 (2)
                            358 BINARY_OP               11 (/)
                            362 LOAD_FAST                0 (self)
                            364 LOAD_METHOD              4 (winfo_height)
                            386 PRECALL                  0
                            390 CALL                     0
                            400 LOAD_CONST               4 (2)
                            402 BINARY_OP               11 (/)
                
-               387         406 LOAD_FAST                0 (self)
+               399         406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (text)
                            418 LOAD_FAST                0 (self)
                            420 LOAD_ATTR               11 (_button_text_back)
                
-               388         430 LOAD_FAST                0 (self)
+               400         430 LOAD_FAST                0 (self)
                            432 LOAD_ATTR               12 (button_text_font)
                
-               385         442 KW_NAMES                 6
+               397         442 KW_NAMES                 6
                            444 PRECALL                  5
                            448 CALL                     5
                            458 LOAD_FAST                0 (self)
                            460 STORE_ATTR              13 (button_text)
                            470 LOAD_CONST               0 (None)
                            472 RETURN_VALUE
                consts
@@ -2773,68 +2829,68 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect3', '_button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
-               firstlineno 368
+               firstlineno 380
                lnotab
                   0x02012a0318010201120112013c013c010c0118f9120a0e031801580118
                   010cfd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               391           0 RESUME                   0
+               403           0 RESUME                   0
                
-               392           2 LOAD_FAST                0 (self)
+               404           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 391
+               firstlineno 403
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundButton2'
-         firstlineno 366
+         firstlineno 378
          lnotab 0x0a020617
       'AdwDrawRoundButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         395           0 RESUME                   0
+         407           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         396          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 396>)
+         408          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 408>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton2'
             code
@@ -2842,59 +2898,59 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764046405640664089c0464096409640a640664
                   089c04640b9c076901a6010000ab010000000000000000010064005300
-               396           0 RESUME                   0
+               408           0 RESUME                   0
                
-               397           2 LOAD_FAST                0 (self)
+               409           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               399          26 LOAD_CONST               1 ('button')
+               411          26 LOAD_CONST               1 ('button')
                
-               400          28 LOAD_CONST               2 (8)
+               412          28 LOAD_CONST               2 (8)
                
-               401          30 LOAD_CONST               3 ('#0067c0')
+               413          30 LOAD_CONST               3 ('#0067c0')
                
-               402          32 LOAD_CONST               4 ('#1473c5')
+               414          32 LOAD_CONST               4 ('#1473c5')
                
-               403          34 LOAD_CONST               5 ('#ffffff')
+               415          34 LOAD_CONST               5 ('#ffffff')
                
-               404          36 LOAD_CONST               6 (1)
+               416          36 LOAD_CONST               6 (1)
                
-               407          38 LOAD_CONST               7 ('#1975c5')
+               419          38 LOAD_CONST               7 ('#1975c5')
                
-               408          40 LOAD_CONST               4 ('#1473c5')
+               420          40 LOAD_CONST               4 ('#1473c5')
                
-               409          42 LOAD_CONST               5 ('#ffffff')
+               421          42 LOAD_CONST               5 ('#ffffff')
                
-               410          44 LOAD_CONST               6 (1)
+               422          44 LOAD_CONST               6 (1)
                
-               406          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               418          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             48 BUILD_CONST_KEY_MAP      4
                
-               414          50 LOAD_CONST               9 ('#3284cb')
+               426          50 LOAD_CONST               9 ('#3284cb')
                
-               415          52 LOAD_CONST               9 ('#3284cb')
+               427          52 LOAD_CONST               9 ('#3284cb')
                
-               416          54 LOAD_CONST              10 ('#fdfdfd')
+               428          54 LOAD_CONST              10 ('#fdfdfd')
                
-               417          56 LOAD_CONST               6 (1)
+               429          56 LOAD_CONST               6 (1)
                
-               413          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               425          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             60 BUILD_CONST_KEY_MAP      4
                
-               399          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               411          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             64 BUILD_CONST_KEY_MAP      7
                
-               398          66 BUILD_MAP                1
+               410          66 BUILD_MAP                1
                
-               397          68 PRECALL                  1
+               409          68 PRECALL                  1
                             72 CALL                     1
                             82 POP_TOP
                             84 LOAD_CONST               0 (None)
                             86 RETURN_VALUE
                consts
                   None
                   'button'
@@ -2910,101 +2966,101 @@
                   ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 396
+               firstlineno 408
                lnotab
                   0x0201180202010201020102010201020302010201020102fc0408020102
                   01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton2'
-         firstlineno 395
+         firstlineno 407
          lnotab 0x0a01
       'AdwDrawRoundAccentButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         424           0 RESUME                   0
+         436           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton2')
                        8 STORE_NAME               2 (__qualname__)
          
-         425          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 425>)
+         437          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 437>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton2'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               425           0 RESUME                   0
+               437           0 RESUME                   0
                
-               426           2 LOAD_FAST                0 (self)
+               438           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 425
+               firstlineno 437
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton2'
-         firstlineno 424
+         firstlineno 436
          lnotab 0x0a01
       'AdwDrawRoundDarkButton2'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a03640284005a0464035300
-         429           0 RESUME                   0
+         441           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         430          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 430>)
+         442          10 LOAD_CONST               1 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 442>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (_draw)
          
-         452          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 452>)
+         464          16 LOAD_CONST               2 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 464>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (default_palette)
                       22 LOAD_CONST               3 (None)
                       24 RETURN_VALUE
          consts
             'AdwDrawRoundButton3'
             code
@@ -3026,104 +3082,104 @@
                   00010064057c005f0800000000000000007c00a009000000000000000000
                   00000000000000000000007c00a003000000000000000000000000000000
                   0000000000a6000000ab00000000000000000064037a0b00007c00a00400
                   00000000000000000000000000000000000000a6000000ab000000000000
                   00000064037a0b00007c006a0a00000000000000007c006a0b0000000000
                   0000007c006a0c0000000000000000ac06a6050000ab0500000000000000
                   007c005f0d000000000000000064005300
-               430           0 RESUME                   0
+               442           0 RESUME                   0
                
-               431           2 LOAD_FAST                0 (self)
+               443           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               434          44 LOAD_FAST                0 (self)
+               446          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               435          68 LOAD_FAST                0 (self)
+               447          68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                2 (_button_border_width)
                             80 LOAD_CONST               2 (1)
                             82 BINARY_OP               10 (-)
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                2 (_button_border_width)
                             98 LOAD_CONST               2 (1)
                            100 BINARY_OP               10 (-)
                
-               436         104 LOAD_FAST                0 (self)
+               448         104 LOAD_FAST                0 (self)
                            106 LOAD_METHOD              3 (winfo_width)
                            128 PRECALL                  0
                            132 CALL                     0
                            142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (_button_border_width)
                            154 LOAD_CONST               3 (2)
                            156 BINARY_OP                5 (*)
                            160 BINARY_OP               10 (-)
                            164 LOAD_CONST               2 (1)
                            166 BINARY_OP                0 (+)
                
-               437         170 LOAD_FAST                0 (self)
+               449         170 LOAD_FAST                0 (self)
                            172 LOAD_METHOD              4 (winfo_height)
                            194 PRECALL                  0
                            198 CALL                     0
                            208 LOAD_FAST                0 (self)
                            210 LOAD_ATTR                2 (_button_border_width)
                            220 LOAD_CONST               3 (2)
                            222 BINARY_OP                5 (*)
                            226 BINARY_OP               10 (-)
                            230 LOAD_CONST               2 (1)
                            232 BINARY_OP                0 (+)
                
-               438         236 LOAD_FAST                0 (self)
+               450         236 LOAD_FAST                0 (self)
                            238 LOAD_ATTR                5 (button_radius)
                
-               439         248 LOAD_FAST                0 (self)
+               451         248 LOAD_FAST                0 (self)
                            250 LOAD_ATTR                2 (_button_border_width)
                
-               440         260 LOAD_FAST                0 (self)
+               452         260 LOAD_FAST                0 (self)
                            262 LOAD_ATTR                6 (_button_border)
                            272 LOAD_FAST                0 (self)
                            274 LOAD_ATTR                7 (_button_back)
                
-               434         284 KW_NAMES                 4
+               446         284 KW_NAMES                 4
                            286 PRECALL                  8
                            290 CALL                     8
                            300 POP_TOP
                
-               443         302 LOAD_CONST               5 ('button_frame')
+               455         302 LOAD_CONST               5 ('button_frame')
                            304 LOAD_FAST                0 (self)
                            306 STORE_ATTR               8 (button_frame)
                
-               446         316 LOAD_FAST                0 (self)
+               458         316 LOAD_FAST                0 (self)
                            318 LOAD_METHOD              9 (create_text)
                
-               447         340 LOAD_FAST                0 (self)
+               459         340 LOAD_FAST                0 (self)
                            342 LOAD_METHOD              3 (winfo_width)
                            364 PRECALL                  0
                            368 CALL                     0
                            378 LOAD_CONST               3 (2)
                            380 BINARY_OP               11 (/)
                            384 LOAD_FAST                0 (self)
                            386 LOAD_METHOD              4 (winfo_height)
                            408 PRECALL                  0
                            412 CALL                     0
                            422 LOAD_CONST               3 (2)
                            424 BINARY_OP               11 (/)
                
-               448         428 LOAD_FAST                0 (self)
+               460         428 LOAD_FAST                0 (self)
                            430 LOAD_ATTR               10 (text)
                            440 LOAD_FAST                0 (self)
                            442 LOAD_ATTR               11 (_button_text_back)
                
-               449         452 LOAD_FAST                0 (self)
+               461         452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR               12 (button_text_font)
                
-               446         464 KW_NAMES                 6
+               458         464 KW_NAMES                 6
                            466 PRECALL                  5
                            470 CALL                     5
                            480 LOAD_FAST                0 (self)
                            482 STORE_ATTR              13 (button_text)
                            492 LOAD_CONST               0 (None)
                            494 RETURN_VALUE
                consts
@@ -3136,68 +3192,68 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_round_rect4', '_button_border_width', 'winfo_width', 'winfo_height', 'button_radius', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
-               firstlineno 430
+               firstlineno 442
                lnotab
                   0x02012a0318012401420142010c010c0118fa12090e031801580118010c
                   fd
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               452           0 RESUME                   0
+               464           0 RESUME                   0
                
-               453           2 LOAD_FAST                0 (self)
+               465           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 452
+               firstlineno 464
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '_draw', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundButton3'
-         firstlineno 429
+         firstlineno 441
          lnotab 0x0a010616
       'AdwDrawRoundButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         456           0 RESUME                   0
+         468           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundAccentButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         457          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 457>)
+         469          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 469>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundAccentButton3'
             code
@@ -3205,59 +3261,59 @@
                nlocals   : 1
                stacksize : 14
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764046405640664089c0464096409640a640664
                   089c04640b9c076901a6010000ab010000000000000000010064005300
-               457           0 RESUME                   0
+               469           0 RESUME                   0
                
-               458           2 LOAD_FAST                0 (self)
+               470           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               460          26 LOAD_CONST               1 ('button')
+               472          26 LOAD_CONST               1 ('button')
                
-               461          28 LOAD_CONST               2 (8)
+               473          28 LOAD_CONST               2 (8)
                
-               462          30 LOAD_CONST               3 ('#0067c0')
+               474          30 LOAD_CONST               3 ('#0067c0')
                
-               463          32 LOAD_CONST               4 ('#1473c5')
+               475          32 LOAD_CONST               4 ('#1473c5')
                
-               464          34 LOAD_CONST               5 ('#ffffff')
+               476          34 LOAD_CONST               5 ('#ffffff')
                
-               465          36 LOAD_CONST               6 (1)
+               477          36 LOAD_CONST               6 (1)
                
-               468          38 LOAD_CONST               7 ('#1975c5')
+               480          38 LOAD_CONST               7 ('#1975c5')
                
-               469          40 LOAD_CONST               4 ('#1473c5')
+               481          40 LOAD_CONST               4 ('#1473c5')
                
-               470          42 LOAD_CONST               5 ('#ffffff')
+               482          42 LOAD_CONST               5 ('#ffffff')
                
-               471          44 LOAD_CONST               6 (1)
+               483          44 LOAD_CONST               6 (1)
                
-               467          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               479          46 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             48 BUILD_CONST_KEY_MAP      4
                
-               475          50 LOAD_CONST               9 ('#3284cb')
+               487          50 LOAD_CONST               9 ('#3284cb')
                
-               476          52 LOAD_CONST               9 ('#3284cb')
+               488          52 LOAD_CONST               9 ('#3284cb')
                
-               477          54 LOAD_CONST              10 ('#fdfdfd')
+               489          54 LOAD_CONST              10 ('#fdfdfd')
                
-               478          56 LOAD_CONST               6 (1)
+               490          56 LOAD_CONST               6 (1)
                
-               474          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
+               486          58 LOAD_CONST               8 (('back', 'border', 'text_back', 'border_width'))
                             60 BUILD_CONST_KEY_MAP      4
                
-               460          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
+               472          62 LOAD_CONST              11 (('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed'))
                             64 BUILD_CONST_KEY_MAP      7
                
-               459          66 BUILD_MAP                1
+               471          66 BUILD_MAP                1
                
-               458          68 PRECALL                  1
+               470          68 PRECALL                  1
                             72 CALL                     1
                             82 POP_TOP
                             84 LOAD_CONST               0 (None)
                             86 RETURN_VALUE
                consts
                   None
                   'button'
@@ -3273,111 +3329,111 @@
                   ('radius', 'back', 'border', 'text_back', 'border_width', 'active', 'pressed')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 457
+               firstlineno 469
                lnotab
                   0x0201180202010201020102010201020302010201020102fc0408020102
                   01020102fc04f204ff02ff
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundAccentButton3'
-         firstlineno 456
+         firstlineno 468
          lnotab 0x0a01
       'AdwDrawRoundAccentButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         485           0 RESUME                   0
+         497           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkButton3')
                        8 STORE_NAME               2 (__qualname__)
          
-         486          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 486>)
+         498          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 498>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkButton3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               486           0 RESUME                   0
+               498           0 RESUME                   0
                
-               487           2 LOAD_FAST                0 (self)
+               499           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 486
+               firstlineno 498
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawRoundDarkButton3'
-         firstlineno 485
+         firstlineno 497
          lnotab 0x0a01
       'AdwDrawRoundDarkButton3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026401640164029c02880066016403840a5a
             03640484005a04880078015a055300
                        0 MAKE_CELL                0 (__class__)
          
-         491           2 RESUME                   0
+         503           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicCircularButton')
                       10 STORE_NAME               2 (__qualname__)
          
-         492          12 LOAD_CONST               1 (120)
+         504          12 LOAD_CONST               1 (120)
                       14 LOAD_CONST               1 (120)
                       16 LOAD_CONST               2 (('width', 'height'))
                       18 BUILD_CONST_KEY_MAP      2
                       20 LOAD_CLOSURE             0 (__class__)
                       22 BUILD_TUPLE              1
-                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 492>)
+                      24 LOAD_CONST               3 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\button.py", line 504>)
                       26 MAKE_FUNCTION           10 (kwdefaults, closure)
                       28 STORE_NAME               3 (__init__)
          
-         495          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 495>)
+         507          30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\button.py", line 507>)
                       32 MAKE_FUNCTION            0
                       34 STORE_NAME               4 (_draw)
                       36 LOAD_CLOSURE             0 (__class__)
                       38 COPY                     1
                       40 STORE_NAME               5 (__classcell__)
                       42 RETURN_VALUE
          consts
@@ -3391,17 +3447,17 @@
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c037c017c0264019c027c04a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               492           2 RESUME                   0
+               504           2 RESUME                   0
                
-               493           4 PUSH_NULL
+               505           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                3 (args)
                             44 LOAD_FAST                1 (width)
                             46 LOAD_FAST                2 (height)
@@ -3418,15 +3474,15 @@
                   ('width', 'height')
                names      ('super', '__init__')
                varnames   ('self', 'width', 'height', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '__init__'
-               firstlineno 492
+               firstlineno 504
                lnotab 0x0401
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -3440,80 +3496,80 @@
                   0000007c005f0700000000000000007c00a0080000000000000000000000
                   0000000000000000007c00a0020000000000000000000000000000000000
                   000000a6000000ab00000000000000000064057a0b00007c00a003000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   0064057a0b00007c006a0900000000000000007c006a0a00000000000000
                   007c006a0b0000000000000000ac06a6050000ab0500000000000000007c
                   005f0c000000000000000064005300
-               495           0 RESUME                   0
+               507           0 RESUME                   0
                
-               496           2 LOAD_FAST                0 (self)
+               508           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               499          44 LOAD_FAST                0 (self)
+               511          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_oval)
                
-               500          68 LOAD_CONST               2 (1.5)
+               512          68 LOAD_CONST               2 (1.5)
                             70 LOAD_CONST               2 (1.5)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                
-               501         160 LOAD_FAST                0 (self)
+               513         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (button_border_width)
                
-               502         172 LOAD_FAST                0 (self)
+               514         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_button_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_button_back)
                
-               499         196 KW_NAMES                 4
+               511         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (button_frame)
                
-               506         224 LOAD_FAST                0 (self)
+               518         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_text)
                
-               507         248 LOAD_FAST                0 (self)
+               519         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-               508         336 LOAD_FAST                0 (self)
+               520         336 LOAD_FAST                0 (self)
                            338 LOAD_ATTR                9 (text)
                            348 LOAD_FAST                0 (self)
                            350 LOAD_ATTR               10 (_button_text_back)
                
-               509         360 LOAD_FAST                0 (self)
+               521         360 LOAD_FAST                0 (self)
                            362 LOAD_ATTR               11 (button_text_font)
                
-               506         372 KW_NAMES                 6
+               518         372 KW_NAMES                 6
                            374 PRECALL                  5
                            378 CALL                     5
                            388 LOAD_FAST                0 (self)
                            390 STORE_ATTR              12 (button_text)
                            400 LOAD_CONST               0 (None)
                            402 RETURN_VALUE
                consts
@@ -3526,135 +3582,135 @@
                   ('text', 'fill', 'font')
                names      ('delete', 'create_oval', 'winfo_width', 'winfo_height', 'button_border_width', '_button_border', '_button_back', 'button_frame', 'create_text', 'text', '_button_text_back', 'button_text_font', 'button_text')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       '_draw'
-               firstlineno 495
+               firstlineno 507
                lnotab 0x02012a0318015c010c0118fd1c071801580118010cfd
          names      ('__name__', '__module__', '__qualname__', '__init__', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawBasicCircularButton'
-         firstlineno 491
+         firstlineno 503
          lnotab 0x0c011203
       'AdwDrawBasicCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         513           0 RESUME                   0
+         525           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         514          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 514>)
+         526          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 526>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               514           0 RESUME                   0
+               526           0 RESUME                   0
                
-               515           2 LOAD_FAST                0 (self)
+               527           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 514
+               firstlineno 526
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawCircularButton'
-         firstlineno 513
+         firstlineno 525
          lnotab 0x0a01
       'AdwDrawCircularButton'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         518           0 RESUME                   0
+         530           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawCircularDarkButton')
                        8 STORE_NAME               2 (__qualname__)
          
-         519          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 519>)
+         531          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\button.py", line 531>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawCircularDarkButton'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               519           0 RESUME                   0
+               531           0 RESUME                   0
                
-               520           2 LOAD_FAST                0 (self)
+               532           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
                name       'default_palette'
-               firstlineno 519
+               firstlineno 531
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       'AdwDrawCircularDarkButton'
-         firstlineno 518
+         firstlineno 530
          lnotab 0x0a01
       'AdwDrawCircularDarkButton'
       '__main__'
       ('Tk',)
       'Hello'
       ('text',)
       '<<Click>>'
@@ -3662,139 +3718,139 @@
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         529           0 RESUME                   0
+         541           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 529
+         firstlineno 541
          lnotab 0x
       'x'
       5
       ('fill', 'padx', 'pady')
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         533           0 RESUME                   0
+         545           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 533
+         firstlineno 545
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         537           0 RESUME                   0
+         549           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 537
+         firstlineno 549
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         541           0 RESUME                   0
+         553           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button4 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button4 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 541
+         firstlineno 553
          lnotab 0x
       code
          argcount  : 1
          nlocals   : 1
          stacksize : 3
          flags     : 3
          code
             0x97007401000000000000000000006401a6010000ab0100000000000000
             005300
-         545           0 RESUME                   0
+         557           0 RESUME                   0
                        2 LOAD_GLOBAL              1 (NULL + print)
                       14 LOAD_CONST               1 ('button6 clicked')
                       16 PRECALL                  1
                       20 CALL                     1
                       30 RETURN_VALUE
          consts
             None
             'button6 clicked'
          names      ('print',)
          varnames   ('evt',)
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
          name       '<lambda>'
-         firstlineno 545
+         firstlineno 557
          lnotab 0x
       None
    names      ('tkinter.font', 'Font', 'nametofont', 'tkadw.windows.canvas.widget', 'AdwWidget', 'AdwDrawBasicButton', 'AdwDrawButton', 'AdwDrawDarkButton', 'AdwDrawAccentButton', 'AdwDrawBasicRoundButton', 'AdwDrawRoundButton', 'AdwDrawRoundAccentButton', 'AdwDrawRoundDarkButton', 'AdwDrawRoundButton2', 'AdwDrawRoundAccentButton2', 'AdwDrawRoundDarkButton2', 'AdwDrawRoundButton3', 'AdwDrawRoundAccentButton3', 'AdwDrawRoundDarkButton3', 'AdwDrawBasicCircularButton', 'AdwDrawCircularButton', 'AdwDrawCircularDarkButton', '__name__', 'tkinter', 'Tk', 'root', 'button', 'bind', 'pack', 'button4', 'button7', 'button10', 'button13', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f00411c051c051c1d1c5a1c051c1d1c051c1d1c
+      0x00ff020110010c041c7f004d1c051c051c1d1c5a1c051c1d1c051c1d1c
       1d1c051c1b1c1d1c061c161c051c050e010c02140218012e01300218012e
       01300218012e01300218012e01300218012e0130022ce7
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/separator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files 26% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xf3c8a464 (Wed Jul  5 01:35:47 2023 UTC)
-files sz: 17760
+moddate:  0x59cdaa64 (Sun Jul  9 15:08:09 2023 UTC)
+files sz: 17817
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -58,697 +58,716 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicText')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicText)
    
-   261          58 PUSH_NULL
+   263          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 261>)
+                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 263>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawText')
                 68 LOAD_NAME                5 (AdwDrawBasicText)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawText)
    
-   266          86 PUSH_NULL
+   268          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 266>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 268>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkText')
                 96 LOAD_NAME                5 (AdwDrawBasicText)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkText)
    
-   272         114 PUSH_NULL
+   274         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 272>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 274>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundText')
                124 LOAD_NAME                5 (AdwDrawBasicText)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundText)
    
-   380         142 PUSH_NULL
+   382         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 380>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 382>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundText')
                152 LOAD_NAME                8 (AdwDrawBasicRoundText)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundText)
    
-   385         170 PUSH_NULL
+   387         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 385>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 387>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkText')
                180 LOAD_NAME                8 (AdwDrawBasicRoundText)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkText)
    
-   390         198 PUSH_NULL
+   392         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 390>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 392>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundText3')
                208 LOAD_NAME                8 (AdwDrawBasicRoundText)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundText3)
    
-   499         226 PUSH_NULL
+   501         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 499>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 501>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundText3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundText3)
    
-   504         254 PUSH_NULL
+   506         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 504>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 506>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkText3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkText3)
    
-   509         282 LOAD_NAME               14 (__name__)
+   511         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   242 (to 778)
    
-   510         294 LOAD_CONST               0 (0)
+   512         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   512         306 PUSH_NULL
+   514         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   514         326 PUSH_NULL
+   516         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawText)
                330 PRECALL                  0
                334 CALL                     0
                344 STORE_NAME              18 (text1)
    
-   515         346 LOAD_NAME               18 (text1)
+   517         346 LOAD_NAME               18 (text1)
                348 LOAD_METHOD             19 (pack)
                370 LOAD_CONST              23 ('x')
                372 LOAD_CONST              24 (5)
                374 LOAD_CONST              24 (5)
                376 KW_NAMES                25
                378 PRECALL                  3
                382 CALL                     3
                392 POP_TOP
    
-   517         394 PUSH_NULL
+   519         394 PUSH_NULL
                396 LOAD_NAME                7 (AdwDrawDarkText)
                398 PRECALL                  0
                402 CALL                     0
                412 STORE_NAME              20 (text2)
    
-   518         414 LOAD_NAME               20 (text2)
+   520         414 LOAD_NAME               20 (text2)
                416 LOAD_METHOD             19 (pack)
                438 LOAD_CONST              23 ('x')
                440 LOAD_CONST              24 (5)
                442 LOAD_CONST              24 (5)
                444 KW_NAMES                25
                446 PRECALL                  3
                450 CALL                     3
                460 POP_TOP
    
-   520         462 PUSH_NULL
+   522         462 PUSH_NULL
                464 LOAD_NAME                9 (AdwDrawRoundText)
                466 PRECALL                  0
                470 CALL                     0
                480 STORE_NAME              21 (text3)
    
-   521         482 LOAD_NAME               21 (text3)
+   523         482 LOAD_NAME               21 (text3)
                484 LOAD_METHOD             19 (pack)
                506 LOAD_CONST              23 ('x')
                508 LOAD_CONST              24 (5)
                510 LOAD_CONST              24 (5)
                512 KW_NAMES                25
                514 PRECALL                  3
                518 CALL                     3
                528 POP_TOP
    
-   523         530 PUSH_NULL
+   525         530 PUSH_NULL
                532 LOAD_NAME               10 (AdwDrawRoundDarkText)
                534 PRECALL                  0
                538 CALL                     0
                548 STORE_NAME              22 (text4)
    
-   524         550 LOAD_NAME               22 (text4)
+   526         550 LOAD_NAME               22 (text4)
                552 LOAD_METHOD             19 (pack)
                574 LOAD_CONST              23 ('x')
                576 LOAD_CONST              24 (5)
                578 LOAD_CONST              24 (5)
                580 KW_NAMES                25
                582 PRECALL                  3
                586 CALL                     3
                596 POP_TOP
    
-   526         598 PUSH_NULL
+   528         598 PUSH_NULL
                600 LOAD_NAME               12 (AdwDrawRoundText3)
                602 PRECALL                  0
                606 CALL                     0
                616 STORE_NAME              23 (text5)
    
-   527         618 LOAD_NAME               23 (text5)
+   529         618 LOAD_NAME               23 (text5)
                620 LOAD_METHOD             19 (pack)
                642 LOAD_CONST              23 ('x')
                644 LOAD_CONST              24 (5)
                646 LOAD_CONST              24 (5)
                648 KW_NAMES                25
                650 PRECALL                  3
                654 CALL                     3
                664 POP_TOP
    
-   529         666 PUSH_NULL
+   531         666 PUSH_NULL
                668 LOAD_NAME               13 (AdwDrawRoundDarkText3)
                670 PRECALL                  0
                674 CALL                     0
                684 STORE_NAME              24 (text6)
    
-   530         686 LOAD_NAME               24 (text6)
+   532         686 LOAD_NAME               24 (text6)
                688 LOAD_METHOD             19 (pack)
                710 LOAD_CONST              23 ('x')
                712 LOAD_CONST              24 (5)
                714 LOAD_CONST              24 (5)
                716 KW_NAMES                25
                718 PRECALL                  3
                722 CALL                     3
                732 POP_TOP
    
-   532         734 LOAD_NAME               17 (root)
+   534         734 LOAD_NAME               17 (root)
                736 LOAD_METHOD             25 (mainloop)
                758 PRECALL                  0
                762 CALL                     0
                772 POP_TOP
                774 LOAD_CONST              26 (None)
                776 RETURN_VALUE
    
-   509     >>  778 LOAD_CONST              26 (None)
+   511     >>  778 LOAD_CONST              26 (None)
                780 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
          nlocals   : 0
-         stacksize : 3
+         stacksize : 4
          flags     : 0
          code
-            0x8700970065005a0164005a026401640264039c02880066016404840a5a
-            03640584005a04640684005a05640784005a06640884005a07640984005a
-            08640a84005a09640b84005a0a640c84005a0b640d84005a0c640e84005a
-            0d640f84005a0e641084005a0f641184005a10641284005a11641384005a
-            126420641584015a136420641684015a146420641784015a156420641884
-            015a166420641984015a176420641a65186602641b84055a19641c84005a
-            1a641d84005a1b641e84005a1c6420641f84015a1d880078015a1e5300
+            0x8700970065005a0164005a0264016402640364049c0364056503660288
+            0066016406840e5a04640784005a05640884005a06640984005a07640a84
+            005a08640b84005a09640c84005a0a640d84005a0b640e84005a0c640f84
+            005a0d641084005a0e641184005a0f641284005a10641384005a11641484
+            005a12641584005a136422641784015a146422641884015a156422641984
+            015a166422641a84015a176422641b84015a186422641c65196602641d84
+            055a1a641e84005a1b641f84005a1c642084005a1d6422642184015a1e88
+            0078015a1f5300
                        0 MAKE_CELL                0 (__class__)
          
            6           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicText')
                       10 STORE_NAME               2 (__qualname__)
          
-           7          12 LOAD_CONST               1 (120)
-                      14 LOAD_CONST               2 (80)
-                      16 LOAD_CONST               3 (('width', 'height'))
-                      18 BUILD_CONST_KEY_MAP      2
-                      20 LOAD_CLOSURE             0 (__class__)
-                      22 BUILD_TUPLE              1
-                      24 LOAD_CONST               4 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 7>)
-                      26 MAKE_FUNCTION           10 (kwdefaults, closure)
-                      28 STORE_NAME               3 (__init__)
-         
-          48          30 LOAD_CONST               5 (<code object tbbox, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 48>)
-                      32 MAKE_FUNCTION            0
-                      34 STORE_NAME               4 (tbbox)
-         
-          51          36 LOAD_CONST               6 (<code object compare, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 51>)
-                      38 MAKE_FUNCTION            0
-                      40 STORE_NAME               5 (compare)
-         
-          54          42 LOAD_CONST               7 (<code object count, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 54>)
-                      44 MAKE_FUNCTION            0
-                      46 STORE_NAME               6 (count)
-         
-          57          48 LOAD_CONST               8 (<code object debug, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 57>)
-                      50 MAKE_FUNCTION            0
-                      52 STORE_NAME               7 (debug)
-         
-          60          54 LOAD_CONST               9 (<code object tdelete, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 60>)
-                      56 MAKE_FUNCTION            0
-                      58 STORE_NAME               8 (tdelete)
-         
-          63          60 LOAD_CONST              10 (<code object dump, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 63>)
-                      62 MAKE_FUNCTION            0
-                      64 STORE_NAME               9 (dump)
-         
-          66          66 LOAD_CONST              11 (<code object get, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 66>)
-                      68 MAKE_FUNCTION            0
-                      70 STORE_NAME              10 (get)
-         
-          69          72 LOAD_CONST              12 (<code object tindex, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 69>)
-                      74 MAKE_FUNCTION            0
-                      76 STORE_NAME              11 (tindex)
-         
-          72          78 LOAD_CONST              13 (<code object tinsert, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 72>)
-                      80 MAKE_FUNCTION            0
-                      82 STORE_NAME              12 (tinsert)
-         
-          75          84 LOAD_CONST              14 (<code object search, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 75>)
-                      86 MAKE_FUNCTION            0
-                      88 STORE_NAME              13 (search)
-         
-          78          90 LOAD_CONST              15 (<code object see, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 78>)
-                      92 MAKE_FUNCTION            0
-                      94 STORE_NAME              14 (see)
-         
-          81          96 LOAD_CONST              16 (<code object undo, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 81>)
-                      98 MAKE_FUNCTION            0
-                     100 STORE_NAME              15 (undo)
-         
-          87         102 LOAD_CONST              17 (<code object redo, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 87>)
-                     104 MAKE_FUNCTION            0
-                     106 STORE_NAME              16 (redo)
-         
-          93         108 LOAD_CONST              18 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 93>)
-                     110 MAKE_FUNCTION            0
-                     112 STORE_NAME              17 (_other)
-         
-          97         114 LOAD_CONST              19 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 97>)
-                     116 MAKE_FUNCTION            0
-                     118 STORE_NAME              18 (_draw)
-         
-         125         120 LOAD_CONST              32 ((None,))
-                     122 LOAD_CONST              21 (<code object _focus, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 125>)
-                     124 MAKE_FUNCTION            1 (defaults)
-                     126 STORE_NAME              19 (_focus)
+           7          12 LOAD_CONST               1 ('')
+                      14 LOAD_CONST               2 (120)
+                      16 LOAD_CONST               3 (80)
+                      18 LOAD_CONST               4 (('text', 'width', 'height'))
+                      20 BUILD_CONST_KEY_MAP      3
+                      22 LOAD_CONST               5 ('text')
+                      24 LOAD_NAME                3 (str)
+                      26 BUILD_TUPLE              2
+                      28 LOAD_CLOSURE             0 (__class__)
+                      30 BUILD_TUPLE              1
+                      32 LOAD_CONST               6 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 7>)
+                      34 MAKE_FUNCTION           14 (kwdefaults, annotations, closure)
+                      36 STORE_NAME               4 (__init__)
+         
+          50          38 LOAD_CONST               7 (<code object tbbox, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 50>)
+                      40 MAKE_FUNCTION            0
+                      42 STORE_NAME               5 (tbbox)
+         
+          53          44 LOAD_CONST               8 (<code object compare, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 53>)
+                      46 MAKE_FUNCTION            0
+                      48 STORE_NAME               6 (compare)
+         
+          56          50 LOAD_CONST               9 (<code object count, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 56>)
+                      52 MAKE_FUNCTION            0
+                      54 STORE_NAME               7 (count)
+         
+          59          56 LOAD_CONST              10 (<code object debug, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 59>)
+                      58 MAKE_FUNCTION            0
+                      60 STORE_NAME               8 (debug)
+         
+          62          62 LOAD_CONST              11 (<code object tdelete, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 62>)
+                      64 MAKE_FUNCTION            0
+                      66 STORE_NAME               9 (tdelete)
+         
+          65          68 LOAD_CONST              12 (<code object dump, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 65>)
+                      70 MAKE_FUNCTION            0
+                      72 STORE_NAME              10 (dump)
+         
+          68          74 LOAD_CONST              13 (<code object get, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 68>)
+                      76 MAKE_FUNCTION            0
+                      78 STORE_NAME              11 (get)
+         
+          71          80 LOAD_CONST              14 (<code object tindex, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 71>)
+                      82 MAKE_FUNCTION            0
+                      84 STORE_NAME              12 (tindex)
+         
+          74          86 LOAD_CONST              15 (<code object tinsert, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 74>)
+                      88 MAKE_FUNCTION            0
+                      90 STORE_NAME              13 (tinsert)
+         
+          77          92 LOAD_CONST              16 (<code object search, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 77>)
+                      94 MAKE_FUNCTION            0
+                      96 STORE_NAME              14 (search)
+         
+          80          98 LOAD_CONST              17 (<code object see, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 80>)
+                     100 MAKE_FUNCTION            0
+                     102 STORE_NAME              15 (see)
+         
+          83         104 LOAD_CONST              18 (<code object undo, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 83>)
+                     106 MAKE_FUNCTION            0
+                     108 STORE_NAME              16 (undo)
+         
+          89         110 LOAD_CONST              19 (<code object redo, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 89>)
+                     112 MAKE_FUNCTION            0
+                     114 STORE_NAME              17 (redo)
+         
+          95         116 LOAD_CONST              20 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 95>)
+                     118 MAKE_FUNCTION            0
+                     120 STORE_NAME              18 (_other)
+         
+          99         122 LOAD_CONST              21 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 99>)
+                     124 MAKE_FUNCTION            0
+                     126 STORE_NAME              19 (_draw)
          
-         134         128 LOAD_CONST              32 ((None,))
-                     130 LOAD_CONST              22 (<code object _focusout, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 134>)
+         127         128 LOAD_CONST              34 ((None,))
+                     130 LOAD_CONST              23 (<code object _focus, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 127>)
                      132 MAKE_FUNCTION            1 (defaults)
-                     134 STORE_NAME              20 (_focusout)
+                     134 STORE_NAME              20 (_focus)
          
-         143         136 LOAD_CONST              32 ((None,))
-                     138 LOAD_CONST              23 (<code object _click, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 143>)
+         136         136 LOAD_CONST              34 ((None,))
+                     138 LOAD_CONST              24 (<code object _focusout, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 136>)
                      140 MAKE_FUNCTION            1 (defaults)
-                     142 STORE_NAME              21 (_click)
+                     142 STORE_NAME              21 (_focusout)
          
-         146         144 LOAD_CONST              32 ((None,))
-                     146 LOAD_CONST              24 (<code object _hover, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 146>)
+         145         144 LOAD_CONST              34 ((None,))
+                     146 LOAD_CONST              25 (<code object _click, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 145>)
                      148 MAKE_FUNCTION            1 (defaults)
-                     150 STORE_NAME              22 (_hover)
+                     150 STORE_NAME              22 (_click)
          
-         149         152 LOAD_CONST              32 ((None,))
-                     154 LOAD_CONST              25 (<code object _hover_release, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 149>)
+         148         152 LOAD_CONST              34 ((None,))
+                     154 LOAD_CONST              26 (<code object _hover, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 148>)
                      156 MAKE_FUNCTION            1 (defaults)
-                     158 STORE_NAME              23 (_hover_release)
+                     158 STORE_NAME              23 (_hover)
          
-         160         160 LOAD_CONST              32 ((None,))
-                     162 LOAD_CONST              26 ('font')
-                     164 LOAD_NAME               24 (Font)
-                     166 BUILD_TUPLE              2
-                     168 LOAD_CONST              27 (<code object font, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 160>)
-                     170 MAKE_FUNCTION            5 (defaults, annotations)
-                     172 STORE_NAME              25 (font)
-         
-         166         174 LOAD_CONST              28 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 166>)
-                     176 MAKE_FUNCTION            0
-                     178 STORE_NAME              26 (default_palette)
-         
-         169         180 LOAD_CONST              29 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 169>)
-                     182 MAKE_FUNCTION            0
-                     184 STORE_NAME              27 (palette_light)
-         
-         196         186 LOAD_CONST              30 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 196>)
-                     188 MAKE_FUNCTION            0
-                     190 STORE_NAME              28 (palette_dark)
-         
-         223         192 LOAD_CONST              32 ((None,))
-                     194 LOAD_CONST              31 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 223>)
-                     196 MAKE_FUNCTION            1 (defaults)
-                     198 STORE_NAME              29 (palette)
-                     200 LOAD_CLOSURE             0 (__class__)
-                     202 COPY                     1
-                     204 STORE_NAME              30 (__classcell__)
-                     206 RETURN_VALUE
+         151         160 LOAD_CONST              34 ((None,))
+                     162 LOAD_CONST              27 (<code object _hover_release, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 151>)
+                     164 MAKE_FUNCTION            1 (defaults)
+                     166 STORE_NAME              24 (_hover_release)
+         
+         162         168 LOAD_CONST              34 ((None,))
+                     170 LOAD_CONST              28 ('font')
+                     172 LOAD_NAME               25 (Font)
+                     174 BUILD_TUPLE              2
+                     176 LOAD_CONST              29 (<code object font, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 162>)
+                     178 MAKE_FUNCTION            5 (defaults, annotations)
+                     180 STORE_NAME              26 (font)
+         
+         168         182 LOAD_CONST              30 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 168>)
+                     184 MAKE_FUNCTION            0
+                     186 STORE_NAME              27 (default_palette)
+         
+         171         188 LOAD_CONST              31 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 171>)
+                     190 MAKE_FUNCTION            0
+                     192 STORE_NAME              28 (palette_light)
+         
+         198         194 LOAD_CONST              32 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 198>)
+                     196 MAKE_FUNCTION            0
+                     198 STORE_NAME              29 (palette_dark)
+         
+         225         200 LOAD_CONST              34 ((None,))
+                     202 LOAD_CONST              33 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 225>)
+                     204 MAKE_FUNCTION            1 (defaults)
+                     206 STORE_NAME              30 (palette)
+                     208 LOAD_CLOSURE             0 (__class__)
+                     210 COPY                     1
+                     212 STORE_NAME              31 (__classcell__)
+                     214 RETURN_VALUE
          consts
             'AdwDrawBasicText'
+            ''
             120
             80
-            ('width', 'height')
+            ('text', 'width', 'height')
+            'text'
             code
                argcount  : 1
-               nlocals   : 6
+               nlocals   : 7
                stacksize : 7
                flags     : 15
                code
                   0x9501870097000200740100000000000000000000a6000000ab00000000
-                  00000000006a0100000000000000007c037c017c02640164029c037c04a4
-                  018e010100640164036c026d037d05010074090000000000000000000064
+                  00000000006a0100000000000000007c047c027c03640164029c037c05a4
+                  018e010100640164036c026d037d06010074090000000000000000000064
                   04a6010000ab01000000000000000089005f05000000000000000002007c
-                  058900640189006a05000000000000000064056401ac06a6050000ab0500
-                  0000000000000089005f0600000000000000008900a00700000000000000
-                  00000000000000000000000000a6000000ab000000000000000000010089
-                  00a0080000000000000000000000000000000000000000a6000000ab0000
-                  00000000000000010089006a09000000000000000089005f0a0000000000
-                  00000089006a0b000000000000000089005f0c000000000000000089006a
-                  0d000000000000000089005f0e000000000000000089006a0f0000000000
-                  00000089005f10000000000000000089006a11000000000000000089005f
-                  1200000000000000008900a0130000000000000000000000000000000000
-                  000000640789006a1400000000000000006408ac09a6030000ab03000000
-                  000000000001008900a01300000000000000000000000000000000000000
-                  00640a89006a1500000000000000006408ac09a6030000ab030000000000
-                  00000001008900a013000000000000000000000000000000000000000064
-                  0b89006a1600000000000000006408ac09a6030000ab0300000000000000
-                  0001008900a0130000000000000000000000000000000000000000640c89
-                  006a1700000000000000006408ac09a6030000ab03000000000000000001
-                  0089006a060000000000000000a013000000000000000000000000000000
-                  0000000000640d89006a1800000000000000006408ac09a6030000ab0300
-                  00000000000000010089006a060000000000000000a01300000000000000
-                  00000000000000000000000000640e89006a1900000000000000006408ac
-                  09a6030000ab03000000000000000001008900a013000000000000000000
-                  0000000000000000000000640f88006601641084086408ac09a6030000ab
-                  03000000000000000001008900a013000000000000000000000000000000
-                  0000000000641188006601641284086408ac09a6030000ab030000000000
-                  00000001008900a013000000000000000000000000000000000000000064
-                  1388006601641484086408ac09a6030000ab030000000000000000010089
-                  00a013000000000000000000000000000000000000000064158800660164
-                  1684086408ac09a6030000ab030000000000000000010089006a06000000
-                  0000000000a0130000000000000000000000000000000000000000640f88
-                  006601641784086408ac09a6030000ab030000000000000000010089006a
-                  060000000000000000a01300000000000000000000000000000000000000
-                  00641188006601641884086408ac09a6030000ab03000000000000000001
-                  0089006a060000000000000000a013000000000000000000000000000000
-                  0000000000641388006601641984086408ac09a6030000ab030000000000
-                  000000010089006a060000000000000000a0130000000000000000000000
-                  000000000000000000641588006601641a84086408ac09a6030000ab0300
-                  0000000000000001008900a0140000000000000000000000000000000000
-                  0000006400a6010000ab010000000000000000010064005300
+                  068900640189006a05000000000000000064056401ac06a6050000ab0500
+                  0000000000000089005f06000000000000000089006a0600000000000000
+                  00a007000000000000000000000000000000000000000064077c01a60200
+                  00ab02000000000000000001008900a00800000000000000000000000000
+                  00000000000000a6000000ab00000000000000000001008900a009000000
+                  0000000000000000000000000000000000a6000000ab0000000000000000
+                  00010089006a0a000000000000000089005f0b000000000000000089006a
+                  0c000000000000000089005f0d000000000000000089006a0e0000000000
+                  00000089005f0f000000000000000089006a10000000000000000089005f
+                  11000000000000000089006a12000000000000000089005f130000000000
+                  0000008900a0140000000000000000000000000000000000000000640889
+                  006a1500000000000000006409ac0aa6030000ab03000000000000000001
+                  008900a0140000000000000000000000000000000000000000640b89006a
+                  1600000000000000006409ac0aa6030000ab030000000000000000010089
+                  00a0140000000000000000000000000000000000000000640c89006a1700
+                  000000000000006409ac0aa6030000ab03000000000000000001008900a0
+                  140000000000000000000000000000000000000000640d89006a18000000
+                  00000000006409ac0aa6030000ab030000000000000000010089006a0600
+                  00000000000000a014000000000000000000000000000000000000000064
+                  0e89006a1900000000000000006409ac0aa6030000ab0300000000000000
+                  00010089006a060000000000000000a01400000000000000000000000000
+                  00000000000000640f89006a1a00000000000000006409ac0aa6030000ab
+                  03000000000000000001008900a014000000000000000000000000000000
+                  0000000000641088006601641184086409ac0aa6030000ab030000000000
+                  00000001008900a014000000000000000000000000000000000000000064
+                  1288006601641384086409ac0aa6030000ab030000000000000000010089
+                  00a014000000000000000000000000000000000000000064148800660164
+                  1584086409ac0aa6030000ab03000000000000000001008900a014000000
+                  0000000000000000000000000000000000641688006601641784086409ac
+                  0aa6030000ab030000000000000000010089006a060000000000000000a0
+                  140000000000000000000000000000000000000000641088006601641884
+                  086409ac0aa6030000ab030000000000000000010089006a060000000000
+                  000000a01400000000000000000000000000000000000000006412880066
+                  01641984086409ac0aa6030000ab030000000000000000010089006a0600
+                  00000000000000a014000000000000000000000000000000000000000064
+                  1488006601641a84086409ac0aa6030000ab030000000000000000010089
+                  006a060000000000000000a0140000000000000000000000000000000000
+                  000000641688006601641b84086409ac0aa6030000ab0300000000000000
+                  0001008900a01500000000000000000000000000000000000000006400a6
+                  010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
                  7           4 RESUME                   0
                
                  9           6 PUSH_NULL
                              8 LOAD_GLOBAL              1 (NULL + super)
                             20 PRECALL                  0
                             24 CALL                     0
                             34 LOAD_ATTR                1 (__init__)
-                            44 LOAD_FAST                3 (args)
-                            46 LOAD_FAST                1 (width)
-                            48 LOAD_FAST                2 (height)
+                            44 LOAD_FAST                4 (args)
+                            46 LOAD_FAST                2 (width)
+                            48 LOAD_FAST                3 (height)
                             50 LOAD_CONST               1 (0)
                             52 LOAD_CONST               2 (('width', 'height', 'highlightthickness'))
                             54 BUILD_CONST_KEY_MAP      3
-                            56 LOAD_FAST                4 (kwargs)
+                            56 LOAD_FAST                5 (kwargs)
                             58 DICT_MERGE               1
                             60 CALL_FUNCTION_EX         1
                             62 POP_TOP
                
                 11          64 LOAD_CONST               1 (0)
                             66 LOAD_CONST               3 (('Text',))
                             68 IMPORT_NAME              2 (tkinter)
                             70 IMPORT_FROM              3 (Text)
-                            72 STORE_FAST               5 (Text)
+                            72 STORE_FAST               6 (Text)
                             74 POP_TOP
                
                 13          76 LOAD_GLOBAL              9 (NULL + nametofont)
                             88 LOAD_CONST               4 ('TkDefaultFont')
                             90 PRECALL                  1
                             94 CALL                     1
                            104 LOAD_DEREF               0 (self)
                            106 STORE_ATTR               5 (text_text_font)
                
                 15         116 PUSH_NULL
-                           118 LOAD_FAST                5 (Text)
+                           118 LOAD_FAST                6 (Text)
                            120 LOAD_DEREF               0 (self)
                            122 LOAD_CONST               1 (0)
                            124 LOAD_DEREF               0 (self)
                            126 LOAD_ATTR                5 (text_text_font)
                            136 LOAD_CONST               5 (True)
                            138 LOAD_CONST               1 (0)
                            140 KW_NAMES                 6
                            142 PRECALL                  5
                            146 CALL                     5
                            156 LOAD_DEREF               0 (self)
                            158 STORE_ATTR               6 (text)
                
                 17         168 LOAD_DEREF               0 (self)
-                           170 LOAD_METHOD              7 (_other)
-                           192 PRECALL                  0
-                           196 CALL                     0
-                           206 POP_TOP
-               
-                19         208 LOAD_DEREF               0 (self)
-                           210 LOAD_METHOD              8 (default_palette)
-                           232 PRECALL                  0
-                           236 CALL                     0
-                           246 POP_TOP
-               
-                21         248 LOAD_DEREF               0 (self)
-                           250 LOAD_ATTR                9 (text_back)
-                           260 LOAD_DEREF               0 (self)
-                           262 STORE_ATTR              10 (_text_back)
-               
-                22         272 LOAD_DEREF               0 (self)
-                           274 LOAD_ATTR               11 (text_border)
-                           284 LOAD_DEREF               0 (self)
-                           286 STORE_ATTR              12 (_text_border)
-               
-                23         296 LOAD_DEREF               0 (self)
-                           298 LOAD_ATTR               13 (text_text_back)
-                           308 LOAD_DEREF               0 (self)
-                           310 STORE_ATTR              14 (_text_text_back)
-               
-                24         320 LOAD_DEREF               0 (self)
-                           322 LOAD_ATTR               15 (text_bottom_line)
-                           332 LOAD_DEREF               0 (self)
-                           334 STORE_ATTR              16 (_text_bottom_line)
-               
-                25         344 LOAD_DEREF               0 (self)
-                           346 LOAD_ATTR               17 (text_bottom_width)
-                           356 LOAD_DEREF               0 (self)
-                           358 STORE_ATTR              18 (_text_bottom_width)
-               
-                27         368 LOAD_DEREF               0 (self)
-                           370 LOAD_METHOD             19 (bind)
-                           392 LOAD_CONST               7 ('<Configure>')
-                           394 LOAD_DEREF               0 (self)
-                           396 LOAD_ATTR               20 (_draw)
-                           406 LOAD_CONST               8 ('+')
-                           408 KW_NAMES                 9
-                           410 PRECALL                  3
-                           414 CALL                     3
-                           424 POP_TOP
-               
-                28         426 LOAD_DEREF               0 (self)
-                           428 LOAD_METHOD             19 (bind)
-                           450 LOAD_CONST              10 ('<Button>')
-                           452 LOAD_DEREF               0 (self)
-                           454 LOAD_ATTR               21 (_click)
-                           464 LOAD_CONST               8 ('+')
-                           466 KW_NAMES                 9
-                           468 PRECALL                  3
-                           472 CALL                     3
-                           482 POP_TOP
-               
-                29         484 LOAD_DEREF               0 (self)
-                           486 LOAD_METHOD             19 (bind)
-                           508 LOAD_CONST              11 ('<Enter>')
-                           510 LOAD_DEREF               0 (self)
-                           512 LOAD_ATTR               22 (_hover)
-                           522 LOAD_CONST               8 ('+')
-                           524 KW_NAMES                 9
-                           526 PRECALL                  3
-                           530 CALL                     3
-                           540 POP_TOP
-               
-                30         542 LOAD_DEREF               0 (self)
-                           544 LOAD_METHOD             19 (bind)
-                           566 LOAD_CONST              12 ('<Leave>')
-                           568 LOAD_DEREF               0 (self)
-                           570 LOAD_ATTR               23 (_hover_release)
-                           580 LOAD_CONST               8 ('+')
-                           582 KW_NAMES                 9
-                           584 PRECALL                  3
-                           588 CALL                     3
-                           598 POP_TOP
-               
-                32         600 LOAD_DEREF               0 (self)
-                           602 LOAD_ATTR                6 (text)
-                           612 LOAD_METHOD             19 (bind)
-                           634 LOAD_CONST              13 ('<FocusIn>')
-                           636 LOAD_DEREF               0 (self)
-                           638 LOAD_ATTR               24 (_focus)
-                           648 LOAD_CONST               8 ('+')
-                           650 KW_NAMES                 9
-                           652 PRECALL                  3
-                           656 CALL                     3
-                           666 POP_TOP
-               
-                34         668 LOAD_DEREF               0 (self)
-                           670 LOAD_ATTR                6 (text)
-                           680 LOAD_METHOD             19 (bind)
-                           702 LOAD_CONST              14 ('<FocusOut>')
-                           704 LOAD_DEREF               0 (self)
-                           706 LOAD_ATTR               25 (_focusout)
-                           716 LOAD_CONST               8 ('+')
-                           718 KW_NAMES                 9
-                           720 PRECALL                  3
-                           724 CALL                     3
-                           734 POP_TOP
-               
-                36         736 LOAD_DEREF               0 (self)
-                           738 LOAD_METHOD             19 (bind)
-                           760 LOAD_CONST              15 ('<Control-z>')
-                           762 LOAD_CLOSURE             0 (self)
-                           764 BUILD_TUPLE              1
-                           766 LOAD_CONST              16 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 36>)
-                           768 MAKE_FUNCTION            8 (closure)
-                           770 LOAD_CONST               8 ('+')
-                           772 KW_NAMES                 9
+                           170 LOAD_ATTR                6 (text)
+                           180 LOAD_METHOD              7 (insert)
+                           202 LOAD_CONST               7 ('1.0')
+                           204 LOAD_FAST                1 (text)
+                           206 PRECALL                  2
+                           210 CALL                     2
+                           220 POP_TOP
+               
+                19         222 LOAD_DEREF               0 (self)
+                           224 LOAD_METHOD              8 (_other)
+                           246 PRECALL                  0
+                           250 CALL                     0
+                           260 POP_TOP
+               
+                21         262 LOAD_DEREF               0 (self)
+                           264 LOAD_METHOD              9 (default_palette)
+                           286 PRECALL                  0
+                           290 CALL                     0
+                           300 POP_TOP
+               
+                23         302 LOAD_DEREF               0 (self)
+                           304 LOAD_ATTR               10 (text_back)
+                           314 LOAD_DEREF               0 (self)
+                           316 STORE_ATTR              11 (_text_back)
+               
+                24         326 LOAD_DEREF               0 (self)
+                           328 LOAD_ATTR               12 (text_border)
+                           338 LOAD_DEREF               0 (self)
+                           340 STORE_ATTR              13 (_text_border)
+               
+                25         350 LOAD_DEREF               0 (self)
+                           352 LOAD_ATTR               14 (text_text_back)
+                           362 LOAD_DEREF               0 (self)
+                           364 STORE_ATTR              15 (_text_text_back)
+               
+                26         374 LOAD_DEREF               0 (self)
+                           376 LOAD_ATTR               16 (text_bottom_line)
+                           386 LOAD_DEREF               0 (self)
+                           388 STORE_ATTR              17 (_text_bottom_line)
+               
+                27         398 LOAD_DEREF               0 (self)
+                           400 LOAD_ATTR               18 (text_bottom_width)
+                           410 LOAD_DEREF               0 (self)
+                           412 STORE_ATTR              19 (_text_bottom_width)
+               
+                29         422 LOAD_DEREF               0 (self)
+                           424 LOAD_METHOD             20 (bind)
+                           446 LOAD_CONST               8 ('<Configure>')
+                           448 LOAD_DEREF               0 (self)
+                           450 LOAD_ATTR               21 (_draw)
+                           460 LOAD_CONST               9 ('+')
+                           462 KW_NAMES                10
+                           464 PRECALL                  3
+                           468 CALL                     3
+                           478 POP_TOP
+               
+                30         480 LOAD_DEREF               0 (self)
+                           482 LOAD_METHOD             20 (bind)
+                           504 LOAD_CONST              11 ('<Button>')
+                           506 LOAD_DEREF               0 (self)
+                           508 LOAD_ATTR               22 (_click)
+                           518 LOAD_CONST               9 ('+')
+                           520 KW_NAMES                10
+                           522 PRECALL                  3
+                           526 CALL                     3
+                           536 POP_TOP
+               
+                31         538 LOAD_DEREF               0 (self)
+                           540 LOAD_METHOD             20 (bind)
+                           562 LOAD_CONST              12 ('<Enter>')
+                           564 LOAD_DEREF               0 (self)
+                           566 LOAD_ATTR               23 (_hover)
+                           576 LOAD_CONST               9 ('+')
+                           578 KW_NAMES                10
+                           580 PRECALL                  3
+                           584 CALL                     3
+                           594 POP_TOP
+               
+                32         596 LOAD_DEREF               0 (self)
+                           598 LOAD_METHOD             20 (bind)
+                           620 LOAD_CONST              13 ('<Leave>')
+                           622 LOAD_DEREF               0 (self)
+                           624 LOAD_ATTR               24 (_hover_release)
+                           634 LOAD_CONST               9 ('+')
+                           636 KW_NAMES                10
+                           638 PRECALL                  3
+                           642 CALL                     3
+                           652 POP_TOP
+               
+                34         654 LOAD_DEREF               0 (self)
+                           656 LOAD_ATTR                6 (text)
+                           666 LOAD_METHOD             20 (bind)
+                           688 LOAD_CONST              14 ('<FocusIn>')
+                           690 LOAD_DEREF               0 (self)
+                           692 LOAD_ATTR               25 (_focus)
+                           702 LOAD_CONST               9 ('+')
+                           704 KW_NAMES                10
+                           706 PRECALL                  3
+                           710 CALL                     3
+                           720 POP_TOP
+               
+                36         722 LOAD_DEREF               0 (self)
+                           724 LOAD_ATTR                6 (text)
+                           734 LOAD_METHOD             20 (bind)
+                           756 LOAD_CONST              15 ('<FocusOut>')
+                           758 LOAD_DEREF               0 (self)
+                           760 LOAD_ATTR               26 (_focusout)
+                           770 LOAD_CONST               9 ('+')
+                           772 KW_NAMES                10
                            774 PRECALL                  3
                            778 CALL                     3
                            788 POP_TOP
                
-                37         790 LOAD_DEREF               0 (self)
-                           792 LOAD_METHOD             19 (bind)
-                           814 LOAD_CONST              17 ('<Control-Z>')
+                38         790 LOAD_DEREF               0 (self)
+                           792 LOAD_METHOD             20 (bind)
+                           814 LOAD_CONST              16 ('<Control-z>')
                            816 LOAD_CLOSURE             0 (self)
                            818 BUILD_TUPLE              1
-                           820 LOAD_CONST              18 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 37>)
+                           820 LOAD_CONST              17 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 38>)
                            822 MAKE_FUNCTION            8 (closure)
-                           824 LOAD_CONST               8 ('+')
-                           826 KW_NAMES                 9
+                           824 LOAD_CONST               9 ('+')
+                           826 KW_NAMES                10
                            828 PRECALL                  3
                            832 CALL                     3
                            842 POP_TOP
                
-                38         844 LOAD_DEREF               0 (self)
-                           846 LOAD_METHOD             19 (bind)
-                           868 LOAD_CONST              19 ('<Control-Shift-z>')
+                39         844 LOAD_DEREF               0 (self)
+                           846 LOAD_METHOD             20 (bind)
+                           868 LOAD_CONST              18 ('<Control-Z>')
                            870 LOAD_CLOSURE             0 (self)
                            872 BUILD_TUPLE              1
-                           874 LOAD_CONST              20 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 38>)
+                           874 LOAD_CONST              19 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 39>)
                            876 MAKE_FUNCTION            8 (closure)
-                           878 LOAD_CONST               8 ('+')
-                           880 KW_NAMES                 9
+                           878 LOAD_CONST               9 ('+')
+                           880 KW_NAMES                10
                            882 PRECALL                  3
                            886 CALL                     3
                            896 POP_TOP
                
-                39         898 LOAD_DEREF               0 (self)
-                           900 LOAD_METHOD             19 (bind)
-                           922 LOAD_CONST              21 ('<Control-Shift-Z>')
+                40         898 LOAD_DEREF               0 (self)
+                           900 LOAD_METHOD             20 (bind)
+                           922 LOAD_CONST              20 ('<Control-Shift-z>')
                            924 LOAD_CLOSURE             0 (self)
                            926 BUILD_TUPLE              1
-                           928 LOAD_CONST              22 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 39>)
+                           928 LOAD_CONST              21 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 40>)
                            930 MAKE_FUNCTION            8 (closure)
-                           932 LOAD_CONST               8 ('+')
-                           934 KW_NAMES                 9
+                           932 LOAD_CONST               9 ('+')
+                           934 KW_NAMES                10
                            936 PRECALL                  3
                            940 CALL                     3
                            950 POP_TOP
                
                 41         952 LOAD_DEREF               0 (self)
-                           954 LOAD_ATTR                6 (text)
-                           964 LOAD_METHOD             19 (bind)
-                           986 LOAD_CONST              15 ('<Control-z>')
-                           988 LOAD_CLOSURE             0 (self)
-                           990 BUILD_TUPLE              1
-                           992 LOAD_CONST              23 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 41>)
-                           994 MAKE_FUNCTION            8 (closure)
-                           996 LOAD_CONST               8 ('+')
-                           998 KW_NAMES                 9
-                          1000 PRECALL                  3
-                          1004 CALL                     3
-                          1014 POP_TOP
-               
-                42        1016 LOAD_DEREF               0 (self)
-                          1018 LOAD_ATTR                6 (text)
-                          1028 LOAD_METHOD             19 (bind)
-                          1050 LOAD_CONST              17 ('<Control-Z>')
-                          1052 LOAD_CLOSURE             0 (self)
-                          1054 BUILD_TUPLE              1
-                          1056 LOAD_CONST              24 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 42>)
-                          1058 MAKE_FUNCTION            8 (closure)
-                          1060 LOAD_CONST               8 ('+')
-                          1062 KW_NAMES                 9
-                          1064 PRECALL                  3
-                          1068 CALL                     3
-                          1078 POP_TOP
-               
-                43        1080 LOAD_DEREF               0 (self)
-                          1082 LOAD_ATTR                6 (text)
-                          1092 LOAD_METHOD             19 (bind)
-                          1114 LOAD_CONST              19 ('<Control-Shift-z>')
-                          1116 LOAD_CLOSURE             0 (self)
-                          1118 BUILD_TUPLE              1
-                          1120 LOAD_CONST              25 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 43>)
-                          1122 MAKE_FUNCTION            8 (closure)
-                          1124 LOAD_CONST               8 ('+')
-                          1126 KW_NAMES                 9
-                          1128 PRECALL                  3
-                          1132 CALL                     3
-                          1142 POP_TOP
-               
-                44        1144 LOAD_DEREF               0 (self)
-                          1146 LOAD_ATTR                6 (text)
-                          1156 LOAD_METHOD             19 (bind)
-                          1178 LOAD_CONST              21 ('<Control-Shift-Z>')
-                          1180 LOAD_CLOSURE             0 (self)
-                          1182 BUILD_TUPLE              1
-                          1184 LOAD_CONST              26 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 44>)
-                          1186 MAKE_FUNCTION            8 (closure)
-                          1188 LOAD_CONST               8 ('+')
-                          1190 KW_NAMES                 9
-                          1192 PRECALL                  3
-                          1196 CALL                     3
-                          1206 POP_TOP
-               
-                46        1208 LOAD_DEREF               0 (self)
-                          1210 LOAD_METHOD             20 (_draw)
-                          1232 LOAD_CONST               0 (None)
-                          1234 PRECALL                  1
-                          1238 CALL                     1
-                          1248 POP_TOP
-                          1250 LOAD_CONST               0 (None)
-                          1252 RETURN_VALUE
+                           954 LOAD_METHOD             20 (bind)
+                           976 LOAD_CONST              22 ('<Control-Shift-Z>')
+                           978 LOAD_CLOSURE             0 (self)
+                           980 BUILD_TUPLE              1
+                           982 LOAD_CONST              23 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 41>)
+                           984 MAKE_FUNCTION            8 (closure)
+                           986 LOAD_CONST               9 ('+')
+                           988 KW_NAMES                10
+                           990 PRECALL                  3
+                           994 CALL                     3
+                          1004 POP_TOP
+               
+                43        1006 LOAD_DEREF               0 (self)
+                          1008 LOAD_ATTR                6 (text)
+                          1018 LOAD_METHOD             20 (bind)
+                          1040 LOAD_CONST              16 ('<Control-z>')
+                          1042 LOAD_CLOSURE             0 (self)
+                          1044 BUILD_TUPLE              1
+                          1046 LOAD_CONST              24 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 43>)
+                          1048 MAKE_FUNCTION            8 (closure)
+                          1050 LOAD_CONST               9 ('+')
+                          1052 KW_NAMES                10
+                          1054 PRECALL                  3
+                          1058 CALL                     3
+                          1068 POP_TOP
+               
+                44        1070 LOAD_DEREF               0 (self)
+                          1072 LOAD_ATTR                6 (text)
+                          1082 LOAD_METHOD             20 (bind)
+                          1104 LOAD_CONST              18 ('<Control-Z>')
+                          1106 LOAD_CLOSURE             0 (self)
+                          1108 BUILD_TUPLE              1
+                          1110 LOAD_CONST              25 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 44>)
+                          1112 MAKE_FUNCTION            8 (closure)
+                          1114 LOAD_CONST               9 ('+')
+                          1116 KW_NAMES                10
+                          1118 PRECALL                  3
+                          1122 CALL                     3
+                          1132 POP_TOP
+               
+                45        1134 LOAD_DEREF               0 (self)
+                          1136 LOAD_ATTR                6 (text)
+                          1146 LOAD_METHOD             20 (bind)
+                          1168 LOAD_CONST              20 ('<Control-Shift-z>')
+                          1170 LOAD_CLOSURE             0 (self)
+                          1172 BUILD_TUPLE              1
+                          1174 LOAD_CONST              26 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 45>)
+                          1176 MAKE_FUNCTION            8 (closure)
+                          1178 LOAD_CONST               9 ('+')
+                          1180 KW_NAMES                10
+                          1182 PRECALL                  3
+                          1186 CALL                     3
+                          1196 POP_TOP
+               
+                46        1198 LOAD_DEREF               0 (self)
+                          1200 LOAD_ATTR                6 (text)
+                          1210 LOAD_METHOD             20 (bind)
+                          1232 LOAD_CONST              22 ('<Control-Shift-Z>')
+                          1234 LOAD_CLOSURE             0 (self)
+                          1236 BUILD_TUPLE              1
+                          1238 LOAD_CONST              27 (<code object <lambda>, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 46>)
+                          1240 MAKE_FUNCTION            8 (closure)
+                          1242 LOAD_CONST               9 ('+')
+                          1244 KW_NAMES                10
+                          1246 PRECALL                  3
+                          1250 CALL                     3
+                          1260 POP_TOP
+               
+                48        1262 LOAD_DEREF               0 (self)
+                          1264 LOAD_METHOD             21 (_draw)
+                          1286 LOAD_CONST               0 (None)
+                          1288 PRECALL                  1
+                          1292 CALL                     1
+                          1302 POP_TOP
+                          1304 LOAD_CONST               0 (None)
+                          1306 RETURN_VALUE
                consts
                   None
                   0
                   ('width', 'height', 'highlightthickness')
                   ('Text',)
                   'TkDefaultFont'
                   True
                   ('bd', 'font', 'undo', 'highlightthickness')
+                  '1.0'
                   '<Configure>'
                   '+'
                   ('add',)
                   '<Button>'
                   '<Enter>'
                   '<Leave>'
                   '<FocusIn>'
@@ -760,236 +779,236 @@
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      36           2 RESUME                   0
+                      38           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (undo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('undo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 36
+                     firstlineno 38
                      lnotab 0x
                   '<Control-Z>'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      37           2 RESUME                   0
+                      39           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (undo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('undo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 37
+                     firstlineno 39
                      lnotab 0x
                   '<Control-Shift-z>'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      38           2 RESUME                   0
+                      40           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (redo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('redo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 38
+                     firstlineno 40
                      lnotab 0x
                   '<Control-Shift-Z>'
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      39           2 RESUME                   0
+                      41           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (redo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('redo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 39
+                     firstlineno 41
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      41           2 RESUME                   0
+                      43           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (undo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('undo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 41
+                     firstlineno 43
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      42           2 RESUME                   0
+                      44           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (undo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('undo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 42
+                     firstlineno 44
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      43           2 RESUME                   0
+                      45           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (redo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('redo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 43
+                     firstlineno 45
                      lnotab 0x
                   code
                      argcount  : 1
                      nlocals   : 1
                      stacksize : 2
                      flags     : 19
                      code
                         0x950197008901a0000000000000000000000000000000000000000000a6
                         000000ab0000000000000000005300
                                    0 COPY_FREE_VARS           1
                      
-                      44           2 RESUME                   0
+                      46           2 RESUME                   0
                                    4 LOAD_DEREF               1 (self)
                                    6 LOAD_METHOD              0 (redo)
                                   28 PRECALL                  0
                                   32 CALL                     0
                                   42 RETURN_VALUE
                      consts
                         None
                      names      ('redo',)
                      varnames   ('event',)
                      freevars   ('self',)
                      cellvars   ()
                      filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                      name       '<lambda>'
-                     firstlineno 44
+                     firstlineno 46
                      lnotab 0x
-               names      ('super', '__init__', 'tkinter', 'Text', 'nametofont', 'text_text_font', 'text', '_other', 'default_palette', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', 'bind', '_draw', '_click', '_hover', '_hover_release', '_focus', '_focusout')
-               varnames   ('self', 'width', 'height', 'args', 'kwargs', 'Text')
+               names      ('super', '__init__', 'tkinter', 'Text', 'nametofont', 'text_text_font', 'text', 'insert', '_other', 'default_palette', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', 'bind', '_draw', '_click', '_hover', '_hover_release', '_focus', '_focusout')
+               varnames   ('self', 'text', 'width', 'height', 'args', 'kwargs', 'Text')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x06023a020c022802340228022802180118011801180118023a013a013a
-                  013a024402440236013601360136024001400140014002
+                  0x06023a020c0228023402360228022802180118011801180118023a013a
+                  013a013a024402440236013601360136024001400140014002
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                48           0 RESUME                   0
+                50           0 RESUME                   0
                
-                49           2 PUSH_NULL
+                51           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (bbox)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -999,27 +1018,27 @@
                   None
                names      ('text', 'bbox')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'tbbox'
-               firstlineno 48
+               firstlineno 50
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                51           0 RESUME                   0
+                53           0 RESUME                   0
                
-                52           2 PUSH_NULL
+                54           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (compare)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1029,27 +1048,27 @@
                   None
                names      ('text', 'compare')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'compare'
-               firstlineno 51
+               firstlineno 53
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                54           0 RESUME                   0
+                56           0 RESUME                   0
                
-                55           2 PUSH_NULL
+                57           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (count)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1059,27 +1078,27 @@
                   None
                names      ('text', 'count')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'count'
-               firstlineno 54
+               firstlineno 56
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                57           0 RESUME                   0
+                59           0 RESUME                   0
                
-                58           2 PUSH_NULL
+                60           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (debug)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1089,27 +1108,27 @@
                   None
                names      ('text', 'debug')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'debug'
-               firstlineno 57
+               firstlineno 59
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                60           0 RESUME                   0
+                62           0 RESUME                   0
                
-                61           2 PUSH_NULL
+                63           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (delete)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1119,27 +1138,27 @@
                   None
                names      ('text', 'delete')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'tdelete'
-               firstlineno 60
+               firstlineno 62
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                63           0 RESUME                   0
+                65           0 RESUME                   0
                
-                64           2 PUSH_NULL
+                66           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (dump)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1149,27 +1168,27 @@
                   None
                names      ('text', 'dump')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'dump'
-               firstlineno 63
+               firstlineno 65
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                66           0 RESUME                   0
+                68           0 RESUME                   0
                
-                67           2 PUSH_NULL
+                69           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (get)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1179,27 +1198,27 @@
                   None
                names      ('text', 'get')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'get'
-               firstlineno 66
+               firstlineno 68
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                69           0 RESUME                   0
+                71           0 RESUME                   0
                
-                70           2 PUSH_NULL
+                72           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (index)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1209,27 +1228,27 @@
                   None
                names      ('text', 'index')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'tindex'
-               firstlineno 69
+               firstlineno 71
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                72           0 RESUME                   0
+                74           0 RESUME                   0
                
-                73           2 PUSH_NULL
+                75           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (insert)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1239,27 +1258,27 @@
                   None
                names      ('text', 'insert')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'tinsert'
-               firstlineno 72
+               firstlineno 74
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                75           0 RESUME                   0
+                77           0 RESUME                   0
                
-                76           2 PUSH_NULL
+                78           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (search)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1269,27 +1288,27 @@
                   None
                names      ('text', 'search')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'search'
-               firstlineno 75
+               firstlineno 77
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x970002007c006a0000000000000000006a0100000000000000007c0169
                   007c02a4018e015300
-                78           0 RESUME                   0
+                80           0 RESUME                   0
                
-                79           2 PUSH_NULL
+                81           2 PUSH_NULL
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_ATTR                1 (see)
                             26 LOAD_FAST                1 (args)
                             28 BUILD_MAP                0
                             30 LOAD_FAST                2 (kwargs)
                             32 DICT_MERGE               1
@@ -1299,42 +1318,42 @@
                   None
                names      ('text', 'see')
                varnames   ('self', 'args', 'kwargs')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'see'
-               firstlineno 78
+               firstlineno 80
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009007c006a000000000000000000a0010000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006400530023
                   000100590064005300780359007701
-                81           0 RESUME                   0
+                83           0 RESUME                   0
                
-                82           2 NOP
+                84           2 NOP
                
-                83           4 LOAD_FAST                0 (self)
+                85           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_METHOD              1 (edit_undo)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                        >>   58 PUSH_EXC_INFO
                
-                84          60 POP_TOP
+                86          60 POP_TOP
                
-                85          62 POP_EXCEPT
+                87          62 POP_EXCEPT
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                        >>   68 COPY                     3
                             70 POP_EXCEPT
                             72 RERAISE                  1
                ExceptionTable:
                  4 to 52 -> 58 [0]
@@ -1343,42 +1362,42 @@
                   None
                names      ('text', 'edit_undo')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'undo'
-               firstlineno 81
+               firstlineno 83
                lnotab 0x0201020138010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009007c006a000000000000000000a0010000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006400530023
                   000100590064005300780359007701
-                87           0 RESUME                   0
+                89           0 RESUME                   0
                
-                88           2 NOP
+                90           2 NOP
                
-                89           4 LOAD_FAST                0 (self)
+                91           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_METHOD              1 (edit_redo)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                        >>   58 PUSH_EXC_INFO
                
-                90          60 POP_TOP
+                92          60 POP_TOP
                
-                91          62 POP_EXCEPT
+                93          62 POP_EXCEPT
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                        >>   68 COPY                     3
                             70 POP_EXCEPT
                             72 RERAISE                  1
                ExceptionTable:
                  4 to 52 -> 58 [0]
@@ -1387,61 +1406,61 @@
                   None
                names      ('text', 'edit_redo')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'redo'
-               firstlineno 87
+               firstlineno 89
                lnotab 0x0201020138010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-                93           0 RESUME                   0
+                95           0 RESUME                   0
                
-                94           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                96           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-                95          34 LOAD_FAST                0 (self)
+                97          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-                94     >>   94 LOAD_CONST               0 (None)
+                96     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 93
+               firstlineno 95
                lnotab 0x020120013cff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -1475,174 +1494,174 @@
                   00000000000000000000000000000000007c006a0e0000000000000000a6
                   010000ab01000000000000000001007c00a00f0000000000000000000000
                   0000000000000000007c006a0e00000000000000007c006a0b0000000000
                   000000a6020000ab02000000000000000001007c006a0a00000000000000
                   00a01000000000000000000000000000000000000000007c006a06000000
                   00000000007c006a11000000000000000064097c006a1100000000000000
                   00ac0aa6040000ab040000000000000000010064005300
-                97           0 RESUME                   0
+                99           0 RESUME                   0
                
-                98           2 LOAD_FAST                0 (self)
+               100           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               100          44 LOAD_FAST                0 (self)
+               102          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-               101          68 LOAD_CONST               2 (0)
+               103          68 LOAD_CONST               2 (0)
                             70 LOAD_CONST               2 (0)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               102         160 LOAD_FAST                0 (self)
+               104         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_border_width)
                
-               103         172 LOAD_FAST                0 (self)
+               105         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_text_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_back)
                
-               100         196 KW_NAMES                 4
+               102         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (text_frame)
                
-               106         224 LOAD_FAST                0 (self)
+               108         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_window)
                
-               107         248 LOAD_FAST                0 (self)
+               109         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-               108         336 LOAD_FAST                0 (self)
+               110         336 LOAD_FAST                0 (self)
                            338 LOAD_METHOD              2 (winfo_width)
                            360 PRECALL                  0
                            364 CALL                     0
                            374 LOAD_FAST                0 (self)
                            376 LOAD_ATTR                4 (text_border_width)
                            386 BINARY_OP               10 (-)
                            390 LOAD_CONST               6 (5)
                            392 BINARY_OP               10 (-)
                            396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR                9 (text_padding)
                            408 LOAD_CONST               2 (0)
                            410 BINARY_SUBSCR
                            420 BINARY_OP               10 (-)
                
-               109         424 LOAD_FAST                0 (self)
+               111         424 LOAD_FAST                0 (self)
                            426 LOAD_METHOD              3 (winfo_height)
                            448 PRECALL                  0
                            452 CALL                     0
                            462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                4 (text_border_width)
                            474 BINARY_OP               10 (-)
                            478 LOAD_CONST               6 (5)
                            480 BINARY_OP               10 (-)
                            484 LOAD_FAST                0 (self)
                            486 LOAD_ATTR                9 (text_padding)
                            496 LOAD_CONST               3 (1)
                            498 BINARY_SUBSCR
                            508 BINARY_OP               10 (-)
                
-               110         512 LOAD_FAST                0 (self)
+               112         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR               10 (text)
                
-               106         524 KW_NAMES                 7
+               108         524 KW_NAMES                 7
                            526 PRECALL                  5
                            530 CALL                     5
                            540 LOAD_FAST                0 (self)
                            542 STORE_ATTR              11 (text_text)
                
-               113         552 LOAD_FAST                0 (self)
+               115         552 LOAD_FAST                0 (self)
                            554 LOAD_METHOD              1 (create_rectangle)
                            576 LOAD_CONST               3 (1)
                            578 LOAD_FAST                0 (self)
                            580 LOAD_METHOD              3 (winfo_height)
                            602 PRECALL                  0
                            606 CALL                     0
                            616 LOAD_FAST                0 (self)
                            618 LOAD_ATTR               12 (_text_bottom_width)
                            628 BINARY_OP               10 (-)
                            632 LOAD_CONST               3 (1)
                            634 BINARY_OP               10 (-)
                
-               114         638 LOAD_FAST                0 (self)
+               116         638 LOAD_FAST                0 (self)
                            640 LOAD_METHOD              2 (winfo_width)
                            662 PRECALL                  0
                            666 CALL                     0
                            676 LOAD_CONST               3 (1)
                            678 BINARY_OP               10 (-)
                            682 LOAD_FAST                0 (self)
                            684 LOAD_METHOD              3 (winfo_height)
                            706 PRECALL                  0
                            710 CALL                     0
                            720 LOAD_CONST               3 (1)
                            722 BINARY_OP               10 (-)
                
-               115         726 LOAD_FAST                0 (self)
+               117         726 LOAD_FAST                0 (self)
                            728 LOAD_ATTR               13 (_text_bottom_line)
                            738 LOAD_FAST                0 (self)
                            740 LOAD_ATTR               13 (_text_bottom_line)
                
-               116         750 LOAD_CONST               2 (0)
+               118         750 LOAD_CONST               2 (0)
                
-               113         752 KW_NAMES                 8
+               115         752 KW_NAMES                 8
                            754 PRECALL                  7
                            758 CALL                     7
                            768 LOAD_FAST                0 (self)
                            770 STORE_ATTR              14 (text_bottom)
                
-               118         780 LOAD_FAST                0 (self)
+               120         780 LOAD_FAST                0 (self)
                            782 LOAD_ATTR               12 (_text_bottom_width)
                            792 LOAD_CONST               2 (0)
                            794 COMPARE_OP               2 (==)
                            800 POP_JUMP_FORWARD_IF_FALSE    26 (to 854)
                
-               119         802 LOAD_FAST                0 (self)
+               121         802 LOAD_FAST                0 (self)
                            804 LOAD_METHOD              0 (delete)
                            826 LOAD_FAST                0 (self)
                            828 LOAD_ATTR               14 (text_bottom)
                            838 PRECALL                  1
                            842 CALL                     1
                            852 POP_TOP
                
-               121     >>  854 LOAD_FAST                0 (self)
+               123     >>  854 LOAD_FAST                0 (self)
                            856 LOAD_METHOD             15 (tag_raise)
                            878 LOAD_FAST                0 (self)
                            880 LOAD_ATTR               14 (text_bottom)
                            890 LOAD_FAST                0 (self)
                            892 LOAD_ATTR               11 (text_text)
                            902 PRECALL                  2
                            906 CALL                     2
                            916 POP_TOP
                
-               123         918 LOAD_FAST                0 (self)
+               125         918 LOAD_FAST                0 (self)
                            920 LOAD_ATTR               10 (text)
                            930 LOAD_METHOD             16 (configure)
                            952 LOAD_FAST                0 (self)
                            954 LOAD_ATTR                6 (_text_back)
                            964 LOAD_FAST                0 (self)
                            966 LOAD_ATTR               17 (_text_text_back)
                            976 LOAD_CONST               9 (True)
@@ -1668,15 +1687,15 @@
                   ('background', 'foreground', 'autoseparators', 'insertbackground')
                names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 97
+               firstlineno 99
                lnotab
                   0x02012a0218015c010c0118fd1c0618015801580158010cfc1c07560158
                   01180102fd1c05160134024002
             None
             code
                argcount  : 2
                nlocals   : 2
@@ -1685,42 +1704,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               125           0 RESUME                   0
+               127           0 RESUME                   0
                
-               126           2 LOAD_FAST                0 (self)
+               128           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               127          26 LOAD_FAST                0 (self)
+               129          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               128          50 LOAD_FAST                0 (self)
+               130          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               129          74 LOAD_FAST                0 (self)
+               131          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               130          98 LOAD_FAST                0 (self)
+               132          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               132         122 LOAD_FAST                0 (self)
+               134         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1728,56 +1747,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 125
+               firstlineno 127
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               134           0 RESUME                   0
+               136           0 RESUME                   0
                
-               135           2 LOAD_FAST                0 (self)
+               137           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               136          26 LOAD_FAST                0 (self)
+               138          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               137          50 LOAD_FAST                0 (self)
+               139          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               138          74 LOAD_FAST                0 (self)
+               140          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               139          98 LOAD_FAST                0 (self)
+               141          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               141         122 LOAD_FAST                0 (self)
+               143         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1785,66 +1804,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 134
+               firstlineno 136
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               143           0 RESUME                   0
+               145           0 RESUME                   0
                
-               144           2 LOAD_FAST                0 (self)
+               146           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 143
+               firstlineno 145
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               146           0 RESUME                   0
+               148           0 RESUME                   0
                
-               147           2 LOAD_CONST               1 (True)
+               149           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 146
+               firstlineno 148
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -1852,184 +1871,184 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               149           0 RESUME                   0
+               151           0 RESUME                   0
                
-               150           2 LOAD_FAST                0 (self)
+               152           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               151          42 LOAD_CONST               1 (False)
+               153          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               152          56 LOAD_FAST                0 (self)
+               154          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               153          80 LOAD_FAST                0 (self)
+               155          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               154         104 LOAD_FAST                0 (self)
+               156         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               155         128 LOAD_FAST                0 (self)
+               157         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               156         152 LOAD_FAST                0 (self)
+               158         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               158         176 LOAD_FAST                0 (self)
+               160         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               150     >>  222 LOAD_CONST               0 (None)
+               152     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 149
+               firstlineno 151
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               160           0 RESUME                   0
+               162           0 RESUME                   0
                
-               161           2 LOAD_FAST                1 (font)
+               163           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               162           6 LOAD_FAST                0 (self)
+               164           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               164     >>   20 LOAD_FAST                1 (font)
+               166     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'font'
-               firstlineno 160
+               firstlineno 162
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               166           0 RESUME                   0
+               168           0 RESUME                   0
                
-               167           2 LOAD_FAST                0 (self)
+               169           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 166
+               firstlineno 168
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066404640764086409640a6406640b640c640d9c0664
                   0e9c086901a6010000ab010000000000000000010064005300
-               169           0 RESUME                   0
+               171           0 RESUME                   0
                
-               170           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               172          26 LOAD_CONST               1 ('text')
+               174          26 LOAD_CONST               1 ('text')
                
-               173          28 LOAD_CONST               2 ((3, 4))
+               175          28 LOAD_CONST               2 ((3, 4))
                
-               175          30 LOAD_CONST               3 ('#fdfdfd')
+               177          30 LOAD_CONST               3 ('#fdfdfd')
                
-               176          32 LOAD_CONST               4 ('#eaeaea')
+               178          32 LOAD_CONST               4 ('#eaeaea')
                
-               177          34 LOAD_CONST               5 ('#5f5f5f')
+               179          34 LOAD_CONST               5 ('#5f5f5f')
                
-               178          36 LOAD_CONST               6 (1)
+               180          36 LOAD_CONST               6 (1)
                
-               180          38 LOAD_CONST               4 ('#eaeaea')
+               182          38 LOAD_CONST               4 ('#eaeaea')
                
-               181          40 LOAD_CONST               7 (0)
+               183          40 LOAD_CONST               7 (0)
                
-               184          42 LOAD_CONST               8 ('#f9f9f9')
+               186          42 LOAD_CONST               8 ('#f9f9f9')
                
-               185          44 LOAD_CONST               9 ('#e2e2e2')
+               187          44 LOAD_CONST               9 ('#e2e2e2')
                
-               186          46 LOAD_CONST              10 ('#1a1a1a')
+               188          46 LOAD_CONST              10 ('#1a1a1a')
                
-               187          48 LOAD_CONST               6 (1)
+               189          48 LOAD_CONST               6 (1)
                
-               189          50 LOAD_CONST              11 ('#185fb4')
+               191          50 LOAD_CONST              11 ('#185fb4')
                
-               190          52 LOAD_CONST              12 (2)
+               192          52 LOAD_CONST              12 (2)
                
-               183          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               185          54 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             56 BUILD_CONST_KEY_MAP      6
                
-               172          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               174          58 LOAD_CONST              14 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             60 BUILD_CONST_KEY_MAP      8
                
-               171          62 BUILD_MAP                1
+               173          62 BUILD_MAP                1
                
-               170          64 PRECALL                  1
+               172          64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                             80 LOAD_CONST               0 (None)
                             82 RETURN_VALUE
                consts
                   None
                   'text'
@@ -2048,69 +2067,69 @@
                   ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 169
+               firstlineno 171
                lnotab
                   0x0201180202010202020102010201020202010203020102010201020202
                   0102f904f504ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640464076406640a640b640c9c0664
                   0d9c086901a6010000ab010000000000000000010064005300
-               196           0 RESUME                   0
+               198           0 RESUME                   0
                
-               197           2 LOAD_FAST                0 (self)
+               199           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               199          26 LOAD_CONST               1 ('text')
+               201          26 LOAD_CONST               1 ('text')
                
-               200          28 LOAD_CONST               2 ((3, 4))
+               202          28 LOAD_CONST               2 ((3, 4))
                
-               202          30 LOAD_CONST               3 ('#353535')
+               204          30 LOAD_CONST               3 ('#353535')
                
-               203          32 LOAD_CONST               4 ('#454545')
+               205          32 LOAD_CONST               4 ('#454545')
                
-               204          34 LOAD_CONST               5 ('#cecece')
+               206          34 LOAD_CONST               5 ('#cecece')
                
-               205          36 LOAD_CONST               6 (1)
+               207          36 LOAD_CONST               6 (1)
                
-               207          38 LOAD_CONST               7 ('#ffffff')
+               209          38 LOAD_CONST               7 ('#ffffff')
                
-               208          40 LOAD_CONST               8 (0)
+               210          40 LOAD_CONST               8 (0)
                
-               211          42 LOAD_CONST               9 ('#2f2f2f')
+               213          42 LOAD_CONST               9 ('#2f2f2f')
                
-               212          44 LOAD_CONST               4 ('#454545')
+               214          44 LOAD_CONST               4 ('#454545')
                
-               213          46 LOAD_CONST               7 ('#ffffff')
+               215          46 LOAD_CONST               7 ('#ffffff')
                
-               214          48 LOAD_CONST               6 (1)
+               216          48 LOAD_CONST               6 (1)
                
-               216          50 LOAD_CONST              10 ('#4cc2ff')
+               218          50 LOAD_CONST              10 ('#4cc2ff')
                
-               217          52 LOAD_CONST              11 (2)
+               219          52 LOAD_CONST              11 (2)
                
-               210          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               212          54 LOAD_CONST              12 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             56 BUILD_CONST_KEY_MAP      6
                
-               199          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               201          58 LOAD_CONST              13 (('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             60 BUILD_CONST_KEY_MAP      8
                
-               198          62 BUILD_MAP                1
+               200          62 BUILD_MAP                1
                
-               197          64 PRECALL                  1
+               199          64 PRECALL                  1
                             68 CALL                     1
                             78 POP_TOP
                             80 LOAD_CONST               0 (None)
                             82 RETURN_VALUE
                consts
                   None
                   'text'
@@ -2128,15 +2147,15 @@
                   ('padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 196
+               firstlineno 198
                lnotab
                   0x0201180202010202020102010201020202010203020102010201020202
                   0102f904f504ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 4
@@ -2166,205 +2185,205 @@
                   006a0200000000000000007c005f0e00000000000000007c006a03000000
                   00000000007c005f0f00000000000000007c006a0500000000000000007c
                   005f1000000000000000007c006a0600000000000000007c005f11000000
                   00000000007c017c005f12000000000000000009007c00a0130000000000
                   0000000000000000000000000000006400a6010000ab0100000000000000
                   000100640053002300742800000000000000000000240072040100590064
                   00530077007803590077017c006a1200000000000000005300
-               223           0 RESUME                   0
+               225           0 RESUME                   0
                
-               224           2 LOAD_FAST                1 (dict)
+               226           2 LOAD_FAST                1 (dict)
                              4 EXTENDED_ARG             1
                              6 POP_JUMP_FORWARD_IF_NONE   406 (to 820)
                
-               225           8 LOAD_CONST               1 ('text')
+               227           8 LOAD_CONST               1 ('text')
                             10 LOAD_FAST                1 (dict)
                             12 CONTAINS_OP              0
                             14 EXTENDED_ARG             1
                             16 POP_JUMP_FORWARD_IF_FALSE   293 (to 604)
                
-               226          18 LOAD_FAST                1 (dict)
+               228          18 LOAD_FAST                1 (dict)
                             20 LOAD_CONST               1 ('text')
                             22 BINARY_SUBSCR
                             32 LOAD_CONST               2 ('padding')
                             34 BINARY_SUBSCR
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               0 (text_padding)
                
-               228          56 LOAD_FAST                1 (dict)
+               230          56 LOAD_FAST                1 (dict)
                             58 LOAD_CONST               1 ('text')
                             60 BINARY_SUBSCR
                             70 LOAD_CONST               3 ('back')
                             72 BINARY_SUBSCR
                             82 LOAD_FAST                0 (self)
                             84 STORE_ATTR               1 (text_back)
                
-               229          94 LOAD_FAST                1 (dict)
+               231          94 LOAD_FAST                1 (dict)
                             96 LOAD_CONST               1 ('text')
                             98 BINARY_SUBSCR
                            108 LOAD_CONST               4 ('border')
                            110 BINARY_SUBSCR
                            120 LOAD_FAST                0 (self)
                            122 STORE_ATTR               2 (text_border)
                
-               230         132 LOAD_FAST                1 (dict)
+               232         132 LOAD_FAST                1 (dict)
                            134 LOAD_CONST               1 ('text')
                            136 BINARY_SUBSCR
                            146 LOAD_CONST               5 ('text_back')
                            148 BINARY_SUBSCR
                            158 LOAD_FAST                0 (self)
                            160 STORE_ATTR               3 (text_text_back)
                
-               231         170 LOAD_FAST                1 (dict)
+               233         170 LOAD_FAST                1 (dict)
                            172 LOAD_CONST               1 ('text')
                            174 BINARY_SUBSCR
                            184 LOAD_CONST               6 ('border_width')
                            186 BINARY_SUBSCR
                            196 LOAD_FAST                0 (self)
                            198 STORE_ATTR               4 (text_border_width)
                
-               233         208 LOAD_FAST                1 (dict)
+               235         208 LOAD_FAST                1 (dict)
                            210 LOAD_CONST               1 ('text')
                            212 BINARY_SUBSCR
                            222 LOAD_CONST               7 ('bottom_line')
                            224 BINARY_SUBSCR
                            234 LOAD_FAST                0 (self)
                            236 STORE_ATTR               5 (text_bottom_line)
                
-               234         246 LOAD_FAST                1 (dict)
+               236         246 LOAD_FAST                1 (dict)
                            248 LOAD_CONST               1 ('text')
                            250 BINARY_SUBSCR
                            260 LOAD_CONST               8 ('bottom_width')
                            262 BINARY_SUBSCR
                            272 LOAD_FAST                0 (self)
                            274 STORE_ATTR               6 (text_bottom_width)
                
-               236         284 LOAD_CONST               9 ('focusin')
+               238         284 LOAD_CONST               9 ('focusin')
                            286 LOAD_FAST                1 (dict)
                            288 LOAD_CONST               1 ('text')
                            290 BINARY_SUBSCR
                            300 CONTAINS_OP              0
                            302 POP_JUMP_FORWARD_IF_FALSE   150 (to 604)
                
-               237         304 LOAD_FAST                1 (dict)
+               239         304 LOAD_FAST                1 (dict)
                            306 LOAD_CONST               1 ('text')
                            308 BINARY_SUBSCR
                            318 LOAD_CONST               9 ('focusin')
                            320 BINARY_SUBSCR
                            330 LOAD_CONST               3 ('back')
                            332 BINARY_SUBSCR
                            342 LOAD_FAST                0 (self)
                            344 STORE_ATTR               7 (text_focusin_back)
                
-               238         354 LOAD_FAST                1 (dict)
+               240         354 LOAD_FAST                1 (dict)
                            356 LOAD_CONST               1 ('text')
                            358 BINARY_SUBSCR
                            368 LOAD_CONST               9 ('focusin')
                            370 BINARY_SUBSCR
                            380 LOAD_CONST               4 ('border')
                            382 BINARY_SUBSCR
                            392 LOAD_FAST                0 (self)
                            394 STORE_ATTR               8 (text_focusin_border)
                
-               239         404 LOAD_FAST                1 (dict)
+               241         404 LOAD_FAST                1 (dict)
                            406 LOAD_CONST               1 ('text')
                            408 BINARY_SUBSCR
                            418 LOAD_CONST               9 ('focusin')
                            420 BINARY_SUBSCR
                            430 LOAD_CONST               5 ('text_back')
                            432 BINARY_SUBSCR
                            442 LOAD_FAST                0 (self)
                            444 STORE_ATTR               9 (text_focusin_text_back)
                
-               240         454 LOAD_FAST                1 (dict)
+               242         454 LOAD_FAST                1 (dict)
                            456 LOAD_CONST               1 ('text')
                            458 BINARY_SUBSCR
                            468 LOAD_CONST               9 ('focusin')
                            470 BINARY_SUBSCR
                            480 LOAD_CONST               6 ('border_width')
                            482 BINARY_SUBSCR
                            492 LOAD_FAST                0 (self)
                            494 STORE_ATTR              10 (text_focusin_border_width)
                
-               242         504 LOAD_FAST                1 (dict)
+               244         504 LOAD_FAST                1 (dict)
                            506 LOAD_CONST               1 ('text')
                            508 BINARY_SUBSCR
                            518 LOAD_CONST               9 ('focusin')
                            520 BINARY_SUBSCR
                            530 LOAD_CONST               7 ('bottom_line')
                            532 BINARY_SUBSCR
                            542 LOAD_FAST                0 (self)
                            544 STORE_ATTR              11 (text_focusin_bottom_line)
                
-               243         554 LOAD_FAST                1 (dict)
+               245         554 LOAD_FAST                1 (dict)
                            556 LOAD_CONST               1 ('text')
                            558 BINARY_SUBSCR
                            568 LOAD_CONST               9 ('focusin')
                            570 BINARY_SUBSCR
                            580 LOAD_CONST               8 ('bottom_width')
                            582 BINARY_SUBSCR
                            592 LOAD_FAST                0 (self)
                            594 STORE_ATTR              12 (text_focusin_bottom_width)
                
-               245     >>  604 LOAD_FAST                0 (self)
+               247     >>  604 LOAD_FAST                0 (self)
                            606 LOAD_ATTR                1 (text_back)
                            616 LOAD_FAST                0 (self)
                            618 STORE_ATTR              13 (_text_back)
                
-               246         628 LOAD_FAST                0 (self)
+               248         628 LOAD_FAST                0 (self)
                            630 LOAD_ATTR                2 (text_border)
                            640 LOAD_FAST                0 (self)
                            642 STORE_ATTR              14 (_text_border)
                
-               247         652 LOAD_FAST                0 (self)
+               249         652 LOAD_FAST                0 (self)
                            654 LOAD_ATTR                3 (text_text_back)
                            664 LOAD_FAST                0 (self)
                            666 STORE_ATTR              15 (_text_text_back)
                
-               248         676 LOAD_FAST                0 (self)
+               250         676 LOAD_FAST                0 (self)
                            678 LOAD_ATTR                5 (text_bottom_line)
                            688 LOAD_FAST                0 (self)
                            690 STORE_ATTR              16 (_text_bottom_line)
                
-               249         700 LOAD_FAST                0 (self)
+               251         700 LOAD_FAST                0 (self)
                            702 LOAD_ATTR                6 (text_bottom_width)
                            712 LOAD_FAST                0 (self)
                            714 STORE_ATTR              17 (_text_bottom_width)
                
-               251         724 LOAD_FAST                1 (dict)
+               253         724 LOAD_FAST                1 (dict)
                            726 LOAD_FAST                0 (self)
                            728 STORE_ATTR              18 (_palette)
                
-               253         738 NOP
+               255         738 NOP
                
-               254         740 LOAD_FAST                0 (self)
+               256         740 LOAD_FAST                0 (self)
                            742 LOAD_METHOD             19 (_draw)
                            764 LOAD_CONST               0 (None)
                            766 PRECALL                  1
                            770 CALL                     1
                            780 POP_TOP
                            782 LOAD_CONST               0 (None)
                            784 RETURN_VALUE
                        >>  786 PUSH_EXC_INFO
                
-               255         788 LOAD_GLOBAL             40 (AttributeError)
+               257         788 LOAD_GLOBAL             40 (AttributeError)
                            800 CHECK_EXC_MATCH
                            802 POP_JUMP_FORWARD_IF_FALSE     4 (to 812)
                            804 POP_TOP
                
-               256         806 POP_EXCEPT
+               258         806 POP_EXCEPT
                            808 LOAD_CONST               0 (None)
                            810 RETURN_VALUE
                
-               255     >>  812 RERAISE                  0
+               257     >>  812 RERAISE                  0
                        >>  814 COPY                     3
                            816 POP_EXCEPT
                            818 RERAISE                  1
                
-               258     >>  820 LOAD_FAST                0 (self)
+               260     >>  820 LOAD_FAST                0 (self)
                            822 LOAD_ATTR               18 (_palette)
                            832 RETURN_VALUE
                ExceptionTable:
                  740 to 780 -> 786 [0]
                  786 to 804 -> 814 [1] lasti
                  812 to 812 -> 814 [1] lasti
                consts
@@ -2380,194 +2399,194 @@
                   'focusin'
                names      ('text_padding', 'text_back', 'text_border', 'text_text_back', 'text_border_width', 'text_bottom_line', 'text_bottom_width', 'text_focusin_back', 'text_focusin_border', 'text_focusin_text_back', 'text_focusin_border_width', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_text_back', '_text_border', '_text_text_back', '_text_bottom_line', '_text_bottom_width', '_palette', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 223
+               firstlineno 225
                lnotab
                   0x020106010a012602260126012601260226012602140132013201320132
                   0232013202180118011801180118020e0202013001120106ff0803
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'tbbox', 'compare', 'count', 'debug', 'tdelete', 'dump', 'get', 'tindex', 'tinsert', 'search', 'see', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'str', '__init__', 'tbbox', 'compare', 'count', 'debug', 'tdelete', 'dump', 'get', 'tindex', 'tinsert', 'search', 'see', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicText'
          firstlineno 6
          lnotab
-            0x0c01122906030603060306030603060306030603060306030603060606
+            0x0c011a2b06030603060306030603060306030603060306030603060606
             060604061c0809080908030803080b0e060603061b061b
       'AdwDrawBasicText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         261           0 RESUME                   0
+         263           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawText')
                        8 STORE_NAME               2 (__qualname__)
          
-         262          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 262>)
+         264          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 264>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               262           0 RESUME                   0
+               264           0 RESUME                   0
                
-               263           2 LOAD_FAST                0 (self)
+               265           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 262
+               firstlineno 264
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawText'
-         firstlineno 261
+         firstlineno 263
          lnotab 0x0a01
       'AdwDrawText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         266           0 RESUME                   0
+         268           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         267          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 267>)
+         269          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 269>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               267           0 RESUME                   0
+               269           0 RESUME                   0
                
-               268           2 LOAD_FAST                0 (self)
+               270           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 267
+               firstlineno 269
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawDarkText'
-         firstlineno 266
+         firstlineno 268
          lnotab 0x0a01
       'AdwDrawDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             0a640484015a05640584005a06640684005a07640784005a08640884005a
             09640a88006601640984095a0a880078015a0b5300
                        0 MAKE_CELL                0 (__class__)
          
-         272           2 RESUME                   0
+         274           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText')
                       10 STORE_NAME               2 (__qualname__)
          
-         273          12 LOAD_CLOSURE             0 (__class__)
+         275          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 273>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 275>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         276          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 276>)
+         278          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 278>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         279          28 LOAD_CONST              10 ((None,))
-                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 279>)
+         281          28 LOAD_CONST              10 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 281>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               5 (border_radius)
          
-         285          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 285>)
+         287          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 287>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               6 (_draw)
          
-         315          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 315>)
+         317          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 317>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               7 (default_palette)
          
-         318          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 318>)
+         320          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 320>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (palette_light)
          
-         346          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 346>)
+         348          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 348>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (palette_dark)
          
-         374          60 LOAD_CONST              10 ((None,))
+         376          60 LOAD_CONST              10 ((None,))
                       62 LOAD_CLOSURE             0 (__class__)
                       64 BUILD_TUPLE              1
-                      66 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 374>)
+                      66 LOAD_CONST               9 (<code object palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 376>)
                       68 MAKE_FUNCTION            9 (defaults, closure)
                       70 STORE_NAME              10 (palette)
                       72 LOAD_CLOSURE             0 (__class__)
                       74 COPY                     1
                       76 STORE_NAME              11 (__classcell__)
                       78 RETURN_VALUE
          consts
@@ -2578,17 +2597,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               273           2 RESUME                   0
+               275           2 RESUME                   0
                
-               274           4 PUSH_NULL
+               276           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -2601,29 +2620,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 273
+               firstlineno 275
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               276           0 RESUME                   0
+               278           0 RESUME                   0
                
-               277           2 LOAD_FAST                0 (self)
+               279           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -2641,48 +2660,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 276
+               firstlineno 278
                lnotab 0x0201
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               279           0 RESUME                   0
+               281           0 RESUME                   0
                
-               280           2 LOAD_FAST                1 (radius)
+               282           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               281           6 LOAD_FAST                0 (self)
+               283           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               283     >>   20 LOAD_FAST                1 (radius)
+               285     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 279
+               firstlineno 281
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2718,27 +2737,27 @@
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
                   007c006a1300000000000000007c006a130000000000000000ac0ba60300
                   00ab030000000000000000010064005300
-               285           0 RESUME                   0
+               287           0 RESUME                   0
                
-               286           2 LOAD_FAST                0 (self)
+               288           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               288          44 LOAD_FAST                0 (self)
+               290          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               289          68 LOAD_CONST               2 (2)
+               291          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2747,159 +2766,159 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               290         172 LOAD_FAST                0 (self)
+               292         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               291         184 LOAD_FAST                0 (self)
+               293         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               288         208 KW_NAMES                 4
+               290         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (text_frame)
                
-               294         236 LOAD_FAST                0 (self)
+               296         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               295         260 LOAD_FAST                0 (self)
+               297         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               296         348 LOAD_FAST                0 (self)
+               298         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (text_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (text_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               297         436 LOAD_FAST                0 (self)
+               299         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (text_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (text_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               298         524 LOAD_FAST                0 (self)
+               300         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (text)
                
-               294         536 KW_NAMES                 8
+               296         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (text_text)
                
-               301         564 LOAD_FAST                0 (self)
+               303         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (text_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               302         612 LOAD_FAST                0 (self)
+               304         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_text_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               303         672 LOAD_FAST                0 (self)
+               305         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (text_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               304         738 LOAD_FAST                0 (self)
+               306         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               305         782 LOAD_FAST                0 (self)
+               307         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_text_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_text_bottom_line)
                
-               306         806 LOAD_CONST               6 (0)
+               308         806 LOAD_CONST               6 (0)
                
-               301         808 KW_NAMES                10
+               303         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (text_bottom)
                
-               308         836 LOAD_FAST                0 (self)
+               310         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_text_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               309         858 LOAD_FAST                0 (self)
+               311         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (text_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               311     >>  910 LOAD_FAST                0 (self)
+               313     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (text_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (text_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               313         974 LOAD_FAST                0 (self)
+               315         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (text)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_text_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_text_text_back)
                           1032 LOAD_FAST                0 (self)
@@ -2925,98 +2944,98 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 285
+               firstlineno 287
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
                   0142012c01180102fb1c07160134024002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               315           0 RESUME                   0
+               317           0 RESUME                   0
                
-               316           2 LOAD_FAST                0 (self)
+               318           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 315
+               firstlineno 317
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b6407640c640d640e9c
                   06640f9c096901a6010000ab010000000000000000010064005300
-               318           0 RESUME                   0
+               320           0 RESUME                   0
                
-               319           2 LOAD_FAST                0 (self)
+               321           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               321          26 LOAD_CONST               1 ('text')
+               323          26 LOAD_CONST               1 ('text')
                
-               322          28 LOAD_CONST               2 (6)
+               324          28 LOAD_CONST               2 (6)
                
-               323          30 LOAD_CONST               3 ((3, 4))
+               325          30 LOAD_CONST               3 ((3, 4))
                
-               325          32 LOAD_CONST               4 ('#fdfdfd')
+               327          32 LOAD_CONST               4 ('#fdfdfd')
                
-               326          34 LOAD_CONST               5 ('#eaeaea')
+               328          34 LOAD_CONST               5 ('#eaeaea')
                
-               327          36 LOAD_CONST               6 ('#5f5f5f')
+               329          36 LOAD_CONST               6 ('#5f5f5f')
                
-               328          38 LOAD_CONST               7 (1)
+               330          38 LOAD_CONST               7 (1)
                
-               330          40 LOAD_CONST               5 ('#eaeaea')
+               332          40 LOAD_CONST               5 ('#eaeaea')
                
-               331          42 LOAD_CONST               8 (0)
+               333          42 LOAD_CONST               8 (0)
                
-               334          44 LOAD_CONST               9 ('#f9f9f9')
+               336          44 LOAD_CONST               9 ('#f9f9f9')
                
-               335          46 LOAD_CONST              10 ('#e2e2e2')
+               337          46 LOAD_CONST              10 ('#e2e2e2')
                
-               336          48 LOAD_CONST              11 ('#1a1a1a')
+               338          48 LOAD_CONST              11 ('#1a1a1a')
                
-               337          50 LOAD_CONST               7 (1)
+               339          50 LOAD_CONST               7 (1)
                
-               339          52 LOAD_CONST              12 ('#185fb4')
+               341          52 LOAD_CONST              12 ('#185fb4')
                
-               340          54 LOAD_CONST              13 (2)
+               342          54 LOAD_CONST              13 (2)
                
-               333          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               335          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               321          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               323          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               320          64 BUILD_MAP                1
+               322          64 BUILD_MAP                1
                
-               319          66 PRECALL                  1
+               321          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3036,71 +3055,71 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 318
+               firstlineno 320
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640a640564086407640b640c640d9c
                   06640e9c096901a6010000ab010000000000000000010064005300
-               346           0 RESUME                   0
+               348           0 RESUME                   0
                
-               347           2 LOAD_FAST                0 (self)
+               349           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               349          26 LOAD_CONST               1 ('text')
+               351          26 LOAD_CONST               1 ('text')
                
-               350          28 LOAD_CONST               2 (6)
+               352          28 LOAD_CONST               2 (6)
                
-               351          30 LOAD_CONST               3 ((3, 4))
+               353          30 LOAD_CONST               3 ((3, 4))
                
-               353          32 LOAD_CONST               4 ('#353535')
+               355          32 LOAD_CONST               4 ('#353535')
                
-               354          34 LOAD_CONST               5 ('#454545')
+               356          34 LOAD_CONST               5 ('#454545')
                
-               355          36 LOAD_CONST               6 ('#cecece')
+               357          36 LOAD_CONST               6 ('#cecece')
                
-               356          38 LOAD_CONST               7 (1)
+               358          38 LOAD_CONST               7 (1)
                
-               358          40 LOAD_CONST               8 ('#ffffff')
+               360          40 LOAD_CONST               8 ('#ffffff')
                
-               359          42 LOAD_CONST               9 (0)
+               361          42 LOAD_CONST               9 (0)
                
-               362          44 LOAD_CONST              10 ('#2f2f2f')
+               364          44 LOAD_CONST              10 ('#2f2f2f')
                
-               363          46 LOAD_CONST               5 ('#454545')
+               365          46 LOAD_CONST               5 ('#454545')
                
-               364          48 LOAD_CONST               8 ('#ffffff')
+               366          48 LOAD_CONST               8 ('#ffffff')
                
-               365          50 LOAD_CONST               7 (1)
+               367          50 LOAD_CONST               7 (1)
                
-               367          52 LOAD_CONST              11 ('#4cc2ff')
+               369          52 LOAD_CONST              11 ('#4cc2ff')
                
-               368          54 LOAD_CONST              12 (2)
+               370          54 LOAD_CONST              12 (2)
                
-               361          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               363          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               349          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               351          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               348          64 BUILD_MAP                1
+               350          64 BUILD_MAP                1
                
-               347          66 PRECALL                  1
+               349          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3119,15 +3138,15 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 346
+               firstlineno 348
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -3136,221 +3155,221 @@
                   0x95019700740100000000000000000000a6000000ab0000000000000000
                   00a00100000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000010064017c01760072157c01640119000000000000
                   0000006402190000000000000000007c005f020000000000000000640053
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               374           2 RESUME                   0
+               376           2 RESUME                   0
                
-               375           4 LOAD_GLOBAL              1 (NULL + super)
+               377           4 LOAD_GLOBAL              1 (NULL + super)
                             16 PRECALL                  0
                             20 CALL                     0
                             30 LOAD_METHOD              1 (palette)
                             52 LOAD_FAST                1 (dict)
                             54 PRECALL                  1
                             58 CALL                     1
                             68 POP_TOP
                
-               376          70 LOAD_CONST               1 ('text')
+               378          70 LOAD_CONST               1 ('text')
                             72 LOAD_FAST                1 (dict)
                             74 CONTAINS_OP              0
                             76 POP_JUMP_FORWARD_IF_FALSE    21 (to 120)
                
-               377          78 LOAD_FAST                1 (dict)
+               379          78 LOAD_FAST                1 (dict)
                             80 LOAD_CONST               1 ('text')
                             82 BINARY_SUBSCR
                             92 LOAD_CONST               2 ('radius')
                             94 BINARY_SUBSCR
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               2 (text_radius)
                            116 LOAD_CONST               0 (None)
                            118 RETURN_VALUE
                
-               376     >>  120 LOAD_CONST               0 (None)
+               378     >>  120 LOAD_CONST               0 (None)
                            122 RETURN_VALUE
                consts
                   None
                   'text'
                   'radius'
                names      ('super', 'palette', 'text_radius')
                varnames   ('self', 'dict')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 374
+               firstlineno 376
                lnotab 0x0401420108012aff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText'
-         firstlineno 272
+         firstlineno 274
          lnotab 0x0c010a0306030806061e0603061c061c
       'AdwDrawBasicRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         380           0 RESUME                   0
+         382           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText')
                        8 STORE_NAME               2 (__qualname__)
          
-         381          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 381>)
+         383          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 383>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               381           0 RESUME                   0
+               383           0 RESUME                   0
                
-               382           2 LOAD_FAST                0 (self)
+               384           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 381
+               firstlineno 383
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundText'
-         firstlineno 380
+         firstlineno 382
          lnotab 0x0a01
       'AdwDrawRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         385           0 RESUME                   0
+         387           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         386          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 386>)
+         388          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 388>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               386           0 RESUME                   0
+               388           0 RESUME                   0
                
-               387           2 LOAD_FAST                0 (self)
+               389           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 386
+               firstlineno 388
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText'
-         firstlineno 385
+         firstlineno 387
          lnotab 0x0a01
       'AdwDrawRoundDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             09640484015a05640584005a06640684005a07640784005a08640884005a
             09880078015a0a5300
                        0 MAKE_CELL                0 (__class__)
          
-         390           2 RESUME                   0
+         392           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText3')
                       10 STORE_NAME               2 (__qualname__)
          
-         391          12 LOAD_CLOSURE             0 (__class__)
+         393          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 391>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 393>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         394          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 394>)
+         396          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 396>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         397          28 LOAD_CONST               9 ((None,))
-                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 397>)
+         399          28 LOAD_CONST               9 ((None,))
+                      30 LOAD_CONST               4 (<code object border_radius, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 399>)
                       32 MAKE_FUNCTION            1 (defaults)
                       34 STORE_NAME               5 (border_radius)
          
-         403          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 403>)
+         405          36 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 405>)
                       38 MAKE_FUNCTION            0
                       40 STORE_NAME               6 (_draw)
          
-         439          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 439>)
+         441          42 LOAD_CONST               6 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 441>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               7 (default_palette)
          
-         442          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 442>)
+         444          48 LOAD_CONST               7 (<code object palette_light, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 444>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (palette_light)
          
-         470          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 470>)
+         472          54 LOAD_CONST               8 (<code object palette_dark, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 472>)
                       56 MAKE_FUNCTION            0
                       58 STORE_NAME               9 (palette_dark)
                       60 LOAD_CLOSURE             0 (__class__)
                       62 COPY                     1
                       64 STORE_NAME              10 (__classcell__)
                       66 RETURN_VALUE
          consts
@@ -3361,17 +3380,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               391           2 RESUME                   0
+               393           2 RESUME                   0
                
-               392           4 PUSH_NULL
+               394           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3384,29 +3403,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 391
+               firstlineno 393
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               394           0 RESUME                   0
+               396           0 RESUME                   0
                
-               395           2 LOAD_FAST                0 (self)
+               397           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3424,48 +3443,48 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 394
+               firstlineno 396
                lnotab 0x0201
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               397           0 RESUME                   0
+               399           0 RESUME                   0
                
-               398           2 LOAD_FAST                1 (radius)
+               400           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               399           6 LOAD_FAST                0 (self)
+               401           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               401     >>   20 LOAD_FAST                1 (radius)
+               403     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 397
+               firstlineno 399
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -3501,195 +3520,195 @@
                   00000000000000000000000000000000007c006a100000000000000000a6
                   010000ab01000000000000000001007c00a0110000000000000000000000
                   0000000000000000007c006a1000000000000000007c006a0c0000000000
                   000000a6020000ab02000000000000000001007c006a0b00000000000000
                   00a01200000000000000000000000000000000000000007c006a07000000
                   00000000007c006a1300000000000000007c006a130000000000000000ac
                   0aa6030000ab030000000000000000010064005300
-               403           0 RESUME                   0
+               405           0 RESUME                   0
                
-               404           2 LOAD_FAST                0 (self)
+               406           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               406          44 LOAD_FAST                0 (self)
+               408          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               407          68 LOAD_CONST               2 (0)
+               409          68 LOAD_CONST               2 (0)
                
-               408          70 LOAD_CONST               2 (0)
+               410          70 LOAD_CONST               2 (0)
                
-               409          72 LOAD_FAST                0 (self)
+               411          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                
-               410         116 LOAD_FAST                0 (self)
+               412         116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               411         160 LOAD_FAST                0 (self)
+               413         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               412         172 LOAD_FAST                0 (self)
+               414         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               413         184 LOAD_FAST                0 (self)
+               415         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               406         208 KW_NAMES                 4
+               408         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 POP_TOP
                
-               416         226 LOAD_CONST               5 ('button_frame')
+               418         226 LOAD_CONST               5 ('button_frame')
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_frame)
                
-               418         240 LOAD_FAST                0 (self)
+               420         240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (create_window)
                
-               419         264 LOAD_FAST                0 (self)
+               421         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              2 (winfo_width)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 LOAD_CONST               6 (2)
                            304 BINARY_OP               11 (/)
                            308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              3 (winfo_height)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_CONST               6 (2)
                            348 BINARY_OP               11 (/)
                
-               420         352 LOAD_FAST                0 (self)
+               422         352 LOAD_FAST                0 (self)
                            354 LOAD_METHOD              2 (winfo_width)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (text_border_width)
                            402 BINARY_OP               10 (-)
                            406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (text_padding)
                            418 LOAD_CONST               2 (0)
                            420 BINARY_SUBSCR
                            430 BINARY_OP               10 (-)
                            434 LOAD_CONST               6 (2)
                            436 BINARY_OP               10 (-)
                
-               421         440 LOAD_FAST                0 (self)
+               423         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD              3 (winfo_height)
                            464 PRECALL                  0
                            468 CALL                     0
                            478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR                5 (text_border_width)
                            490 BINARY_OP               10 (-)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (text_padding)
                            506 LOAD_CONST               3 (1)
                            508 BINARY_SUBSCR
                            518 BINARY_OP               10 (-)
                            522 LOAD_CONST               6 (2)
                            524 BINARY_OP               10 (-)
                
-               422         528 LOAD_FAST                0 (self)
+               424         528 LOAD_FAST                0 (self)
                            530 LOAD_ATTR               11 (text)
                
-               418         540 KW_NAMES                 7
+               420         540 KW_NAMES                 7
                            542 PRECALL                  5
                            546 CALL                     5
                            556 LOAD_FAST                0 (self)
                            558 STORE_ATTR              12 (text_text)
                
-               425         568 LOAD_FAST                0 (self)
+               427         568 LOAD_FAST                0 (self)
                            570 LOAD_METHOD             13 (create_rectangle)
                            592 LOAD_CONST               3 (1)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR                4 (text_radius)
                            606 LOAD_CONST               8 (5)
                            608 BINARY_OP               11 (/)
                            612 BINARY_OP                0 (+)
                
-               426         616 LOAD_FAST                0 (self)
+               428         616 LOAD_FAST                0 (self)
                            618 LOAD_METHOD              3 (winfo_height)
                            640 PRECALL                  0
                            644 CALL                     0
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               14 (_text_bottom_width)
                            666 BINARY_OP               10 (-)
                            670 LOAD_CONST               3 (1)
                            672 BINARY_OP               10 (-)
                
-               427         676 LOAD_FAST                0 (self)
+               429         676 LOAD_FAST                0 (self)
                            678 LOAD_METHOD              2 (winfo_width)
                            700 PRECALL                  0
                            704 CALL                     0
                            714 LOAD_CONST               3 (1)
                            716 BINARY_OP               10 (-)
                            720 LOAD_FAST                0 (self)
                            722 LOAD_ATTR                4 (text_radius)
                            732 LOAD_CONST               8 (5)
                            734 BINARY_OP               11 (/)
                            738 BINARY_OP               10 (-)
                
-               428         742 LOAD_FAST                0 (self)
+               430         742 LOAD_FAST                0 (self)
                            744 LOAD_METHOD              3 (winfo_height)
                            766 PRECALL                  0
                            770 CALL                     0
                            780 LOAD_CONST               3 (1)
                            782 BINARY_OP               10 (-)
                
-               429         786 LOAD_FAST                0 (self)
+               431         786 LOAD_FAST                0 (self)
                            788 LOAD_ATTR               15 (_text_bottom_line)
                            798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               15 (_text_bottom_line)
                
-               430         810 LOAD_CONST               2 (0)
+               432         810 LOAD_CONST               2 (0)
                
-               425         812 KW_NAMES                 9
+               427         812 KW_NAMES                 9
                            814 PRECALL                  7
                            818 CALL                     7
                            828 LOAD_FAST                0 (self)
                            830 STORE_ATTR              16 (text_bottom)
                
-               432         840 LOAD_FAST                0 (self)
+               434         840 LOAD_FAST                0 (self)
                            842 LOAD_ATTR               14 (_text_bottom_width)
                            852 LOAD_CONST               2 (0)
                            854 COMPARE_OP               2 (==)
                            860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
                
-               433         862 LOAD_FAST                0 (self)
+               435         862 LOAD_FAST                0 (self)
                            864 LOAD_METHOD              0 (delete)
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               16 (text_bottom)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               435     >>  914 LOAD_FAST                0 (self)
+               437     >>  914 LOAD_FAST                0 (self)
                            916 LOAD_METHOD             17 (tag_raise)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               16 (text_bottom)
                            950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR               12 (text_text)
                            962 PRECALL                  2
                            966 CALL                     2
                            976 POP_TOP
                
-               437         978 LOAD_FAST                0 (self)
+               439         978 LOAD_FAST                0 (self)
                            980 LOAD_ATTR               11 (text)
                            990 LOAD_METHOD             18 (configure)
                           1012 LOAD_FAST                0 (self)
                           1014 LOAD_ATTR                7 (_text_back)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR               19 (_text_text_back)
                           1036 LOAD_FAST                0 (self)
@@ -3714,98 +3733,98 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 403
+               firstlineno 405
                lnotab
                   0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
                   0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               439           0 RESUME                   0
+               441           0 RESUME                   0
                
-               440           2 LOAD_FAST                0 (self)
+               442           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 439
+               firstlineno 441
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b6407640c640d640e9c
                   06640f9c096901a6010000ab010000000000000000010064005300
-               442           0 RESUME                   0
+               444           0 RESUME                   0
                
-               443           2 LOAD_FAST                0 (self)
+               445           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               445          26 LOAD_CONST               1 ('text')
+               447          26 LOAD_CONST               1 ('text')
                
-               446          28 LOAD_CONST               2 (6)
+               448          28 LOAD_CONST               2 (6)
                
-               447          30 LOAD_CONST               3 ((3, 4))
+               449          30 LOAD_CONST               3 ((3, 4))
                
-               449          32 LOAD_CONST               4 ('#fdfdfd')
+               451          32 LOAD_CONST               4 ('#fdfdfd')
                
-               450          34 LOAD_CONST               5 ('#eaeaea')
+               452          34 LOAD_CONST               5 ('#eaeaea')
                
-               451          36 LOAD_CONST               6 ('#5f5f5f')
+               453          36 LOAD_CONST               6 ('#5f5f5f')
                
-               452          38 LOAD_CONST               7 (1)
+               454          38 LOAD_CONST               7 (1)
                
-               454          40 LOAD_CONST               5 ('#eaeaea')
+               456          40 LOAD_CONST               5 ('#eaeaea')
                
-               455          42 LOAD_CONST               8 (0)
+               457          42 LOAD_CONST               8 (0)
                
-               458          44 LOAD_CONST               9 ('#f9f9f9')
+               460          44 LOAD_CONST               9 ('#f9f9f9')
                
-               459          46 LOAD_CONST              10 ('#e2e2e2')
+               461          46 LOAD_CONST              10 ('#e2e2e2')
                
-               460          48 LOAD_CONST              11 ('#1a1a1a')
+               462          48 LOAD_CONST              11 ('#1a1a1a')
                
-               461          50 LOAD_CONST               7 (1)
+               463          50 LOAD_CONST               7 (1)
                
-               463          52 LOAD_CONST              12 ('#185fb4')
+               465          52 LOAD_CONST              12 ('#185fb4')
                
-               464          54 LOAD_CONST              13 (2)
+               466          54 LOAD_CONST              13 (2)
                
-               457          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               459          56 LOAD_CONST              14 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               445          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               447          60 LOAD_CONST              15 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               444          64 BUILD_MAP                1
+               446          64 BUILD_MAP                1
                
-               443          66 PRECALL                  1
+               445          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3825,71 +3844,71 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 442
+               firstlineno 444
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 18
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   026403640464056406640764086409640a640564086407640b640c640d9c
                   06640e9c096901a6010000ab010000000000000000010064005300
-               470           0 RESUME                   0
+               472           0 RESUME                   0
                
-               471           2 LOAD_FAST                0 (self)
+               473           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               473          26 LOAD_CONST               1 ('text')
+               475          26 LOAD_CONST               1 ('text')
                
-               474          28 LOAD_CONST               2 (6)
+               476          28 LOAD_CONST               2 (6)
                
-               475          30 LOAD_CONST               3 ((3, 4))
+               477          30 LOAD_CONST               3 ((3, 4))
                
-               477          32 LOAD_CONST               4 ('#353535')
+               479          32 LOAD_CONST               4 ('#353535')
                
-               478          34 LOAD_CONST               5 ('#454545')
+               480          34 LOAD_CONST               5 ('#454545')
                
-               479          36 LOAD_CONST               6 ('#cecece')
+               481          36 LOAD_CONST               6 ('#cecece')
                
-               480          38 LOAD_CONST               7 (1)
+               482          38 LOAD_CONST               7 (1)
                
-               482          40 LOAD_CONST               8 ('#ffffff')
+               484          40 LOAD_CONST               8 ('#ffffff')
                
-               483          42 LOAD_CONST               9 (0)
+               485          42 LOAD_CONST               9 (0)
                
-               486          44 LOAD_CONST              10 ('#2f2f2f')
+               488          44 LOAD_CONST              10 ('#2f2f2f')
                
-               487          46 LOAD_CONST               5 ('#454545')
+               489          46 LOAD_CONST               5 ('#454545')
                
-               488          48 LOAD_CONST               8 ('#ffffff')
+               490          48 LOAD_CONST               8 ('#ffffff')
                
-               489          50 LOAD_CONST               7 (1)
+               491          50 LOAD_CONST               7 (1)
                
-               491          52 LOAD_CONST              11 ('#4cc2ff')
+               493          52 LOAD_CONST              11 ('#4cc2ff')
                
-               492          54 LOAD_CONST              12 (2)
+               494          54 LOAD_CONST              12 (2)
                
-               485          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
+               487          56 LOAD_CONST              13 (('back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width'))
                             58 BUILD_CONST_KEY_MAP      6
                
-               473          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
+               475          60 LOAD_CONST              14 (('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin'))
                             62 BUILD_CONST_KEY_MAP      9
                
-               472          64 BUILD_MAP                1
+               474          64 BUILD_MAP                1
                
-               471          66 PRECALL                  1
+               473          66 PRECALL                  1
                             70 CALL                     1
                             80 POP_TOP
                             82 LOAD_CONST               0 (None)
                             84 RETURN_VALUE
                consts
                   None
                   'text'
@@ -3908,138 +3927,138 @@
                   ('radius', 'padding', 'back', 'border', 'text_back', 'border_width', 'bottom_line', 'bottom_width', 'focusin')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 470
+               firstlineno 472
                lnotab
                   0x0201180202010201020202010201020102020201020302010201020102
                   02020102f904f404ff02ff
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'border_radius', '_draw', 'default_palette', 'palette_light', 'palette_dark', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText3'
-         firstlineno 390
+         firstlineno 392
          lnotab 0x0c010a030603080606240603061c
       'AdwDrawBasicRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         499           0 RESUME                   0
+         501           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         500          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 500>)
+         502          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 502>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               500           0 RESUME                   0
+               502           0 RESUME                   0
                
-               501           2 LOAD_FAST                0 (self)
+               503           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 500
+               firstlineno 502
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundText3'
-         firstlineno 499
+         firstlineno 501
          lnotab 0x0a01
       'AdwDrawRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         504           0 RESUME                   0
+         506           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         505          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 505>)
+         507          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\windows\canvas\textbox.py", line 507>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               505           0 RESUME                   0
+               507           0 RESUME                   0
                
-               506           2 LOAD_FAST                0 (self)
+               508           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 505
+               firstlineno 507
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText3'
-         firstlineno 504
+         firstlineno 506
          lnotab 0x0a01
       'AdwDrawRoundDarkText3'
       '__main__'
       ('Tk',)
       'x'
       5
       ('fill', 'padx', 'pady')
@@ -4048,10 +4067,10 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\textbox.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f007f00011c051c061c6c1c051c051c6d1c051c
+      0x00ff020110010c041c7f007f00031c051c061c6c1c051c051c6d1c051c
       050c010c0214021401300214013002140130021401300214013002140130
       022ce9
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/canvas/__pycache__/widget.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xebc8a464 (Wed Jul  5 01:35:39 2023 UTC)
-files sz: 406
+moddate:  0xc6e3b064 (Fri Jul 14 05:57:26 2023 UTC)
+files sz: 520
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
@@ -34,84 +34,88 @@
       ('AdwDrawEngine',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
-            0x8700970065005a0164005a0288006601640184085a03640284005a0464
-            05640484015a05880078015a065300
+            0x8700970065005a0164005a0264015a0388006601640284085a04640384
+            005a056406640584015a06880078015a075300
                        0 MAKE_CELL                0 (__class__)
          
            4           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwWidget')
                       10 STORE_NAME               2 (__qualname__)
          
-           5          12 LOAD_CLOSURE             0 (__class__)
-                      14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 5>)
-                      18 MAKE_FUNCTION            8 (closure)
-                      20 STORE_NAME               3 (__init__)
+           6          12 LOAD_CONST               1 ('\n    基础绘制组件类\n\n    特性：自动将背景颜色设为父组件背景颜色\n    ')
+                      14 STORE_NAME               3 (__doc__)
          
-          11          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 11>)
-                      24 MAKE_FUNCTION            0
-                      26 STORE_NAME               4 (_other)
+          12          16 LOAD_CLOSURE             0 (__class__)
+                      18 BUILD_TUPLE              1
+                      20 LOAD_CONST               2 (<code object __init__, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 12>)
+                      22 MAKE_FUNCTION            8 (closure)
+                      24 STORE_NAME               4 (__init__)
          
-          14          28 LOAD_CONST               5 ((None,))
-                      30 LOAD_CONST               4 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 14>)
-                      32 MAKE_FUNCTION            1 (defaults)
-                      34 STORE_NAME               5 (_draw)
-                      36 LOAD_CLOSURE             0 (__class__)
-                      38 COPY                     1
-                      40 STORE_NAME               6 (__classcell__)
-                      42 RETURN_VALUE
+          18          26 LOAD_CONST               3 (<code object _other, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 18>)
+                      28 MAKE_FUNCTION            0
+                      30 STORE_NAME               5 (_other)
+         
+          21          32 LOAD_CONST               6 ((None,))
+                      34 LOAD_CONST               5 (<code object _draw, file "D:\tkadw\tkadw\windows\canvas\widget.py", line 21>)
+                      36 MAKE_FUNCTION            1 (defaults)
+                      38 STORE_NAME               6 (_draw)
+                      40 LOAD_CLOSURE             0 (__class__)
+                      42 COPY                     1
+                      44 STORE_NAME               7 (__classcell__)
+                      46 RETURN_VALUE
          consts
             'AdwWidget'
+            '\n    基础绘制组件类\n\n    特性：自动将背景颜色设为父组件背景颜色\n    '
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e0101007c00a00200
                   0000000000000000000000000000000000000064017c006a030000000000
                   0000006402ac03a6030000ab03000000000000000001007c00a004000000
                   0000000000000000000000000000000000a6000000ab0000000000000000
                   00010064005300
                              0 COPY_FREE_VARS           1
                
-                 5           2 RESUME                   0
+                12           2 RESUME                   0
                
-                 6           4 PUSH_NULL
+                13           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
                             48 DICT_MERGE               1
                             50 CALL_FUNCTION_EX         1
                             52 POP_TOP
                
-                 8          54 LOAD_FAST                0 (self)
+                15          54 LOAD_FAST                0 (self)
                             56 LOAD_METHOD              2 (bind)
                             78 LOAD_CONST               1 ('<Configure>')
                             80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                3 (_draw)
                             92 LOAD_CONST               2 ('+')
                             94 KW_NAMES                 3
                             96 PRECALL                  3
                            100 CALL                     3
                            110 POP_TOP
                
-                 9         112 LOAD_FAST                0 (self)
+                16         112 LOAD_FAST                0 (self)
                            114 LOAD_METHOD              4 (_other)
                            136 PRECALL                  0
                            140 CALL                     0
                            150 POP_TOP
                            152 LOAD_CONST               0 (None)
                            154 RETURN_VALUE
                consts
@@ -121,29 +125,29 @@
                   ('add',)
                names      ('super', '__init__', 'bind', '_draw', '_other')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '__init__'
-               firstlineno 5
+               firstlineno 12
                lnotab 0x040132023a01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-                11           0 RESUME                   0
+                18           0 RESUME                   0
                
-                12           2 LOAD_FAST                0 (self)
+                19           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -161,46 +165,46 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_other'
-               firstlineno 11
+               firstlineno 18
                lnotab 0x0201
             None
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x970064005300
-                14           0 RESUME                   0
+                21           0 RESUME                   0
                
-                15           2 LOAD_CONST               0 (None)
+                22           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
                name       '_draw'
-               firstlineno 14
+               firstlineno 21
                lnotab 0x0201
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', '_other', '_draw', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', '__init__', '_other', '_draw', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
          name       'AdwWidget'
          firstlineno 4
-         lnotab 0x0c010a060603
+         lnotab 0x0c0204060a060603
       'AdwWidget'
       None
    names      ('tkadw.windows.canvas.drawengine', 'AdwDrawEngine', 'AdwWidget')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\windows\\canvas\\widget.py'
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/button.py` & `tkadw-0.3.2/tkadw/windows/canvas/button.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from tkinter.font import Font, nametofont
 from tkadw.windows.canvas.widget import AdwWidget
 
 
 # Button
 class AdwDrawBasicButton(AdwWidget):
+
+    """
+    自绘基础按钮
+    """
+
     def __init__(self, *args, width=120, height=40, text: str = "", command=None, **kwargs):
         super().__init__(*args, width=width, height=height, bd=0, highlightthickness=0, **kwargs)
 
         self.default_palette()
 
         self.text = text
 
@@ -36,15 +41,22 @@
             self.bind("<<Click>>", lambda event: self.command())
         elif "text" in kwargs:
             self.text = kwargs.pop("text")
             self._draw(None)
         else:
             super().configure(**kwargs)
 
-    def _draw(self, evt):
+    def update(self) -> None:
+        """
+        多执行一道绘制
+        """
+        super().update()
+        self._draw(None)
+
+    def _draw(self, evt=None):
         self.delete("all")
 
         # 绘制按钮边框
         self.button_frame = self.create_rectangle(
             self._button_border_width - 1, self._button_border_width - 1,
             self.winfo_width() - self._button_border_width + 1,
             self.winfo_height() - self._button_border_width + 1,
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/checkbox.py` & `tkadw-0.3.2/tkadw/windows/canvas/checkbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/drawengine.py` & `tkadw-0.3.2/tkadw/windows/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/entry.py` & `tkadw-0.3.2/tkadw/windows/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/frame.py` & `tkadw-0.3.2/tkadw/windows/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/separator.py` & `tkadw-0.3.2/tkadw/windows/canvas/separator.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/textbox.py` & `tkadw-0.3.2/tkadw/windows/canvas/textbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from tkinter.font import Font, nametofont
 from tkadw.windows.canvas.drawengine import AdwDrawEngine
 
 
 # Text
 class AdwDrawBasicText(AdwDrawEngine):
-    def __init__(self, *args, width=120, height=80, **kwargs):
+    def __init__(self, *args, text: str = "", width=120, height=80, **kwargs):
 
         super().__init__(*args, width=width, height=height, highlightthickness=0, **kwargs)
 
         from tkinter import Text
 
         self.text_text_font = nametofont("TkDefaultFont")
 
         self.text = Text(self, bd=0, font=self.text_text_font, undo=True, highlightthickness=0)
 
+        self.text.insert("1.0", text)
+
         self._other()
 
         self.default_palette()
 
         self._text_back = self.text_back
         self._text_border = self.text_border
         self._text_text_back = self.text_text_back
```

### Comparing `tkadw-0.3.1/tkadw/windows/canvas/titlebar.py` & `tkadw-0.3.2/tkadw/windows/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/fluent/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/button.py` & `tkadw-0.3.2/tkadw/windows/fluent/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/entry.py` & `tkadw-0.3.2/tkadw/windows/fluent/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/frame.py` & `tkadw-0.3.2/tkadw/windows/fluent/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/GeneralSans-Regular.ttf` & `tkadw-0.3.2/tkadw/windows/fluent/GeneralSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/fluent/test.py` & `tkadw-0.3.2/tkadw/windows/fluent/test.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/theme.py` & `tkadw-0.3.2/tkadw/windows/theme.py`

 * *Files 16% similar despite different names*

```diff
@@ -552,14 +552,200 @@
         "back": "#232527",
         "border_width": 1,
 
         "rounded": True
     }
 }
 
+metro_theme = {
+    "window": {
+        "back": "#ffffff"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#000000",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#eeeeee",
+        "border": "#cccccc",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "active": {
+            "back": "#666666",
+            "border": "#666666",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#333333",
+            "border": "#333333",
+            "text_back": "#ffffff",
+            "border_width": 1,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#ffffff",
+        "border": "#bfbfbf",
+        "border_width": 2,
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#ffffff",
+        "border": "#999999",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#ffffff",
+            "border": "#00aedb",
+            "text_back": "#000000",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#ffffff",
+        "border": "#999999",
+        "text_back": "#000000",
+        "border_width": 1,
+
+        "bottom_line": "#ffffff",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#ffffff",
+            "border": "#00aedb",
+            "text_back": "#000000",
+            "border_width": 1,
+
+            "bottom_line": "#ffffff",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#999999",
+        "border_width": 1,
+
+        "rounded": True
+    }
+}
+
+metro_dark_theme = {
+    "window": {
+        "back": "#111111"
+    },
+
+    "label": {
+        "back": "transparent",
+        "text_back": "#000000",
+    },
+
+    "button": {
+        "radius": 0,
+        "back": "#222222",
+        "border": "#444444",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "active": {
+            "back": "#aaaaaa",
+            "border": "#aaaaaa",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+
+        "pressed": {
+            "back": "#eeeeee",
+            "border": "#eeeeee",
+            "text_back": "#000000",
+            "border_width": 1,
+        },
+    },
+
+    "frame": {
+        "radius": 0,
+        "back": "#111111",
+        "border": "#373737",
+        "border_width": 2,
+    },
+
+    "entry": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#111111",
+        "border": "#999999",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#000000",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#111111",
+            "border": "#00aedb",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#000000",
+            "bottom_width": 0,
+        }
+    },
+
+    "text": {
+        "radius": 0,
+        "padding": (3, 3),
+
+        "back": "#111111",
+        "border": "#999999",
+        "text_back": "#ffffff",
+        "border_width": 1,
+
+        "bottom_line": "#000000",
+        "bottom_width": 0,
+
+        "focusin": {
+            "back": "#111111",
+            "border": "#00aedb",
+            "text_back": "#ffffff",
+            "border_width": 1,
+
+            "bottom_line": "#000000",
+            "bottom_width": 0,
+        }
+    },
+
+    "separator": {
+        "back": "#999999",
+        "border_width": 1,
+
+        "rounded": False
+    }
+}
+
 
 def get_default_theme():
     from os import environ
     from json import loads
     try:
         return loads(environ["tkAdwite.DefaultTheme"])
     except KeyError:
@@ -615,14 +801,29 @@
                     _set_default_theme(bilibili_dark_theme)
                 else:
                     _set_default_theme(bilibili_theme)
         elif mode.lower() == "dark":
             _set_default_theme(bilibili_dark_theme)
         else:
             _set_default_theme(bilibili_theme)
+    elif theme == "metro" or theme == "Metro":
+        if mode.lower() == "system" or mode.lower() == "auto":
+            try:
+                from darkdetect import isDark
+            except ModuleNotFoundError:
+                _set_default_theme(metro_theme)
+            else:
+                if isDark():
+                    _set_default_theme(metro_dark_theme)
+                else:
+                    _set_default_theme(metro_theme)
+        elif mode.lower() == "dark":
+            _set_default_theme(metro_dark_theme)
+        else:
+            _set_default_theme(metro_theme)
     else:
         _set_default_theme(theme)
 
 
 set_default_theme("win11")
 
 
@@ -631,14 +832,16 @@
 
 class Adwite(Adw):
     def set_default_theme(self, theme, _mode="auto"):
         set_default_theme(theme, _mode)
         for widget in self.winfo_children():
             if hasattr(widget, "palette"):
                 widget.palette(get_default_theme())
+                widget.configure(background=widget.master.cget("bg"))
+                widget._draw(None)
         self.palette(get_default_theme())
 
     def default_palette(self):
         self.palette(get_default_theme())
 
 
 from tkadw.windows.widgets import AdwLabel
@@ -689,19 +892,23 @@
         self.palette(get_default_theme())
 
 
 if __name__ == '__main__':
     from darkdetect import isDark
 
     root = Adwite()
-    root.set_default_theme("win11")
-    button = AdwTButton()
+    root.set_default_theme("metro")
+
+    def toggle():
+        root.set_default_theme("win11")
+
+    button = AdwTButton(text="AdwTButton", command=toggle)
     button.pack(fill="x", padx=5, pady=5)
     separator = AdwTSeparator()
     separator.pack(fill="x", padx=5, pady=5)
-    entry = AdwTEntry()
+    entry = AdwTEntry(text="AdwTEntry")
     entry.pack(fill="x", padx=5, pady=5)
-    text = AdwTText()
+    text = AdwTText(text="AdwTText")
     text.pack(fill="x", padx=5, pady=5)
     frame = AdwTFrame()
     frame.pack(fill="x", padx=5, pady=5)
     root.mainloop()
```

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/adw.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc` & `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc` & `tkadw-0.3.2/tkadw/windows/widgets/__pycache__/label.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/adw.py` & `tkadw-0.3.2/tkadw/windows/widgets/adw.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/label.py` & `tkadw-0.3.2/tkadw/windows/widgets/label.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.3.1/tkadw/windows/widgets/mdi.py` & `tkadw-0.3.2/tkadw/windows/widgets/mdi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,52 @@
-from tkadw import AdwTFrame, AdwTButton
+from tkadw.windows.theme import AdwTFrame, AdwTButton
 
 
-class MDI(AdwTFrame):
+class AdwMDI(AdwTFrame):
+
+    """
+    多文档窗口
+    """
+
     def create_child(self):
+        """
+        创建一个子窗口
+
+        :return: AdwTFrame
+        """
         child = AdwTFrame(self.frame)
         child.place(x=10, y=10, width=150, height=150)
 
-        child.closebutton = AdwTButton(child.frame, text="✕", width=25, height=25, command=lambda: child.place_forget())
+        child.titlebar = AdwTFrame(child.frame, height=38)
+        child.titlebar.frame_border_width = 0
+        child.titlebar.frame_border = child.frame_back
+        child.closebutton = AdwTButton(child.titlebar.frame, text="✕", width=25, height=25, command=lambda: child.place_forget())
         child.closebutton.pack(anchor="ne", padx=2, pady=2)
+        child.titlebar.pack(fill="x", side="top", padx=2, pady=2)
 
-        child.frame.bind("<Button-1>", self._click)
-        child.frame.bind("<B1-Motion>", lambda event: self._move(event, child))
+        child.titlebar.frame.bind("<Button-1>", self._click)
+        child.titlebar.frame.bind("<B1-Motion>", lambda event: self._move(event, child))
 
         return child
 
     def _click(self, event):
         self.x, self.y = event.x, event.y
 
     def _move(self, event, child):
         child.place(
-            x=event.x-self.x+self.winfo_rootx(),
-            y=event.y-self.y+self.winfo_rooty()
+            x=(event.x-self.x)+child.winfo_x(),
+            y=(event.y-self.y)+child.winfo_y()
         )
-        print(child.winfo_x(), child.winfo_y())
 
 
 if __name__ == '__main__':
     from tkadw import Adwite, set_default_theme
 
-    set_default_theme("win11", "light")
+    set_default_theme("gtk", "light")
 
     root = Adwite()
 
-    mdi = MDI()
+    mdi = AdwMDI()
     mdiChild1 = mdi.create_child()
     mdi.pack(fill="both", expand="yes", padx=10, pady=10)
 
     root.mainloop()
```

### Comparing `tkadw-0.3.1/PKG-INFO` & `tkadw-0.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.3.1
+Version: 0.3.2
 Summary: extra for tkinter
 License: MIT
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -86,7 +86,12 @@
 >> `301`新增`AdwSeparator`分割线组件 新增`AdwWidget`简化组件绘制流程
 > 
 >> `302`分支`widgets`库，将加入仅使用组件组合起来的控件，而非用canvas绘出来的组件
 > 
 >> `303`调改`AdwDrawEntry`和`AdwDrawText`的焦点事件绑定
 > 
 >> `304`新增主题类组件，只需使用`set_default_theme`设置主题。对于经过特殊设计和特殊样式的组件，比如`Fluent`主题组件、`Win11`主题控件`AccentButton`，将不加入主题变量内
+
+> `0.3.2`
+>> `321` 新增`AdwMDI`组件
+> 
+>> `322` 添加`metro`主题
```

