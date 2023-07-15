# Comparing `tmp/junatum-1.0.1.tar.gz` & `tmp/junatum-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "junatum-1.0.1.tar", last modified: Sat Oct 15 15:12:29 2022, max compression
+gzip compressed data, was "junatum-1.0.2.tar", last modified: Sat Jul 15 13:45:47 2023, max compression
```

## Comparing `junatum-1.0.1.tar` & `junatum-1.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.071873 junatum-1.0.1/
--rw-r--r--   0 benjamin   (501) staff       (20)      215 2022-04-03 09:52:58.000000 junatum-1.0.1/LICENSE
--rw-r--r--   0 benjamin   (501) staff       (20)       42 2022-09-08 03:22:33.000000 junatum-1.0.1/MANIFEST.in
--rw-r--r--   0 benjamin   (501) staff       (20)      795 2022-10-15 15:12:29.071925 junatum-1.0.1/PKG-INFO
--rw-r--r--   0 benjamin   (501) staff       (20)     2504 2022-09-08 03:54:08.000000 junatum-1.0.1/README.md
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.069954 junatum-1.0.1/junatum/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2019-04-06 02:42:54.000000 junatum-1.0.1/junatum/__init__.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.070740 junatum-1.0.1/junatum/common/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2019-04-06 04:32:17.000000 junatum-1.0.1/junatum/common/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)      999 2020-05-07 15:20:12.000000 junatum-1.0.1/junatum/common/decorators.py
--rw-r--r--   0 benjamin   (501) staff       (20)       65 2019-04-06 04:32:57.000000 junatum-1.0.1/junatum/common/exceptions.py
--rw-r--r--   0 benjamin   (501) staff       (20)      158 2022-04-03 09:52:58.000000 junatum-1.0.1/junatum/common/models.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.071060 junatum-1.0.1/junatum/common/tests/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2020-08-27 03:04:43.000000 junatum-1.0.1/junatum/common/tests/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     5814 2022-09-08 03:22:58.000000 junatum-1.0.1/junatum/common/tests/test_utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)     7553 2022-09-08 03:22:58.000000 junatum-1.0.1/junatum/common/utils.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.071603 junatum-1.0.1/junatum/finance/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2020-08-27 03:04:43.000000 junatum-1.0.1/junatum/finance/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     1625 2022-04-03 09:52:58.000000 junatum-1.0.1/junatum/finance/constants.py
-drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2022-10-15 15:12:29.071783 junatum-1.0.1/junatum/finance/tests/
--rw-r--r--   0 benjamin   (501) staff       (20)        0 2020-08-27 03:04:43.000000 junatum-1.0.1/junatum/finance/tests/__init__.py
--rw-r--r--   0 benjamin   (501) staff       (20)     4977 2022-10-15 15:08:06.000000 junatum-1.0.1/junatum/finance/tests/test_utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)     3159 2022-10-15 15:02:31.000000 junatum-1.0.1/junatum/finance/utils.py
--rw-r--r--   0 benjamin   (501) staff       (20)      188 2021-12-05 13:49:28.000000 junatum-1.0.1/pyproject.toml
--rw-r--r--   0 benjamin   (501) staff       (20)       83 2022-04-03 09:52:58.000000 junatum-1.0.1/requirements.txt
--rw-r--r--   0 benjamin   (501) staff       (20)      593 2022-10-15 15:12:29.072287 junatum-1.0.1/setup.cfg
--rw-r--r--   0 benjamin   (501) staff       (20)      951 2022-10-15 15:01:58.000000 junatum-1.0.1/setup.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.914594 junatum-1.0.2/
+-rw-r--r--   0 benjamin   (501) staff       (20)      215 2023-07-15 13:44:29.000000 junatum-1.0.2/LICENSE
+-rw-r--r--   0 benjamin   (501) staff       (20)       42 2023-07-15 07:09:53.000000 junatum-1.0.2/MANIFEST.in
+-rw-r--r--   0 benjamin   (501) staff       (20)      775 2023-07-15 13:45:47.914660 junatum-1.0.2/PKG-INFO
+-rw-r--r--   0 benjamin   (501) staff       (20)     2210 2023-07-15 13:44:21.000000 junatum-1.0.2/README.md
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.913162 junatum-1.0.2/junatum/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2019-04-06 02:42:54.000000 junatum-1.0.2/junatum/__init__.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.913649 junatum-1.0.2/junatum/common/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2019-04-06 04:32:17.000000 junatum-1.0.2/junatum/common/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      999 2020-05-07 15:20:12.000000 junatum-1.0.2/junatum/common/decorators.py
+-rw-r--r--   0 benjamin   (501) staff       (20)       65 2019-04-06 04:32:57.000000 junatum-1.0.2/junatum/common/exceptions.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      158 2022-04-03 09:52:58.000000 junatum-1.0.2/junatum/common/models.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.913911 junatum-1.0.2/junatum/common/tests/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2020-08-27 03:04:43.000000 junatum-1.0.2/junatum/common/tests/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     5814 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/common/tests/test_utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     7553 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/common/utils.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.914254 junatum-1.0.2/junatum/finance/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/finance/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     1625 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/finance/constants.py
+drwxr-xr-x   0 benjamin   (501) staff       (20)        0 2023-07-15 13:45:47.914490 junatum-1.0.2/junatum/finance/tests/
+-rw-r--r--   0 benjamin   (501) staff       (20)        0 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/finance/tests/__init__.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     4977 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/finance/tests/test_utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)     3159 2023-07-15 07:09:53.000000 junatum-1.0.2/junatum/finance/utils.py
+-rw-r--r--   0 benjamin   (501) staff       (20)      188 2023-07-15 07:10:02.000000 junatum-1.0.2/pyproject.toml
+-rw-r--r--   0 benjamin   (501) staff       (20)       83 2023-07-15 13:41:04.000000 junatum-1.0.2/requirements.txt
+-rw-r--r--   0 benjamin   (501) staff       (20)      593 2023-07-15 13:45:47.914984 junatum-1.0.2/setup.cfg
+-rw-r--r--   0 benjamin   (501) staff       (20)      904 2023-07-15 07:10:02.000000 junatum-1.0.2/setup.py
```

### Comparing `junatum-1.0.1/PKG-INFO` & `junatum-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: junatum
-Version: 1.0.1
+Version: 1.0.2
 Summary: Common modules for all projects.
 Home-page: https://github.com/Junatum/junatum
 Author: Junatum
 Author-email: admin@junatum.com
-License: © 2015-2022 Junatum. All rights reserved.
+License: © 2015-2023 Junatum. All rights reserved.
         
         Unauthorized copying of this file, via any medium is strictly prohibited proprietary and confidential.
         Written by Junatum Administrator <admin@junatum.com>, December 2015
         
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `junatum-1.0.1/README.md` & `junatum-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # Junatum 프로젝트
 
-[![codecov](https://codecov.io/gh/Junatum/junatum/branch/master/graph/badge.svg?token=VXPOL1XT7U)](https://codecov.io/gh/Junatum/junatum) [![CircleCI](https://circleci.com/gh/Junatum/junatum.svg?style=svg&circle-token=7ab6e0231496707e9520da253ada611db0084d34)](https://circleci.com/gh/Junatum/junatum)
+![Github Workflow](https://github.com/Junatum/junatum/actions/workflows/main.yml/badge.svg)
 
 Junatum 프로젝트는 공통으로 사용되는 모듈을 패키지화 하는 프로젝트입니다.
 
 
 # 주요 시스템 구성 요소
 
-* Python 3.8
-* Python 3.9
 * Python 3.10
+* Python 3.11
 
 
 # 개발
 
 ## 패키징 하는 방법
 
 1. setup.py 에서 version 을 변경합니다.
 2. `make build` 를 실행한다.
 
 ## 테스트 방법
 
 1. `pyenv`를 준비한다.
    ```
-   pyenv virtualenv -p python3.8 3.8.0 py38
-   pyenv virtualenv -p python3.9 3.9.0 py39
-   pyenv virtualenv -p python3.9 3.10.0 py310
+   pyenv virtualenv 3.10.0 py310
+   pyenv virtualenv 3.11.0 py311
 
-   pyenv local py38 py39 py310
+   pyenv local py310 py311
    ```
 2. `tox` 를 실행한다.
 
 ## 브랜치 전략
 
 * Trunk-based Development ([링크](https://www.flagship.io/glossary/trunk-based-development/)) 를 기반으로 합니다.
 
@@ -71,8 +69,8 @@
 [LICENSE](LICENSE) 참조
 
 
 # 저자
 
 * Junatum <admin@junatum.com>
 
-© 2015-2022 Junatum. All rights reserved.
+© 2015-2023 Junatum. All rights reserved.
```

### Comparing `junatum-1.0.1/junatum/common/decorators.py` & `junatum-1.0.2/junatum/common/decorators.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/junatum/common/tests/test_utils.py` & `junatum-1.0.2/junatum/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/junatum/common/utils.py` & `junatum-1.0.2/junatum/common/utils.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/junatum/finance/constants.py` & `junatum-1.0.2/junatum/finance/constants.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/junatum/finance/tests/test_utils.py` & `junatum-1.0.2/junatum/finance/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/junatum/finance/utils.py` & `junatum-1.0.2/junatum/finance/utils.py`

 * *Files identical despite different names*

### Comparing `junatum-1.0.1/setup.cfg` & `junatum-1.0.2/setup.cfg`

 * *Files identical despite different names*

