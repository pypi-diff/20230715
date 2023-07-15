# Comparing `tmp/versioned-0.5.2.tar.gz` & `tmp/versioned-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "versioned-0.5.2.tar", last modified: Fri Jul 14 20:47:33 2023, max compression
+gzip compressed data, was "versioned-0.5.3.tar", last modified: Sat Jul 15 03:18:00 2023, max compression
```

## Comparing `versioned-0.5.2.tar` & `versioned-0.5.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001953 versioned-0.5.2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.5.2/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.5.2/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.5.2/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4256 2023-07-14 20:47:33.001833 versioned-0.5.2/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3121 2023-07-14 20:43:22.000000 versioned-0.5.2/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     4772 2023-07-14 20:47:04.000000 versioned-0.5.2/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.5.2/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.5.2/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      159 2023-07-14 20:41:46.000000 versioned-0.5.2/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-14 20:47:33.001993 versioned-0.5.2/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.5.2/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:32.997287 versioned-0.5.2/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1197 2023-07-14 20:45:40.000000 versioned-0.5.2/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    10411 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_s3_and_dynamodb_backend.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    15087 2023-07-14 20:41:46.000000 versioned-0.5.2/tests/test_s3_only_backend.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:32.999826 versioned-0.5.2/versioned/
--rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.5.2/versioned/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-14 20:45:16.000000 versioned-0.5.2/versioned/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      472 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.5.2/versioned/bootstrap.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/compat.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/constants.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.000739 versioned-0.5.2/versioned/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     4518 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/dynamodb.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      157 2023-07-02 06:40:29.000000 versioned-0.5.2/versioned/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    17807 2023-07-14 20:46:31.000000 versioned-0.5.2/versioned/s3_and_dynamodb_backend.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    23254 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/s3_only_backend.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001160 versioned-0.5.2/versioned/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.5.2/versioned/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.001645 versioned-0.5.2/versioned/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7573 2023-07-14 20:41:46.000000 versioned-0.5.2/versioned/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.5.2/versioned/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-14 20:47:33.000632 versioned-0.5.2/versioned.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4256 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      911 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      281 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-14 20:47:32.000000 versioned-0.5.2/versioned.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.588434 versioned-0.5.3/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-07-01 03:35:21.000000 versioned-0.5.3/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1120 2023-07-01 03:35:21.000000 versioned-0.5.3/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      317 2023-07-01 03:35:21.000000 versioned-0.5.3/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4419 2023-07-15 03:18:00.588241 versioned-0.5.3/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3284 2023-07-15 03:09:37.000000 versioned-0.5.3/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5368 2023-07-15 03:14:36.000000 versioned-0.5.3/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-07-01 03:35:21.000000 versioned-0.5.3/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-07-01 03:35:21.000000 versioned-0.5.3/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-07-01 03:35:21.000000 versioned-0.5.3/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-07-02 06:52:14.000000 versioned-0.5.3/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      159 2023-07-14 20:41:46.000000 versioned-0.5.3/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-07-15 03:18:00.588491 versioned-0.5.3/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7558 2023-07-01 03:35:21.000000 versioned-0.5.3/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.580461 versioned-0.5.3/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1197 2023-07-14 20:45:40.000000 versioned-0.5.3/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-07-14 20:41:46.000000 versioned-0.5.3/tests/test_dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    11352 2023-07-15 03:11:42.000000 versioned-0.5.3/tests/test_s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    15816 2023-07-15 02:57:06.000000 versioned-0.5.3/tests/test_s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.583342 versioned-0.5.3/versioned/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      435 2023-07-02 06:36:19.000000 versioned-0.5.3/versioned/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-07-15 03:15:41.000000 versioned-0.5.3/versioned/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      553 2023-07-15 03:15:58.000000 versioned-0.5.3/versioned/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1959 2023-07-07 14:49:41.000000 versioned-0.5.3/versioned/bootstrap.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      383 2023-07-14 20:41:46.000000 versioned-0.5.3/versioned/compat.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      230 2023-07-14 20:41:46.000000 versioned-0.5.3/versioned/constants.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.584605 versioned-0.5.3/versioned/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4518 2023-07-14 20:41:46.000000 versioned-0.5.3/versioned/dynamodb.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      209 2023-07-15 02:21:01.000000 versioned-0.5.3/versioned/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    18389 2023-07-15 03:10:32.000000 versioned-0.5.3/versioned/s3_and_dynamodb_backend.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    25088 2023-07-15 02:57:22.000000 versioned-0.5.3/versioned/s3_only_backend.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.585291 versioned-0.5.3/versioned/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-07-02 02:30:24.000000 versioned-0.5.3/versioned/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.587901 versioned-0.5.3/versioned/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7573 2023-07-14 20:41:46.000000 versioned-0.5.3/versioned/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-07-01 03:35:22.000000 versioned-0.5.3/versioned/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-07-15 03:18:00.584478 versioned-0.5.3/versioned.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4419 2023-07-15 03:18:00.000000 versioned-0.5.3/versioned.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      911 2023-07-15 03:18:00.000000 versioned-0.5.3/versioned.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-07-15 03:18:00.000000 versioned-0.5.3/versioned.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      281 2023-07-15 03:18:00.000000 versioned-0.5.3/versioned.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       10 2023-07-15 03:18:00.000000 versioned-0.5.3/versioned.egg-info/top_level.txt
```

### Comparing `versioned-0.5.2/AUTHORS.rst` & `versioned-0.5.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/LICENSE.txt` & `versioned-0.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/PKG-INFO` & `versioned-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.5.2
+Version: 0.5.3
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -82,15 +82,16 @@
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
-- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+- `Quick Start - S3 and Dynamodb Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_and_dynamodb_backend.ipynb>`_
+- `Quick Start - S3 only Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_only_backend.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
 Related Project:
```

### Comparing `versioned-0.5.2/README.rst` & `versioned-0.5.3/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
-- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+- `Quick Start - S3 and Dynamodb Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_and_dynamodb_backend.ipynb>`_
+- `Quick Start - S3 only Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_only_backend.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
 Related Project:
```

### Comparing `versioned-0.5.2/requirements-doc.txt` & `versioned-0.5.3/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/setup.py` & `versioned-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/tests/test_api.py` & `versioned-0.5.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/tests/test_dynamodb.py` & `versioned-0.5.3/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/tests/test_s3_and_dynamodb_backend.py` & `versioned-0.5.3/tests/test_s3_and_dynamodb_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,57 @@
 # -*- coding: utf-8 -*-
 
 import moto
 import pytest
 
+from datetime import datetime
 from s3pathlib import S3Path, context
 
 from versioned import exc
 from versioned import constants
 from versioned.dynamodb import encode_version_sk
 from versioned.tests.mock_aws import BaseMockTest
-from versioned.s3_and_dynamodb_backend import Repository
+from versioned.s3_and_dynamodb_backend import (
+    Alias,
+    Repository,
+)
 
 from rich import print as rprint
 
 
+class TestAlias:
+    def test_random_artifact(self):
+        ali = Alias(
+            name="deploy",
+            alias="LIVE",
+            update_at=datetime.utcnow(),
+            version="1",
+            secondary_version="2",
+            secondary_version_weight=50,
+            version_s3uri="s3uri1",
+            secondary_version_s3uri="s3uri2",
+        )
+        for _ in range(10):
+            assert ali.random_artifact() in ["s3uri1", "s3uri2"]
+
+        ali = Alias(
+            name="deploy",
+            alias="LIVE",
+            update_at=datetime.utcnow(),
+            version="1",
+            secondary_version=None,
+            secondary_version_weight=None,
+            version_s3uri="s3uri1",
+            secondary_version_s3uri=None,
+        )
+        for _ in range(10):
+            artifact_s3_uri = ali.random_artifact()
+            assert artifact_s3_uri == "s3uri1"
+
+
 class Test(BaseMockTest):
     use_mock = True
 
     mock_list = [
         moto.mock_sts,
         moto.mock_s3,
         moto.mock_dynamodb,
```

### Comparing `versioned-0.5.2/tests/test_s3_only_backend.py` & `versioned-0.5.3/tests/test_s3_only_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         "LATEST",
         "hello-world",
         "123abc",
     ]:
         with pytest.raises(ValueError):
             validate_alias_name(alias)
 
+
 class TestAlias:
     def test_random_artifact(self):
         ali = Alias(
             name="deploy",
             alias="LIVE",
             update_at="",
             version="1",
@@ -107,29 +108,34 @@
             s3_bucket=f"{cls.bsm.aws_account_id}-{cls.bsm.aws_region}-artifacts",
             suffix=".txt",
         )
         cls.repo.bootstrap(cls.bsm)
 
     def _test_error(self):
         name = "deploy"
+        LIVE = "LIVE"
         self.repo.purge_all(bsm=self.bsm)
 
         # --- test Artifact error ---
         # at this moment, no artifact exists
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.publish_artifact_version(bsm=self.bsm, name=name)
 
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.get_artifact_version(bsm=self.bsm, name=name)
 
         artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
 
+        with pytest.raises(exc.ArtifactS3BackendError):
+            self.repo.delete_artifact_version(
+                bsm=self.bsm, name=name, version=constants.LATEST_VERSION
+            )
+
         # delete an non existing artifact version should always success for idempotency
-        self.repo.delete_artifact_version(bsm=self.bsm, name=name)
         self.repo.delete_artifact_version(bsm=self.bsm, name=name, version=1)
 
         # --- test Alias error ---
         alias = "LIVE"
 
         # try to put alias on non-exist artifact
         with pytest.raises(exc.ArtifactNotFoundError):
@@ -204,14 +210,17 @@
         # alias not exists
         with pytest.raises(exc.AliasNotFoundError):
             self.repo.get_alias(bsm=self.bsm, name=name, alias="Invalid")
 
         alias_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(alias_list) == 0
 
+        # delete an non existing alias should always success for idempotency
+        self.repo.delete_alias(bsm=self.bsm, name=name, alias=LIVE)
+
     def _test_artifact_and_alias(self):
         name = "deploy"
         alias = "LIVE"
 
         self.repo.purge_all(bsm=self.bsm)
 
         # ======================================================================
@@ -380,61 +389,78 @@
         # rprint(ali)
         _assert_alias(ali)
 
         ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 1
         _assert_alias(ali_list[0])
 
+        # the second version doesn't exists, should raise error
         with pytest.raises(exc.ArtifactNotFoundError):
             self.repo.put_alias(
                 bsm=self.bsm,
                 name=name,
                 alias=alias,
                 secondary_version=999,
                 secondary_version_weight=50,
             )
 
-        # --- test delete methods
+    def _test_delete_and_purge(self):
+        name = "deploy"
+        LIVE = "LIVE"
+        DEV = "DEV"
+
+        self.repo.purge_all(bsm=self.bsm)
+
+        # prepare
+        self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v1")
+        self.repo.publish_artifact_version(bsm=self.bsm, name=name)
+        self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v2")
+        self.repo.publish_artifact_version(bsm=self.bsm, name=name)
+        self.repo.put_artifact(bsm=self.bsm, name=name, content=b"v3")
+        self.repo.publish_artifact_version(bsm=self.bsm, name=name)
+
+        self.repo.put_alias(
+            bsm=self.bsm,
+            name=name,
+            alias=LIVE,
+            version=2,
+            secondary_version=3,
+            secondary_version_weight=10,
+        )
+        self.repo.put_alias(bsm=self.bsm, name=name, alias=DEV)
+
+        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
+        assert len(ali_list) == 2
+
         # delete alias then get it back, should raise error
-        self.repo.delete_alias(bsm=self.bsm, name=name, alias=alias)
+        self.repo.delete_alias(bsm=self.bsm, name=name, alias=DEV)
         with pytest.raises(exc.AliasNotFoundError):
-            self.repo.get_alias(bsm=self.bsm, name=name, alias=alias)
+            self.repo.get_alias(bsm=self.bsm, name=name, alias=DEV)
         ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
-        assert len(ali_list) == 0
+        assert len(ali_list) == 1
 
         # delete artifact version then get it back, should raise error
-        self.repo.delete_artifact_version(bsm=self.bsm, name=name)
-        with pytest.raises(exc.ArtifactNotFoundError):
-            self.repo.get_artifact_version(bsm=self.bsm, name=name)
         artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
-        assert len(artifact_list) == 2
-
-        self.repo.delete_artifact_version(bsm=self.bsm, name=name, version=1)
+        assert len(artifact_list) == 4
+        self.repo.delete_artifact_version(bsm=self.bsm, name=name, version=3)
         with pytest.raises(exc.ArtifactNotFoundError):
-            self.repo.get_artifact_version(bsm=self.bsm, name=name, version=1)
+            self.repo.get_artifact_version(bsm=self.bsm, name=name, version=3)
         artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
-        assert len(artifact_list) == 1
+        assert len(artifact_list) == 3
 
         # --- purge
-        # try to put alias based on a deleted version, then it should raise error
-        with pytest.raises(exc.ArtifactNotFoundError):
-            self.repo.put_alias(bsm=self.bsm, name=name, alias="DEV", version=1)
-
-        self.repo.put_alias(bsm=self.bsm, name=name, alias="DEV", version=2)
-        ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
-        assert len(ali_list) == 1
-
         self.repo.purge_artifact(bsm=self.bsm, name=name)
         artifact_list = self.repo.list_artifact_versions(bsm=self.bsm, name=name)
         assert len(artifact_list) == 0
         ali_list = self.repo.list_aliases(bsm=self.bsm, name=name)
         assert len(ali_list) == 0
 
     def test(self):
         self._test_error()
         self._test_artifact_and_alias()
+        self._test_delete_and_purge()
 
 
 if __name__ == "__main__":
     from versioned.tests import run_cov_test
 
     run_cov_test(__file__, "versioned.s3_only_backend", preview=False)
```

### Comparing `versioned-0.5.2/versioned/bootstrap.py` & `versioned-0.5.3/versioned/bootstrap.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned/dynamodb.py` & `versioned-0.5.3/versioned/dynamodb.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned/paths.py` & `versioned-0.5.3/versioned/paths.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned/s3_and_dynamodb_backend.py` & `versioned-0.5.3/versioned/s3_and_dynamodb_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 
 import typing as T
 
+import random
 import dataclasses
 from datetime import datetime
 
 from boto_session_manager import BotoSesManager
 from s3pathlib import S3Path, context
 from func_args import NOTHING
 from pynamodb.connection import Connection
 
 from . import constants
 from . import dynamodb
 from . import exc
+from .compat import cached_property
 from .bootstrap import bootstrap
 from .vendor.hashes import hashes
 
 hashes.use_sha256()
 
 
 @dataclasses.dataclass
@@ -103,14 +105,31 @@
 
     def get_secondary_version_content(self, bsm: BotoSesManager) -> bytes:
         """
         Get the content of the secondary artifact version of this alias.
         """
         return self.s3path_secondary_version.read_bytes(bsm=bsm)
 
+    @cached_property
+    def _version_weight(self) -> int:
+        if self.secondary_version_weight is None:
+            return 100
+        else:
+            return 100 - self.secondary_version_weight
+
+    def random_artifact(self) -> str:
+        """
+        Randomly return either the primary or secondary artifact version s3uri
+        based on the weight.
+        """
+        if random.randint(1, 100) <= self._version_weight:
+            return self.version_s3uri
+        else:
+            return self.secondary_version_s3uri
+
 
 @dataclasses.dataclass
 class Repository:
     """
     Repository class for artifact store.
 
     :param aws_region: the aws region of where the artifact store is.
```

### Comparing `versioned-0.5.2/versioned/s3_only_backend.py` & `versioned-0.5.3/versioned/s3_only_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -318,28 +318,62 @@
             if "Not Found" in error_msg or "does not exist" in error_msg:
                 raise exc.ArtifactNotFoundError(
                     f"Cannot find artifact: artifact name = {name!r}, version = {version!r}"
                 )
             else:
                 raise e
 
+    def _list_artifact_versions_s3path(
+        self,
+        bsm: BotoSesManager,
+        name: str,
+        limit: T.Optional[int] = None,
+    ) -> T.List[S3Path]:  # pragma: no cover
+        """
+        List the s3path of artifact versions of this artifact. Perform additional
+        check to make sure the s3 dir structure are not contaminated.
+        """
+        s3dir_artifact = self._get_artifact_s3dir(name=name).joinpath("versions")
+        if limit is None:
+            s3path_list = s3dir_artifact.iter_objects(bsm=bsm).all()
+        else:
+            s3path_list = s3dir_artifact.iter_objects(bsm=bsm, limit=limit).all()
+        n = len(s3path_list)
+        if n >= 1:
+            if decode_filename(s3path_list[0].fname) != LATEST_VERSION:
+                raise exc.ArtifactS3BackendError(
+                    f"S3 folder {s3dir_artifact.uri} for artifact {name!r} is contaminated! "
+                    f"The first s3 object is not the LATEST version {s3path_list[0].uri}"
+                )
+        if n >= 2:
+            for s3path in s3path_list[1:]:
+                if decode_filename(s3path.fname).isdigit() is False:
+                    raise exc.ArtifactS3BackendError(
+                        f"S3 folder {s3dir_artifact.uri} for artifact {name!r} is contaminated! "
+                        f"Found non-numeric version {s3path.uri!r}"
+                    )
+        return s3path_list
+
     def get_latest_published_artifact_version_number(
         self,
         bsm: BotoSesManager,
         name: str,
     ) -> int:
         """
         Return the latest published artifact version number,
         if no version has been published yet, return 0.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        s3dir_artifact = self._get_artifact_s3dir(name=name)
-        s3path_list = s3dir_artifact.iter_objects(bsm=bsm, limit=2).all()
+        s3path_list = self._list_artifact_versions_s3path(
+            bsm=bsm,
+            name=name,
+            limit=2,
+        )
         if len(s3path_list) in [0, 1]:
             return 0
         else:
             return int(decode_filename(s3path_list[1].fname))
 
     def _get_alias_object(
         self,
@@ -451,99 +485,111 @@
         """
         Return a list of artifact versions. The latest version is always the first item.
         And the newer version comes first.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        s3dir_artifact = self._get_artifact_s3dir(name=name)
-        return [
-            Artifact(
+        artifact_list = list()
+        for s3path in self._list_artifact_versions_s3path(
+            bsm=bsm,
+            name=name,
+        ):
+            s3path.head_object(bsm=bsm)
+            artifact = Artifact(
                 name=name,
                 version=decode_filename(s3path.fname),
                 update_at=s3path.last_modified_at.isoformat(),
                 s3uri=s3path.uri,
                 sha256=s3path.metadata[METADATA_KEY_ARTIFACT_SHA256],
             )
-            for s3path in s3dir_artifact.iter_objects(bsm=bsm)
-        ]
+            artifact_list.append(artifact)
+        return artifact_list
 
     def publish_artifact_version(
         self,
         bsm: BotoSesManager,
         name: str,
     ) -> Artifact:
         """
         Creates a version from the latest artifact. Use versions to create an
         immutable snapshot of your latest artifact.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
-        s3dir_artifact = self._get_artifact_s3dir(name=name)
-        s3path_list = s3dir_artifact.iter_objects(bsm=bsm, limit=2).all()
-        n = len(s3path_list)
-        s3path_latest = self._get_artifact_s3path(
+        s3path_list = self._list_artifact_versions_s3path(
+            bsm=bsm,
             name=name,
-            version=LATEST_VERSION,
+            limit=2,
         )
+        n = len(s3path_list)
         if n == 0:
             raise exc.ArtifactNotFoundError(
                 f"artifact {name!r} not found! you must put artifact first!"
             )
-        elif n == 1:
+        s3path_latest = s3path_list[0]
+        if n == 1:
             new_version = "1"
             s3path_new = self._get_artifact_s3path(name=name, version=new_version)
             s3path_latest.copy_to(s3path_new, bsm=bsm)
+            s3path_new.head_object(bsm=bsm)
             return Artifact(
                 name=name,
                 version=new_version,
                 update_at=s3path_new.last_modified_at.isoformat(),
                 s3uri=s3path_new.uri,
                 sha256=s3path_new.metadata[METADATA_KEY_ARTIFACT_SHA256],
             )
         else:
-            previous_version = decode_filename(s3path_list[1].fname)
+            s3path_previous = s3path_list[1]
+            previous_version = decode_filename(s3path_previous.fname)
             new_version = str(int(previous_version) + 1)
-            s3path_new = self._get_artifact_s3path(name=name, version=new_version)
             s3path_previous = s3path_list[1]
             if s3path_previous.etag == s3path_latest.etag:
+                s3path_previous.head_object(bsm=bsm)
                 return Artifact(
                     name=name,
                     version=previous_version,
                     update_at=s3path_previous.last_modified_at.isoformat(),
                     s3uri=s3path_previous.uri,
                     sha256=s3path_previous.metadata[METADATA_KEY_ARTIFACT_SHA256],
                 )
             else:
+                s3path_new = self._get_artifact_s3path(name=name, version=new_version)
                 s3path_latest.copy_to(s3path_new, bsm=bsm)
+                s3path_new.head_object(bsm=bsm)
                 return Artifact(
                     name=name,
                     version=new_version,
                     update_at=s3path_new.last_modified_at.isoformat(),
                     s3uri=s3path_new.uri,
                     sha256=s3path_new.metadata[METADATA_KEY_ARTIFACT_SHA256],
                 )
 
     def delete_artifact_version(
         self,
         bsm: BotoSesManager,
         name: str,
-        version: T.Optional[T.Union[int, str]] = None,
+        version: T.Union[int, str],
     ):
         """
         Deletes a specific version of artifact. If version is not specified,
         the latest version is deleted. Note that this is a soft delete,
         neither the S3 artifact nor the DynamoDB item is deleted. It is just
         become "invisible" to the :func:`get_artifact` and :func:`list_artifacts``.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         :param version: artifact version. If ``None``, delete the latest version.
         """
+        if encode_version(version) == LATEST_VERSION:
+            raise exc.ArtifactS3BackendError(
+                "You cannot delete the LATEST artifact version!"
+            )
         self._get_artifact_s3path(name=name, version=version).delete(bsm=bsm)
 
     # ------------------------------------------------------------------------------
     # Alias
     # ------------------------------------------------------------------------------
     def put_alias(
         self,
@@ -649,22 +695,20 @@
         """
         Returns a list of aliases for an artifact.
 
         :param bsm: ``boto_session_manager.BotoSesManager`` object.
         :param name: artifact name.
         """
         s3dir = self._get_artifact_s3dir(name=name).joinpath("aliases")
-        return [
-            self._get_alias_object(
-                bsm=bsm,
-                name=s3path.parent.parent.basename,
-                alias=s3path.fname,
-            )
-            for s3path in s3dir.iter_objects(bsm=bsm)
-        ]
+        alias_list = list()
+        for s3path in s3dir.iter_objects(bsm=bsm):
+            alias = Alias.from_dict(json.loads(s3path.read_text(bsm=bsm)))
+            alias.update_at = s3path.last_modified_at.isoformat()
+            alias_list.append(alias)
+        return alias_list
 
     def delete_alias(
         self,
         bsm: BotoSesManager,
         name: str,
         alias: str,
     ):
```

### Comparing `versioned-0.5.2/versioned/tests/mock_aws.py` & `versioned-0.5.3/versioned/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned/vendor/hashes.py` & `versioned-0.5.3/versioned/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned/vendor/pytest_cov_helper.py` & `versioned-0.5.3/versioned/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `versioned-0.5.2/versioned.egg-info/PKG-INFO` & `versioned-0.5.3/versioned.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: versioned
-Version: 0.5.2
+Version: 0.5.3
 Summary: The version and alias best practice for immutable artifacts and deployment.
 Home-page: https://github.com/MacHu-GWU/versioned-project
-Download-URL: https://pypi.python.org/pypi/versioned/0.5.2#downloads
+Download-URL: https://pypi.python.org/pypi/versioned/0.5.3#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
@@ -82,15 +82,16 @@
 
 Welcome to ``versioned`` Documentation
 ==============================================================================
 The version and alias best practice for immutable artifacts and deployment.
 
 Tutorial:
 
-- `Quick Start <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/Quick-Start.ipynb>`_
+- `Quick Start - S3 and Dynamodb Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_and_dynamodb_backend.ipynb>`_
+- `Quick Start - S3 only Backend <https://github.com/MacHu-GWU/versioned-project/blob/main/examples/s3_only_backend.ipynb>`_
 
 Learn why Blue / Green, Canary deployment and Rollback made easy with versioning and alias management.
 
 .. image:: https://github.com/MacHu-GWU/versioned-project/assets/6800411/57f7970e-3821-45a0-9deb-64890e04c129
 
 Related Project:
```

### Comparing `versioned-0.5.2/versioned.egg-info/SOURCES.txt` & `versioned-0.5.3/versioned.egg-info/SOURCES.txt`

 * *Files identical despite different names*

