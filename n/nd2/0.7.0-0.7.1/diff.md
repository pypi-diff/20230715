# Comparing `tmp/nd2-0.7.0.tar.gz` & `tmp/nd2-0.7.1.tar.gz`

## Comparing `nd2-0.7.0.tar` & `nd2-0.7.1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.7.0/.github_changelog_generator
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nd2-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    18887 2020-02-02 00:00:00.000000 nd2-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 nd2-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/cron.yml
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 nd2-0.7.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/index.md
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/nd2.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/nd2_binary.md
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/API/structures.md
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nd2-0.7.0/docs/styles/extra.css
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/bf_describe.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/compare.py
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/comparison.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/download_samples.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/gather.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nd2-0.7.0/scripts/nd2_describe.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/__init__.py
--rw-r--r--   0        0        0     8543 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_binary.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_clx_lite.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_clx_xml.py
--rw-r--r--   0        0        0     8440 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_ome.py
--rw-r--r--   0        0        0     6219 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_util.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_version.py
--rw-r--r--   0        0        0     9120 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/index.py
--rw-r--r--   0        0        0    49780 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/nd2file.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/py.typed
--rw-r--r--   0        0        0    14331 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/structures.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/__init__.py
--rw-r--r--   0        0        0    12041 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/_legacy.py
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_legacy/_legacy_xml.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/__init__.py
--rw-r--r--   0        0        0    14677 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_chunk_decode.py
--rw-r--r--   0        0        0    25557 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_parse.py
--rw-r--r--   0        0        0    21293 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_pysdk.py
--rw-r--r--   0        0        0    21560 2020-02-02 00:00:00.000000 nd2-0.7.0/src/nd2/_pysdk/_sdk_types.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/readlim_output.json
--rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/samples_metadata.json
--rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_aicsimage.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_binary.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_codspeed.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_dask_dispatch.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_deprecations.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_index.py
--rw-r--r--   0        0        0     5686 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_metadata.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_ome.py
--rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_parse.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_reader.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_readme.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_rescue.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_rois.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_segfaults.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/test_xml.py
--rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/variant.xml
--rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.7.0/tests/variant_CustomDataV2_0.xml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.7.0/.gitignore
--rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.7.0/LICENSE
--rw-r--r--   0        0        0    32417 2020-02-02 00:00:00.000000 nd2-0.7.0/README.md
--rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 nd2-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    34675 2020-02-02 00:00:00.000000 nd2-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nd2-0.7.1/.github_changelog_generator
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 nd2-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 nd2-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 nd2-0.7.1/mkdocs.yml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 nd2-0.7.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 nd2-0.7.1/docs/index.md
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nd2-0.7.1/docs/API/nd2.md
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nd2-0.7.1/docs/API/nd2_binary.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nd2-0.7.1/docs/API/structures.md
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 nd2-0.7.1/docs/styles/extra.css
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/bf_describe.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/compare.py
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/comparison.json
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/download_samples.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/gather.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nd2-0.7.1/scripts/nd2_describe.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/__init__.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_binary.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_ome.py
+-rw-r--r--   0        0        0    21767 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_sdk_types.py
+-rw-r--r--   0        0        0     6285 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_version.py
+-rw-r--r--   0        0        0     9147 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/index.py
+-rw-r--r--   0        0        0    46579 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/nd2file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/py.typed
+-rw-r--r--   0        0        0    14317 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/structures.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/__init__.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/_chunk_decode.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/_clx_lite.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/_clx_xml.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/_legacy_xml.py
+-rw-r--r--   0        0        0    25561 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/_parse/_parse.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/__init__.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/_legacy/__init__.py
+-rw-r--r--   0        0        0    18922 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/_legacy/legacy_reader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/_modern/__init__.py
+-rw-r--r--   0        0        0    25590 2020-02-02 00:00:00.000000 nd2-0.7.1/src/nd2/readers/_modern/modern_reader.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0  5234229 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/readlim_output.json
+-rw-r--r--   0        0        0   513829 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/samples_metadata.json
+-rw-r--r--   0        0        0     6728 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_aicsimage.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_binary.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_codspeed.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_dask_dispatch.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_deprecations.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_index.py
+-rw-r--r--   0        0        0     6091 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_metadata.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_ome.py
+-rw-r--r--   0        0        0     4185 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_parse.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_reader.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_readme.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_rescue.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_rois.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_segfaults.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/test_xml.py
+-rw-r--r--   0        0        0    34639 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/variant.xml
+-rw-r--r--   0        0        0     5601 2020-02-02 00:00:00.000000 nd2-0.7.1/tests/variant_CustomDataV2_0.xml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nd2-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 nd2-0.7.1/LICENSE
+-rw-r--r--   0        0        0    22785 2020-02-02 00:00:00.000000 nd2-0.7.1/README.md
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 nd2-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    25043 2020-02-02 00:00:00.000000 nd2-0.7.1/PKG-INFO
```

### Comparing `nd2-0.7.0/.pre-commit-config.yaml` & `nd2-0.7.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/CHANGELOG.md` & `nd2-0.7.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,34 @@
 # Changelog
 
+## [v0.7.1](https://github.com/tlambert03/nd2/tree/v0.7.1) (2023-07-15)
+
+[Full Changelog](https://github.com/tlambert03/nd2/compare/v0.7.0...v0.7.1)
+
+**Implemented enhancements:**
+
+- feat: accept file handles as well as paths [\#161](https://github.com/tlambert03/nd2/pull/161) ([tlambert03](https://github.com/tlambert03))
+- feat: decode compressed lite variant, and read string type tags [\#159](https://github.com/tlambert03/nd2/pull/159) ([tlambert03](https://github.com/tlambert03))
+
+**Fixed bugs:**
+
+- fix: fix binary reshaping [\#164](https://github.com/tlambert03/nd2/pull/164) ([tlambert03](https://github.com/tlambert03))
+
+**Tests & CI:**
+
+- test: bump coverage [\#163](https://github.com/tlambert03/nd2/pull/163) ([tlambert03](https://github.com/tlambert03))
+
+**Documentation:**
+
+- docs: update readme [\#162](https://github.com/tlambert03/nd2/pull/162) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- refactor: use common base class for legacy and modern reader, move logic from nd2file [\#160](https://github.com/tlambert03/nd2/pull/160) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.7.0](https://github.com/tlambert03/nd2/tree/v0.7.0) (2023-07-05)
 
 [Full Changelog](https://github.com/tlambert03/nd2/compare/v0.6.1...v0.7.0)
 
 **Implemented enhancements:**
 
 - feat: add ome\_metadata output to ome-types [\#153](https://github.com/tlambert03/nd2/pull/153) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `nd2-0.7.0/mkdocs.yml` & `nd2-0.7.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/.github/workflows/ci.yml` & `nd2-0.7.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/.github/workflows/cron.yml` & `nd2-0.7.1/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/docs/index.md` & `nd2-0.7.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/docs/styles/extra.css` & `nd2-0.7.1/docs/styles/extra.css`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/scripts/bf_describe.py` & `nd2-0.7.1/scripts/bf_describe.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/scripts/compare.py` & `nd2-0.7.1/scripts/compare.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/scripts/comparison.json` & `nd2-0.7.1/scripts/comparison.json`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/scripts/download_samples.py` & `nd2-0.7.1/scripts/download_samples.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import requests
 
 TEST_DATA = Path(__file__).parent.parent / "tests" / "data"
 URL = "https://www.dropbox.com/sh/pg9my6hnjj918x8/AACiKLlcDsljRgjJOec-9PQwa?dl=1"
 
 # this is just here to invalidate the github actions cache
 # change it when a new file is added to the test data in the dropbox folder
-__HASH__ = "2b6b31e6-8606-42c4-9011-5e233581e53b"
+__HASH__ = "a1b2c3d4-e5f6-g7h8-i9j0-k1l2m3n4o5p6"
 
 
-def main():
+def main() -> None:
     response = requests.get(URL, stream=True)
     total_length = response.headers.get("content-length")
 
     f = BytesIO()
     if total_length is None:  # no content length header
         f.write(response.content)
     else:
```

### Comparing `nd2-0.7.0/scripts/gather.py` & `nd2-0.7.1/scripts/gather.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/scripts/nd2_describe.py` & `nd2-0.7.1/scripts/nd2_describe.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     python scripts/nd2_describe.py > tests/samples_metadata.json
 """
 import struct
 from dataclasses import asdict
 from pathlib import Path
 
 import nd2
-from nd2._pysdk._chunk_decode import iter_chunks
+from nd2._parse._chunk_decode import iter_chunks
 
 
 def _get_version(path):
     with open(path, "rb") as fh:
         if fh.read(4) == b"\xda\xce\xbe\n":
             for name, start, length in iter_chunks(fh):
                 fh.seek(start)
```

### Comparing `nd2-0.7.0/src/nd2/__init__.py` & `nd2-0.7.1/src/nd2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
     "structures",
     "__version__",
 ]
 
 
 from . import structures
 from ._binary import BinaryLayer, BinaryLayers
-from ._pysdk._chunk_decode import rescue_nd2
+from ._parse._chunk_decode import rescue_nd2
 from ._util import AXIS, is_legacy, is_supported_file
 from .nd2file import ND2File, imread
```

### Comparing `nd2-0.7.0/src/nd2/_binary.py` & `nd2-0.7.1/src/nd2/_binary.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Utilities for binary layers in ND2 files."""
 from __future__ import annotations
 
 import io
 import struct
 import warnings
+import zlib
 from typing import TYPE_CHECKING, Iterator, NamedTuple, Sequence, cast, overload
 
 import numpy as np
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
 
-    from ._pysdk._pysdk import ND2Reader as LatestSDKReader
-    from .nd2file import ND2File
 
 I7 = struct.Struct("<" + "I" * 7)
 I9 = struct.Struct("<" + "I" * 9)
 I2 = struct.Struct("<" + "I" * 2)
 
 
 class BinaryLayer(NamedTuple):
@@ -53,21 +52,21 @@
     coordinate_shape : tuple[int, ...]
         The shape of the coordinates for the associated nd2 file.  This is used
         to reshape the data into a 3D array in `asarray`.
     """
 
     data: list[np.ndarray | None]
     name: str
-    comp_name: str
-    comp_order: int
-    color: int
-    color_mode: int
-    state: int
     file_tag: str
-    layer_id: int
+    comp_name: str | None
+    comp_order: int | None
+    color: int | None
+    color_mode: int | None
+    state: int | None
+    layer_id: int | None
     coordinate_shape: tuple[int, ...]
 
     @property
     def frame_shape(self) -> tuple[int, ...]:
         """Shape (Y, X) of each mask in `data`."""
         return next((s.shape for s in self.data if s is not None), (0, 0))
 
@@ -150,89 +149,32 @@
         out = []
         for bin_layer in self._data:
             d = bin_layer.asarray()
             if d is not None:
                 out.append(d)
         return np.stack(out)
 
-    @classmethod
-    def from_nd2file(cls, nd2file: ND2File) -> BinaryLayers | None:
-        """Extract binary layers from an ND2 file."""
-        if nd2file.is_legacy:  # pragma: no cover
-            warnings.warn(
-                "`binary_data` is not supported for legacy ND2 files",
-                UserWarning,
-                stacklevel=2,
-            )
-            return None
-        rdr = cast("LatestSDKReader", nd2file._rdr)
-
-        try:
-            binary_meta = rdr._decode_chunk(
-                b"CustomDataVar|BinaryMetadata_v1!", strip_prefix=True
-            )
-        except KeyError:
-            return None
-
-        try:
-            items: dict = binary_meta["BinaryMetadata_v1"]
-        except KeyError:  # pragma: no cover
-            warnings.warn(
-                "Could not find 'BinaryMetadata_v1' tag, please open an "
-                "issue with this file at https://github.com/tlambert03/nd2/issues/new",
-                stacklevel=2,
-            )
-            return None
-
-        binseqs = sorted(x for x in rdr.chunkmap if b"RleZipBinarySequence" in x)
-        mask_items = []
-        for _, item in sorted(items.items()):
-            key = item["FileTag"].encode()
-            _masks: list[np.ndarray | None] = []
-            for bs in binseqs:
-                if key in bs:
-                    data = rdr._load_chunk(bs)[4:]
-                    _masks.append(_decode_binary_mask(data) if data else None)
-            mask_items.append(
-                BinaryLayer(
-                    data=_masks,
-                    name=item["Name"],
-                    comp_name=item["CompName"],
-                    comp_order=item["CompOrder"],
-                    color_mode=item["ColorMode"],
-                    state=item["State"],
-                    color=item["Color"],
-                    file_tag=key,
-                    layer_id=item["BinLayerID"],
-                    coordinate_shape=nd2file._coord_shape,
-                )
-            )
-
-        return cls(mask_items)
-
 
 def _unpack(stream: io.BufferedIOBase, strct: struct.Struct) -> tuple:
     return strct.unpack(stream.read(strct.size))
 
 
-def _decode_binary_mask(data: bytes, dtype: DTypeLike = "uint16") -> np.ndarray:
+def decode_binary_mask(data: bytes, dtype: DTypeLike = "uint16") -> np.ndarray:
     # this receives data as would be extracted from a
     # `CustomDataSeq|RleZipBinarySequence...` section in the metadata
 
     # NOTE it is up to ND2File to strip the first 4 bytes... and not call this if there
     # is no data (i.e. if the chunk is just '\x00')
-    import zlib
-
     decomp = zlib.decompress(data)
     stream = io.BytesIO(decomp)
 
     # still not sure what _q is
     # tot_bytes should be length of the stream remaining after this
     (v, ncols, nrows, nmasks, tot_bytes, _q, _zero) = _unpack(stream, I7)
-    if v != 3:
+    if v != 3:  # pragma: no cover
         warnings.warn(
             f"Expected first byte to be 3 but got {v}. "
             "Please submit this file :) https://github.com/tlambert03/nd2/issues/.",
             stacklevel=2,
         )
 
     output = np.zeros((nrows, ncols), dtype=dtype)
```

### Comparing `nd2-0.7.0/src/nd2/_clx_lite.py` & `nd2-0.7.1/src/nd2/_parse/_clx_lite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import io
 import re
 import struct
+import zlib
 from typing import TYPE_CHECKING, Any, Callable, Union, cast
 
 if TYPE_CHECKING:
     from typing import Final
 
     JsonValueType = Union[dict[str, "JsonValueType"], int, str, float, None, bool, list]
 
@@ -110,25 +111,25 @@
     stream: io.BytesIO, strip_prefix: bool = True
 ) -> tuple[str, int]:
     header = stream.read(strctBB.size)
     if not header:
         return ("", -1)
 
     data_type, name_length = strctBB.unpack(header)
-    if data_type == ELxLiteVariantType.COMPRESS:
-        # NOTE: the rois.nd2 test file has compressed metadata
-        # in b'CustomData|CustomDescriptionV1_0!'
-        raise NotImplementedError("Compressed metadata not yet implemented.")
     if data_type in (ELxLiteVariantType.DEPRECATED, ELxLiteVariantType.UNKNOWN):
-        raise ValueError(f"Unknown data type in metadata header: {data_type}")
-
-    # name of the section is a utf16 string of length `name_length * 2`
-    name = stream.read(name_length * 2).decode("utf16")[:-1]
-    if strip_prefix:
-        name = lower.sub("", name)
+        raise ValueError(  # pragma: no cover
+            f"Unknown data type in metadata header: {data_type}"
+        )
+    elif data_type == ELxLiteVariantType.COMPRESS:
+        name = ""
+    else:
+        # name of the section is a utf16 string of length `name_length * 2`
+        name = stream.read(name_length * 2).decode("utf16")[:-1]
+        if strip_prefix:
+            name = lower.sub("", name)
     return (name, data_type)
 
 
 # lite variant
 def json_from_clx_lite_variant(
     data: bytes | io.BytesIO, strip_prefix: bool = True, _count: int = 1
 ) -> dict[str, JsonValueType]:
@@ -138,16 +139,23 @@
 
     stream = data if isinstance(data, io.BytesIO) else io.BytesIO(data)
 
     for _ in range(_count):
         curs = stream.tell()
 
         name, data_type = _chunk_name_and_dtype(stream, strip_prefix)
+
+        if data_type == ELxLiteVariantType.COMPRESS:
+            stream.seek(10, 1)
+            deflated = zlib.decompress(stream.read())
+            return json_from_clx_lite_variant(deflated, strip_prefix)
+
         if data_type == -1:
-            break
+            # never seen this, but it's in the sdk
+            break  # pragma: no cover
 
         value: JsonValueType
         if data_type == ELxLiteVariantType.LEVEL:
             item_count, length = strctIQ.unpack(stream.read(strctIQ.size))
             next_data_length = stream.read(length - (stream.tell() - curs))
             val: dict = json_from_clx_lite_variant(
                 next_data_length, strip_prefix, item_count
@@ -161,15 +169,16 @@
                 value = {f"i{n:010}": x for n, x in enumerate(value)}
             else:
                 value = val
 
         elif data_type in _PARSERS:
             value = _PARSERS[data_type](stream)
         else:
-            value = None
+            # also never seen this
+            value = None  # pragma: no cover
         if name == "" and name in output:
             # nd2 uses empty strings as keys for lists
             if not isinstance(output[name], list):
                 output[name] = [output[name]]
             cast(list, output[name]).append(value)
         else:
             output[name] = value
```

### Comparing `nd2-0.7.0/src/nd2/_clx_xml.py` & `nd2-0.7.1/src/nd2/_parse/_clx_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 LOWER = re.compile("^[a-z_]+")
 
 
 def _float_or_nan(x: str) -> float:
     try:
         return float(x)
-    except ValueError:
+    except ValueError:  # pragma: no cover
         return float("nan")
 
 
 # functions to cast CLxvariants to python types
 _XMLCAST: dict[str | None | bytes, Callable[[Any], Scalar]] = {
     "bool": lambda x: x.lower() in {"true", "1"},
     "CLxByteArray": lambda x: bytearray(x, "utf8"),
@@ -146,12 +146,13 @@
                 "MinSrc",
                 "MaxSrc",
             ):
                 if not cval:
                     # skip empty nodes ... the sdk does this too
                     continue
                 cname = f"i{i:010}"
-            if cname in value:
+            if cname in value:  # pragma: no cover
+                # don't see this in tests anymore. but just in case...
                 warnings.warn(f"Duplicate key {cname} in {name}", stacklevel=2)
             value[cname] = cval
 
     return name, value
```

### Comparing `nd2-0.7.0/src/nd2/_ome.py` & `nd2-0.7.1/src/nd2/_ome.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 from ome_types.model.channel import AcquisitionMode, ContrastMethod, IlluminationType
 from ome_types.model.pixels import DimensionOrder
 from ome_types.model.simple_types import UnitsLength, UnitsTime
 
 if TYPE_CHECKING:
     from nd2 import ND2File
 
-    from ._pysdk._pysdk import ND2Reader as LatestSDKReader
-    from ._pysdk._sdk_types import RawMetaDict
-    from .structures import Metadata, ModalityFlags
+    from ._sdk_types import RawMetaDict
+    from .readers import ModernReader
+    from .structures import ModalityFlags
 
 
 def nd2_ome_metadata(f: ND2File) -> m.OME:
     if f.is_legacy:
         raise NotImplementedError("OME metadata is not available for legacy files")
-    rdr = cast("LatestSDKReader", f._rdr)
-    meta = cast("Metadata", f.metadata)
+    rdr = cast("ModernReader", f._rdr)
+    meta = f.metadata
 
     ch0 = next(iter(meta.channels or ()), None)
     channels = [
         m.Channel(
             id=f"Channel:{c_idx}",
             name=ch.channel.name,
             acquisition_mode=ome_acquisition_mode(ch.microscope.modalityFlags),
```

### Comparing `nd2-0.7.0/src/nd2/_util.py` & `nd2-0.7.1/src/nd2/_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,67 @@
 from __future__ import annotations
 
 import math
 import re
+import warnings
 from datetime import datetime
 from itertools import product
-from typing import TYPE_CHECKING, Mapping, NamedTuple
+from typing import TYPE_CHECKING, BinaryIO, NamedTuple, cast
 
 if TYPE_CHECKING:
     from os import PathLike
-    from typing import IO, Any, Callable, ClassVar, Sequence, Union
+    from typing import Any, Callable, ClassVar, Mapping, Sequence, Union
 
-    from ._legacy import LegacyND2Reader
-    from ._pysdk._pysdk import ND2Reader
+    from nd2.readers import ND2Reader
 
-    StrOrBytesPath = Union[str, bytes, PathLike[str], PathLike[bytes]]
+    StrOrPath = Union[str, PathLike]
+    FileOrBinaryIO = Union[StrOrPath, BinaryIO]
 
     ListOfDicts = list[dict[str, Any]]
     DictOfLists = Mapping[str, Sequence[Any]]
     DictOfDicts = Mapping[str, dict[int, Any]]
 
 NEW_HEADER_MAGIC = b"\xda\xce\xbe\n"
 OLD_HEADER_MAGIC = b"\x00\x00\x00\x0c"
 VERSION = re.compile(r"^ND2 FILE SIGNATURE CHUNK NAME01!Ver([\d\.]+)$")
 
 
+def _open_binary(path: StrOrPath) -> BinaryIO:
+    return open(path, "rb")
+
+
 def is_supported_file(
-    path: StrOrBytesPath, open_: Callable[[StrOrBytesPath, str], IO[Any]] = open
+    path: FileOrBinaryIO,
+    open_: Callable[[StrOrPath], BinaryIO] = _open_binary,
 ) -> bool:
     """Return `True` if `path` can be opened as an nd2 file.
 
     Parameters
     ----------
     path : Union[str, bytes, PathLike]
         A path to query
-    open_ : Callable[[StrOrBytesPath, str], IO[Any]]
+    open_ : Callable[[StrOrBytesPath, str], BinaryIO]
         Filesystem opener, by default `builtins.open`
 
     Returns
     -------
     bool
         Whether the can be opened.
     """
-    with open_(path, "rb") as fh:
-        return fh.read(4) in (NEW_HEADER_MAGIC, OLD_HEADER_MAGIC)
+    if hasattr(path, "read"):
+        path = cast("BinaryIO", path)
+        path.seek(0)
+        magic = path.read(4)
+    else:
+        with open_(path) as fh:
+            magic = fh.read(4)
+    return magic in (NEW_HEADER_MAGIC, OLD_HEADER_MAGIC)
 
 
-def is_legacy(path: StrOrBytesPath) -> bool:
+def is_legacy(path: StrOrPath) -> bool:
     """Return `True` if `path` is a legacy ND2 file.
 
     Parameters
     ----------
     path : Union[str, bytes, PathLike]
         A path to query
 
@@ -59,35 +71,24 @@
         Whether the file is a legacy ND2 file.
     """
     with open(path, "rb") as fh:
         return fh.read(4) == OLD_HEADER_MAGIC
 
 
 def get_reader(
-    path: str,
-    validate_frames: bool = False,
-    search_window: int = 100,
-) -> ND2Reader | LegacyND2Reader:
-    with open(path, "rb") as fh:
-        magic_num = fh.read(4)
-        if magic_num == NEW_HEADER_MAGIC:
-            from ._pysdk._pysdk import ND2Reader
-
-            return ND2Reader(
-                path,
-                validate_frames=validate_frames,
-                search_window=search_window,
-            )
-        elif magic_num == OLD_HEADER_MAGIC:
-            from ._legacy._legacy import LegacyND2Reader
-
-            return LegacyND2Reader(path)
-        raise OSError(
-            f"file {path} not recognized as ND2.  First 4 bytes: {magic_num!r}"
-        )
+    path: str, validate_frames: bool = False, search_window: int = 100
+) -> ND2Reader:  # pragma: no cover
+    warnings.warn(
+        "Deprecated, use nd2.readers.ND2Reader.create if you want to "
+        "directly instantiate a reader subclass.",
+        stacklevel=2,
+    )
+    from nd2.readers import ND2Reader
+
+    return ND2Reader.create(path, search_window * 1000 if validate_frames else None)
 
 
 def is_new_format(path: str) -> bool:
     # TODO: this is just for dealing with missing test data
     with open(path, "rb") as fh:
         return fh.read(4) == NEW_HEADER_MAGIC
 
@@ -124,14 +125,18 @@
         "TimeLoop": TIME,
         "XYPosLoop": POSITION,
         "ZStackLoop": Z,
         "NETimeLoop": TIME,
         "CustomLoop": UNKNOWN,
     }
 
+    @classmethod
+    def frame_coords(cls) -> set[str]:
+        return {cls.X, cls.Y, cls.CHANNEL, cls.RGB}
+
 
 class VoxelSize(NamedTuple):
     x: float
     y: float
     z: float
 
 
@@ -147,15 +152,15 @@
 
 def parse_time(time_str: str) -> datetime:
     for fmt_str in TIME_FMT_STRINGS:
         try:
             return datetime.strptime(time_str, fmt_str)
         except ValueError:
             continue
-    raise ValueError(f"Could not parse {time_str}")
+    raise ValueError(f"Could not parse {time_str}")  # pragma: no cover
 
 
 # utils for converting records to dicts, in recorded_data method
 
 
 def convert_records_to_dict_of_lists(
     records: ListOfDicts, null_val: Any = float("nan")
```

### Comparing `nd2-0.7.0/src/nd2/index.py` & `nd2-0.7.1/src/nd2/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 "kb": round(stat.st_size / 1000, 2),
                 "acquired": acquired or "",
                 "experiment": ";".join([f"{t}:{c}" for t, c in exp]),
                 "dtype": str(nd.dtype),
                 "shape": list(shape),
                 "axes": "".join(axes),
                 "binary": binary,
-                "rois": bool(nd.rois),
+                "rois": False if nd.is_legacy else bool(nd.rois),
                 "software_name": software.get("SWNameString", ""),
                 "software_version": software.get("VersionString", ""),
                 "grabber": software.get("GrabberString", ""),
             }
         )
```

### Comparing `nd2-0.7.0/src/nd2/nd2file.py` & `nd2-0.7.1/src/nd2/nd2file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,47 @@
 from __future__ import annotations
 
 import threading
 import warnings
 from itertools import product
-from pathlib import Path
 from typing import TYPE_CHECKING, cast, overload
 
 import numpy as np
 
 from nd2 import _util
 
-from ._pysdk._chunk_decode import ND2_FILE_SIGNATURE, get_version
-from ._util import AXIS, TIME_KEY, is_supported_file
-from .structures import ROI
+from ._util import AXIS, is_supported_file
+from .readers.protocol import ND2Reader
 
 try:
     from functools import cached_property
 except ImportError:
     cached_property = property  # type: ignore
 
 
 if TYPE_CHECKING:
-    import mmap
+    from pathlib import Path
     from typing import Any, Sequence, Sized, SupportsInt
 
     import dask.array
     import dask.array.core
     import xarray as xr
     from ome_types import OME
     from typing_extensions import Literal
 
     from ._binary import BinaryLayers
-    from ._pysdk._pysdk import ND2Reader as LatestSDKReader
-    from ._util import DictOfDicts, DictOfLists, ListOfDicts, StrOrBytesPath
+    from ._util import (
+        DictOfDicts,
+        DictOfLists,
+        FileOrBinaryIO,
+        ListOfDicts,
+        StrOrPath,
+    )
     from .structures import (
+        ROI,
         Attributes,
         ExpLoop,
         FrameMetadata,
         Metadata,
         TextInfo,
         XYPosLoop,
     )
@@ -86,75 +90,73 @@
 
         If `True`, use the SDK to read the file. If `False`, inspects the chunkmap
         and reads from a `numpy.memmap`. If `None` (the default), uses the SDK if
         the file is compressed, otherwise uses the memmap. Note: using
         `read_using_sdk=False` on a compressed file will result in a ValueError.
     """
 
-    _memmap: mmap.mmap
-    _is_legacy: bool
-
     def __init__(
         self,
-        path: Path | str,
+        path: FileOrBinaryIO,
         *,
         validate_frames: bool = False,
         search_window: int = 100,
         read_using_sdk: bool | None = None,
     ) -> None:
         if read_using_sdk is not None:
             warnings.warn(
                 "The `read_using_sdk` argument is deprecated and will be removed in "
                 "a future version.",
                 FutureWarning,
                 stacklevel=2,
             )
-        self._path = str(path)
-        self._rdr = _util.get_reader(
-            self._path,
-            validate_frames=validate_frames,
-            search_window=search_window,
+        self._error_radius: int | None = (
+            search_window * 1000 if validate_frames else None
         )
-        self._closed = False
-        self._is_legacy = "Legacy" in type(self._rdr).__name__
+        self._rdr = ND2Reader.create(path, self._error_radius)
+        self._path = self._rdr._path
         self._lock = threading.RLock()
-        self._version: tuple[int, ...] | None = None
 
     @staticmethod
-    def is_supported_file(path: StrOrBytesPath) -> bool:
+    def is_supported_file(path: StrOrPath) -> bool:
         """Return `True` if the file is supported by this reader."""
         return is_supported_file(path)
 
-    @property
+    @cached_property
     def version(self) -> tuple[int, ...]:
         """Return the file format version as a tuple of ints.
 
         Likely values are:
 
         - `(1, 0)` = a legacy nd2 file (JPEG2000)
         - `(2, 0)`, `(2, 1)` = non-JPEG2000 nd2 with xml metadata
         - `(3, 0)` = new format nd2 file with lite variant metadata
+        - `(-1, -1)` =
+
+        Returns
+        -------
+        tuple[int, ...]
+            The file format version as a tuple of ints.
+
+        Raises
+        ------
+        ValueError
+            If the file is not a valid nd2 file.
         """
-        if self._version is None:
-            try:
-                self._version = get_version(self._rdr._fh or self._rdr._path)
-            except Exception:
-                self._version = (-1, -1)
-                raise
-        return self._version
+        return self._rdr.version()
 
     @property
     def path(self) -> str:
         """Path of the image."""
-        return self._path
+        return str(self._path)
 
     @property
     def is_legacy(self) -> bool:
         """Whether file is a legacy nd2 (JPEG2000) file."""
-        return self._is_legacy
+        return self._rdr.is_legacy()
 
     def open(self) -> None:
         """Open file for reading.
 
         !!! note
 
             Files are best opened using a context manager:
@@ -164,15 +166,14 @@
                 ...
             ```
 
             This will automatically close the file when the context exits.
         """
         if self.closed:
             self._rdr.open()
-            self._closed = False
 
     def close(self) -> None:
         """Close file.
 
         !!! note
 
             Files are best opened using a context manager:
@@ -182,29 +183,29 @@
                 ...
             ```
 
             This will automatically close the file when the context exits.
         """
         if not self.closed:
             self._rdr.close()
-            self._closed = True
 
     @property
     def closed(self) -> bool:
         """Return `True` if the file is closed."""
-        return self._closed
+        return self._rdr._closed
 
     def __enter__(self) -> ND2File:
         """Open file for reading."""
         self.open()
         return self
 
     def __del__(self) -> None:
         """Delete file handle on garbage collection."""
-        if not getattr(self, "_closed", True):
+        # if it came in as an open file handle, it's ok to remain open after deletion
+        if not getattr(self, "closed", True) and not self._rdr._was_open:
             warnings.warn(
                 "ND2File file not closed before garbage collection. "
                 "Please use `with ND2File(...):` context or call `.close()`.",
                 stacklevel=2,
             )
             self._rdr.close()
 
@@ -213,22 +214,25 @@
         self.close()
 
     def __getstate__(self) -> dict[str, Any]:
         """Return state for pickling."""
         state = self.__dict__.copy()
         del state["_rdr"]
         del state["_lock"]
+        state["_closed"] = self.closed
         return state
 
     def __setstate__(self, d: dict[str, Any]) -> None:
         """Load state from pickling."""
+        _was_closed = d.pop("_closed", False)
         self.__dict__ = d
         self._lock = threading.RLock()
-        self._rdr = _util.get_reader(self._path)
-        if self._closed:
+        self._rdr = ND2Reader.create(self._path, self._error_radius)
+
+        if _was_closed:
             self._rdr.close()
 
     @cached_property
     def attributes(self) -> Attributes:
         """Core image attributes.
 
         !!! example "Example Output"
@@ -253,18 +257,18 @@
 
 
         Returns
         -------
         attrs : Attributes
             Core image attributes
         """
-        return self._rdr.attributes
+        return self._rdr.attributes()
 
     @cached_property
-    def text_info(self) -> TextInfo | dict:
+    def text_info(self) -> TextInfo:
         r"""Miscellaneous text info.
 
         ??? example "Example Output"
 
             ```python
             {
                 'description': 'Metadata:\r\nDimensions: T(3) x XY(4) x λ(2) x Z(5)...'
@@ -287,34 +291,15 @@
         """Return dict of `{id: ROI}` for all ROIs found in the metadata.
 
         Returns
         -------
         dict[int, ROI]
             The dict of ROIs is keyed by the ROI ID.
         """
-        key = b"CustomData|RoiMetadata_v1!"
-        if self.is_legacy or key not in self._rdr.chunkmap:  # type: ignore
-            return {}  # pragma: no cover
-
-        data = cast("LatestSDKReader", self._rdr)._decode_chunk(key)
-        data = data.get("RoiMetadata_v1", {}).copy()
-        dicts: list[dict] = []
-        if "Global_Size" in data:
-            dicts.extend(data[f"Global_{i}"] for i in range(data["Global_Size"]))
-        if "2PerMPoint_Size" in data:
-            for i in range(data.get("2PerMPoint_Size", 0)):
-                item: dict = data[f"2PerMPoint_{i}"]
-                dicts.extend(item[str(idx)] for idx in range(item.get("Size", 0)))
-
-        try:
-            _rois = [ROI._from_meta_dict(d) for d in dicts]
-        except Exception as e:  # pragma: no cover
-            return {}
-            raise ValueError(f"Could not parse ROI metadata: {e}") from e
-        return {r.id: r for r in _rois}
+        return {r.id: r for r in self._rdr.rois()}
 
     @cached_property
     def experiment(self) -> list[ExpLoop]:
         """Loop information for each axis of an nD acquisition.
 
         ??? example "Example Output"
 
@@ -408,45 +393,15 @@
         -------
         ListOfDicts | DictOfLists | DictOfDicts
             Tabular data in the format specified by `orient`.
         """
         if orient not in ("records", "dict", "list"):  # pragma: no cover
             raise ValueError("orient must be one of 'records', 'dict', or 'list'")
 
-        if self.is_legacy:  # pragma: no cover
-            warnings.warn(
-                "`recorded_data` is not implemented for legacy ND2 files",
-                UserWarning,
-                stacklevel=2,
-            )
-            return [] if orient == "records" else {}  # type: ignore[return-value]
-
-        rdr = cast("LatestSDKReader", self._rdr)
-        acq_data = rdr._acquisition_data()  # comes back as a dict of lists
-        acq_data.update(rdr._custom_tags())
-
-        img_events = rdr._img_exp_events()
-        if not img_events and orient == "list":
-            # by default, acq_data is already oriented as a dict of lists,
-            # so if we don't have any image events, we can just return it
-            return acq_data
-
-        # re-orient acq_data as a list of dicts, to combine with events
-        records = _util.convert_dict_of_lists_to_records(acq_data)
-        for e in img_events:
-            records.append({TIME_KEY: e.time / 1000, "Events": e.description})
-
-        # sort by time
-        records.sort(key=lambda x: x.get(TIME_KEY, 0))
-
-        if orient == "dict":
-            return _util.convert_records_to_dict_of_dicts(records, null_val=null_value)
-        elif orient == "list":
-            return _util.convert_records_to_dict_of_lists(records, null_val=null_value)
-        return records
+        return self._rdr.events(orient=orient, null_value=null_value)
 
     def unstructured_metadata(
         self,
         *,
         strip_prefix: bool = True,
         include: set[str] | None = None,
         exclude: set[str] | None = None,
@@ -481,55 +436,24 @@
         Returns
         -------
         dict[str, Any]
             A dict of the unstructured metadata, with keys that are the type of the
             metadata chunk (things like 'CustomData|RoiMetadata_v1' or
             'ImageMetadataLV'), and values that are associated metadata chunk.
         """
-        if self.is_legacy:  # pragma: no cover
-            raise NotImplementedError(
-                "unstructured_metadata not available for legacy files"
-            )
-
         if unnest is not None:
             warnings.warn(
                 "The unnest parameter is deprecated, and no longer has any effect.",
                 FutureWarning,
                 stacklevel=2,
             )
-
-        rdr = cast("LatestSDKReader", self._rdr)
-        keys = {
-            k.decode()[:-1]
-            for k in rdr.chunkmap
-            if not k.startswith((b"ImageDataSeq", b"CustomData", ND2_FILE_SIGNATURE))
-        }
-
-        if include:
-            _keys: set[str] = set()
-            for i in include:
-                if i not in keys:
-                    warnings.warn(f"Key {i!r} not found in metadata", stacklevel=2)
-                else:
-                    _keys.add(i)
-            keys = _keys
-        if exclude:
-            keys = {k for k in keys if k not in exclude}
-
-        output: dict[str, Any] = {}
-        for key in sorted(keys):
-            name = f"{key}!".encode()
-            try:
-                output[key] = rdr._decode_chunk(name, strip_prefix=strip_prefix)
-            except Exception:  # pragma: no cover
-                output[key] = rdr._load_chunk(name)
-        return output
+        return self._rdr.unstructured_metadata(strip_prefix, include, exclude)
 
     @cached_property
-    def metadata(self) -> Metadata | dict:
+    def metadata(self) -> Metadata:
         """Various metadata (will be `dict` only if legacy format).
 
         ??? example "Example output"
 
             ```python
             Metadata(
                 contents=Contents(channelCount=2, frameCount=15),
@@ -798,15 +722,15 @@
             else seq_index,
         )
         return self._rdr.frame_metadata(idx)
 
     @cached_property
     def custom_data(self) -> dict[str, Any]:
         """Dict of various unstructured custom metadata."""
-        return self._rdr._custom_data()
+        return self._rdr.custom_data()
 
     @cached_property
     def ndim(self) -> int:
         """Number of dimensions (i.e. `len(`[`self.shape`][nd2.ND2File.shape]`)`)."""
         return len(self.shape)
 
     @cached_property
@@ -816,14 +740,17 @@
         Examples
         --------
         >>> ndfile.shape
         (3, 5, 2, 512, 512)
         """
         return self._coord_shape + self._frame_shape
 
+    def _coord_info(self) -> list[tuple[int, str, int]]:
+        return [(i, x.type, x.count) for i, x in enumerate(self.experiment)]
+
     @cached_property
     def sizes(self) -> dict[str, int]:
         """Names and sizes for each axis.
 
         This is an ordered dict, with the same order
         as the corresponding [shape][nd2.ND2File.shape]
 
@@ -831,15 +758,15 @@
         --------
         >>> ndfile.sizes
         {'T': 3, 'Z': 5, 'C': 2, 'Y': 512, 'X': 512}
         >>> ndfile.shape
         (3, 5, 2, 512, 512)
         """
         attrs = self.attributes
-        dims = {AXIS._MAP[c[1]]: c[2] for c in self._rdr._coord_info()}
+        dims = {AXIS._MAP[c[1]]: c[2] for c in self._coord_info()}
         dims[AXIS.CHANNEL] = (
             dims.pop(AXIS.CHANNEL)
             if AXIS.CHANNEL in dims
             else (attrs.channelCount or 1)
         )
         dims[AXIS.Y] = attrs.heightPx
         dims[AXIS.X] = attrs.widthPx or -1
@@ -1097,44 +1024,40 @@
             },
         )
         if delayed and position is not None and AXIS.POSITION in coords:
             x = x.isel({AXIS.POSITION: [position]})
         return x.squeeze() if squeeze else x
 
     @property
-    def _frame_coords(self) -> set[str]:
-        return {AXIS.X, AXIS.Y, AXIS.CHANNEL, AXIS.RGB}
-
-    @property
     def _raw_frame_shape(self) -> tuple[int, int, int, int]:
         """Sizes of each frame coordinate, prior to reshape."""
         attr = self.attributes
         return (
             attr.heightPx,
             attr.widthPx or -1,
             attr.channelCount or 1,
             self.components_per_channel,
         )
 
     @property
     def _frame_shape(self) -> tuple[int, ...]:
         """Sizes of each frame coordinate, after reshape & squeeze."""
-        return tuple(v for k, v in self.sizes.items() if k in self._frame_coords)
+        return tuple(v for k, v in self.sizes.items() if k in AXIS.frame_coords())
 
     @cached_property
     def _coord_shape(self) -> tuple[int, ...]:
         """Sizes of each *non-frame* coordinate."""
-        return tuple(v for k, v in self.sizes.items() if k not in self._frame_coords)
+        return tuple(v for k, v in self.sizes.items() if k not in AXIS.frame_coords())
 
     @property
     def _frame_count(self) -> int:
         return int(np.prod(self._coord_shape))
 
     def _get_frame(self, index: SupportsInt) -> np.ndarray:
-        frame = self._rdr._read_image(int(index))
+        frame = self._rdr.read_frame(int(index))
         frame.shape = self._raw_frame_shape
         return frame.transpose((2, 0, 1, 3)).squeeze()
 
     def _expand_coords(self, squeeze: bool = True) -> dict:
         """Return a dict that can be used as the coords argument to xr.DataArray.
 
         Parameters
@@ -1191,21 +1114,21 @@
                     break
         if loop is None:
             return ["XYPos:0"]
         return [p.name or f"XYPos:{i}" for i, p in enumerate(loop.parameters.points)]
 
     @property
     def _channel_names(self) -> list[str]:
-        return self._rdr.channel_names()
+        return [c.channel.name for c in self.metadata.channels or []]
 
     def __repr__(self) -> str:
         """Return a string representation of the ND2File."""
         try:
             details = " (closed)" if self.closed else f" {self.dtype}: {self.sizes!r}"
-            extra = f": {Path(self.path).name!r}{details}"
+            extra = f": {self._path.name!r}{details}"
         except Exception:
             extra = ""
         return f"<ND2File at {hex(id(self))}{extra}>"
 
     @property
     def recorded_data(self) -> DictOfLists:
         """Return tabular data recorded for each frame of the experiment.
@@ -1257,17 +1180,15 @@
         comp_name='Widefield Green', comp_order=2, color=65280, color_mode=0,
         state=524288, file_tag='RleZipBinarySequence_1_v1', layer_id=2)
         >>> f.binary_data[0].data  # list of arrays
         >>> np.asarray(f.binary_data[0])  # just the first binary mask
         >>> np.asarray(f.binary_data).shape  # cast all layers to array
         (4, 3, 4, 5, 32, 32)
         """
-        from ._binary import BinaryLayers
-
-        return BinaryLayers.from_nd2file(self)
+        return self._rdr.binary_data()
 
     def ome_metadata(self) -> OME:
         """Return OME metadata for the file."""
         from ._ome import nd2_ome_metadata
 
         return nd2_ome_metadata(self)
```

### Comparing `nd2-0.7.0/src/nd2/structures.py` & `nd2-0.7.1/src/nd2/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import builtins
 from dataclasses import dataclass, field
 from enum import IntEnum
 from typing import TYPE_CHECKING, NamedTuple, Union
 
 from typing_extensions import Literal, TypedDict
 
-from ._pysdk._sdk_types import EventMeaning, StimulationType
+from ._sdk_types import EventMeaning, StimulationType
 
 if TYPE_CHECKING:
-    from ._pysdk._sdk_types import AxisInterpretation, LoopTypeString
+    from ._sdk_types import AxisInterpretation, LoopTypeString
 
 
 class TextInfo(TypedDict, total=False):
     imageId: str
     type: str
     group: str
     sampleId: str
```

### Comparing `nd2-0.7.0/src/nd2/_legacy/_legacy_xml.py` & `nd2-0.7.1/src/nd2/_parse/_legacy_xml.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/src/nd2/_pysdk/_chunk_decode.py` & `nd2-0.7.1/src/nd2/_parse/_chunk_decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """FIXME: this has a lot of code duplication with _chunkmap.py."""
 from __future__ import annotations
 
 import mmap
 import struct
-from contextlib import contextmanager
-from io import BufferedReader
+from contextlib import contextmanager, nullcontext
 from pathlib import Path
-from typing import TYPE_CHECKING, BinaryIO, Iterator, cast
+from typing import TYPE_CHECKING, BinaryIO, ContextManager, cast
 
 import numpy as np
 
 if TYPE_CHECKING:
     from os import PathLike
-    from typing import Final
+    from typing import Final, Iterator
 
     from numpy.typing import DTypeLike
 
     StrOrBytesPath = str | bytes | PathLike[str] | PathLike[bytes]
 
     StartFileChunk = tuple[int, int, int, bytes, bytes]
     #              = (magic, name_length, data_length, name, data)
@@ -67,50 +66,54 @@
 
 
 def get_version(fh: BinaryIO | StrOrBytesPath) -> tuple[int, int]:
     """Get the version of the ND2 file or raise an exception.
 
     Parameters
     ----------
-    fh : BufferedReader | str | bytes | Path
+    fh : BinaryIO | str | bytes | Path
         The file handle or path to the ND2 file.
 
     Returns
     -------
     tuple[int, int]
         (major, minor) version of the ND2 file
 
     Raises
     ------
     ValueError
         If the file is not a valid ND2 file or the header chunk is corrupt.
     """
-    if not isinstance(fh, (BinaryIO, BufferedReader)):
-        with open(fh, "rb") as fh:
-            chunk = START_FILE_CHUNK.unpack(fh.read(START_FILE_CHUNK.size))
+    if hasattr(fh, "read"):
+        ctx: ContextManager[BinaryIO] = nullcontext(cast("BinaryIO", fh))
     else:
-        # leave it open if it came in open
+        ctx = open(fh, "rb")
+
+    with ctx as fh:
         fh.seek(0)
+        fname = str(fh.name)
         chunk = START_FILE_CHUNK.unpack(fh.read(START_FILE_CHUNK.size))
 
     magic, name_length, data_length, name, data = cast("StartFileChunk", chunk)
 
     # sanity checks
     if magic != ND2_CHUNK_MAGIC:
         if magic == JP2_MAGIC:
             return (1, 0)  # legacy JP2 files are version 1.0
-        raise ValueError(f"Not a valid ND2 file: {fh.name}. (magic: {magic!r})")
+        raise ValueError(  # pragma: no cover
+            f"Not a valid ND2 file: {fname}. (magic: {magic!r})"
+        )
     if name_length != 32 or data_length != 64 or name != ND2_FILE_SIGNATURE:
-        raise ValueError(f"Corrupt ND2 file header chunk: {fh.name}")
+        raise ValueError(f"Corrupt ND2 file header chunk: {fname}")  # pragma: no cover
 
     # data will now be something like Ver2.0, Ver3.0, etc.
     return (int(chr(data[3])), int(chr(data[5])))
 
 
-def get_chunkmap(fh: BufferedReader, error_radius: int | None = None) -> ChunkMap:
+def get_chunkmap(fh: BinaryIO, error_radius: int | None = None) -> ChunkMap:
     """Read the map of the chunks at the end of an ND2 file.
 
     A Chunkmap is mapping of chunk names (bytes) to (offset, size) pairs.
 
     ```python
     {
       b'ImageTextInfoLV!': (13041664, 2128),
@@ -118,15 +121,15 @@
       b'ImageMetadataSeq|0!': (237568, 33412),
       ...
     }
     ```
 
     Parameters
     ----------
-    fh : BufferedReader
+    fh : BinaryIO
         An open nd2 file.  File is assumed to be a valid ND2 file.  (use `get_version`)
     error_radius : int, optional
         If b"ND2 FILEMAP SIGNATURE NAME 0001!" is not found at expected location and
         `error_radius` is not None, then an area of +/- `error_radius` bytes will be
         searched for the signature.
 
     Returns
@@ -138,15 +141,15 @@
     ------
     ValueError
         If the file is not a valid ND2 file or the chunkmap is corrupt.
     """
     # the last (32,8) bytes of the file contain the (signature, location) of chunkmap
     fh.seek(-40, 2)
     sig, location = SIG_CHUNKMAP_LOC.unpack(fh.read(SIG_CHUNKMAP_LOC.size))
-    if sig != ND2_CHUNKMAP_SIGNATURE:
+    if sig != ND2_CHUNKMAP_SIGNATURE:  # pragma: no cover
         raise ValueError(f"Invalid ChunkMap signature {sig!r} in file {fh.name!r}")
 
     # get all of the data in the chunkmap
     chunkmap_data = _robustly_read_named_chunk(
         fh, location, search_radius=error_radius, expect_name=ND2_FILEMAP_SIGNATURE
     )
 
@@ -172,30 +175,30 @@
             size = -1
         chunk_map[chunk_name] = (offset, size)
         current_position = p + QQ.size
     return chunk_map
 
 
 def read_nd2_chunk(
-    fh: BufferedReader, start_position: int, expect_name: bytes | None = None
+    fh: BinaryIO, start_position: int, expect_name: bytes | None = None
 ) -> bytes:
     """Read a single chunk in an ND2 file at `start_position`.
 
     Each data chunk starts with:
       - 4 bytes: CHUNK_MAGIC -> 0x0ABECEDA (big endian: 0xDACEBE0A)
       - 4 bytes: length of the chunk header (this section contains the chunk name...)
       - 8 bytes: length of chunk following the header, up to the next CHUNK_MAGIC
 
     For example:
         magic    name_len <-  data_len   -> <- NameChunk (name_len long) ...
         DACEBE0A 20100000 D00F0000 00000000 004E4432 20434855 4E4B204D 41...
 
     Parameters
     ----------
-    fh : BufferedReader
+    fh : BinaryIO
         An open nd2 file.  File is assumed to be a valid ND2 file.  (use `get_version`)
     start_position : int
         The position in the file to start reading the chunk.
     expect_name : bytes | None
         If not None, the chunk name must match this value.
 
     Returns
@@ -225,28 +228,28 @@
                 f"Expected chunk name {expect_name!r} at {start_position}"
                 f" but found {_name!r}"
             )
     return fh.read(data_length)  # then read data_length bytes
 
 
 def _robustly_read_named_chunk(
-    fh: BufferedReader,
+    fh: BinaryIO,
     start_position: int,
     expect_name: bytes = ND2_FILEMAP_SIGNATURE,
     search_radius: int | None = None,
 ) -> bytes:
     """Read nd2 chunk at start_position ND2 file, with error robustness.
 
     Same logic as _read_nd2_chunk, but allows for a search radius around the
     expected location of the chunkmap if a chunk named `expect_name` is not found at
     the expected location.
 
     Parameters
     ----------
-    fh : BufferedReader
+    fh : BinaryIO
         An open nd2 file.  File is assumed to be a valid ND2 file.
     start_position : int
         The position in the file to start reading the chunk.
     expect_name : bytes
         The name of the chunk to expect at `start_position` + 16 bytes.
     search_radius : int | None
         If not None, and `expect_name` is not found at `start_position` + 16 bytes,
@@ -272,24 +275,24 @@
             else:
                 fixed_position = new_start + idx - CHUNK_HEADER.size
                 return read_nd2_chunk(fh, fixed_position)
 
         raise ValueError(err_msg) from e
 
 
-def iter_chunks(handle: BufferedReader) -> Iterator[tuple[str, int, int]]:
+def iter_chunks(handle: BinaryIO) -> Iterator[tuple[str, int, int]]:
     file_size = handle.seek(0, 2)
     handle.seek(0)
     pos = 0
     while True:
         magic, shift, length = CHUNK_HEADER.unpack(handle.read(CHUNK_HEADER.size))
         if magic:
             try:
                 name = handle.read(shift).split(b"\x00", 1)[0].decode("utf-8")
-            except UnicodeDecodeError:
+            except UnicodeDecodeError:  # pragma: no cover
                 name = "?"
             yield (name, pos + +CHUNK_HEADER.size + shift, length)
         pos += CHUNK_HEADER.size + shift + length
         if pos >= file_size:
             break
         handle.seek(pos)
 
@@ -383,15 +386,15 @@
                         shape = frame_shape or ((length - 8) // dtype.itemsize,)
                         yield np.ndarray(
                             shape=shape,
                             dtype=dtype,
                             buffer=mm,
                             offset=end_hdr + shift + 8,
                         )
-                    except TypeError as e:
+                    except TypeError as e:  # pragma: no cover
                         # buffer is likely too small
                         if verbose:
                             print(f"Error at offset {offset}: {e}")
                     iters += 1
             elif verbose:
                 print(f"Found chunk at offset {offset} with no image data")
```

### Comparing `nd2-0.7.0/src/nd2/_pysdk/_parse.py` & `nd2-0.7.1/src/nd2/_parse/_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,20 @@
 from math import ceil
 from struct import Struct
 from typing import TYPE_CHECKING, Iterable, cast
 
 import numpy as np
 
 from nd2 import structures as strct
-
-from ._sdk_types import ELxModalityMask, EventMeaning, StimulationType
+from nd2._sdk_types import ELxModalityMask, EventMeaning, StimulationType
 
 if TYPE_CHECKING:
     from typing_extensions import TypeGuard
 
-    from nd2.structures import ExpLoop, XYPosLoopParams
-
-    from ._sdk_types import (
+    from nd2._sdk_types import (
         AxisInterpretation,
         CompressionType,
         FilterDict,
         FluorescentProbeDict,
         GlobalMetadata,
         LoopTypeString,
         NETimeLoopPars,
@@ -36,14 +33,15 @@
         RawTextInfoDict,
         SpectLoopPars,
         SpectrumDict,
         TimeLoopPars,
         XYPosLoopPars,
         ZStackLoopPars,
     )
+    from nd2.structures import ExpLoop, XYPosLoopParams
 
 
 strctd = Struct("d")
 
 
 def _parse_xy_pos_loop(
     item: XYPosLoopPars, valid: list[int] | dict[str, bool]
```

### Comparing `nd2-0.7.0/src/nd2/_pysdk/_pysdk.py` & `nd2-0.7.1/src/nd2/readers/_modern/modern_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 from __future__ import annotations
 
-import mmap
 import os
 import warnings
+import zlib
 from itertools import product
-from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Sequence, cast
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence, cast
 
 import numpy as np
 
-from nd2 import structures
-from nd2._clx_lite import json_from_clx_lite_variant
-from nd2._clx_xml import json_from_clx_variant
-from nd2._pysdk._chunk_decode import (
+from nd2 import _util, structures
+from nd2._parse._chunk_decode import (
+    ND2_FILE_SIGNATURE,
     _robustly_read_named_chunk,
     get_chunkmap,
-    get_version,
     read_nd2_chunk,
 )
-from nd2._pysdk._parse import (
+from nd2._parse._clx_lite import json_from_clx_lite_variant
+from nd2._parse._clx_xml import json_from_clx_variant
+from nd2._parse._parse import (
     load_attributes,
     load_events,
     load_experiment,
     load_frame_metadata,
     load_global_metadata,
     load_metadata,
     load_text_info,
 )
-from nd2._util import TIME_KEY, Z_SERIES_KEY
+from nd2.readers.protocol import ND2Reader
+from nd2.structures import ROI
 
 if TYPE_CHECKING:
     import datetime
-    from io import BufferedReader
     from os import PathLike
-    from typing import Any
 
-    from typing_extensions import TypeAlias
+    from typing_extensions import Literal, TypeAlias
 
-    from ._chunk_decode import ChunkMap
-    from ._sdk_types import (
+    from nd2._binary import BinaryLayers
+    from nd2._parse._chunk_decode import ChunkMap
+    from nd2._sdk_types import (
+        BinaryMetaDict,
         GlobalMetadata,
         RawAttributesDict,
         RawExperimentDict,
         RawExperimentRecordDict,
         RawMetaDict,
         RawTagDict,
         RawTextInfoDict,
     )
+    from nd2._util import FileOrBinaryIO
 
     StrOrBytesPath: TypeAlias = str | bytes | PathLike[str] | PathLike[bytes]
     StartFileChunk: TypeAlias = tuple[int, int, int, bytes, bytes]
 
 
-class ND2Reader:
-    def __init__(
-        self, path: str | Path, validate_frames: bool = False, search_window: int = 100
-    ) -> None:
-        self._path = Path(path)
-        self._fh: BufferedReader | None = None
-        self._mmap: mmap.mmap | None = None
-        self._chunkmap: ChunkMap = {}
+class ModernReader(ND2Reader):
+    HEADER_MAGIC = _util.NEW_HEADER_MAGIC
+
+    def __init__(self, path: FileOrBinaryIO, error_radius: int | None = None) -> None:
+        super().__init__(path, error_radius)
+
         self._cached_decoded_chunks: dict[bytes, Any] = {}
-        self._error_radius: int | None = (
-            search_window * 1000 if validate_frames else None
-        )
 
-        self._version: tuple[int, int] | None = None
         self._attributes: structures.Attributes | None = None
         self._experiment: list[structures.ExpLoop] | None = None
         self._text_info: structures.TextInfo | None = None
         self._metadata: structures.Metadata | None = None
         self._events: list[structures.ExperimentEvent] | None = None
 
         self._global_metadata: GlobalMetadata | None = None
@@ -80,73 +75,54 @@
         self._frame_times: list[float] | None = None
         # these caches could be removed... they aren't really used
         self._raw_attributes: RawAttributesDict | None = None
         self._raw_experiment: RawExperimentDict | None = None
         self._raw_text_info: RawTextInfoDict | None = None
         self._raw_image_metadata: RawMetaDict | None = None
 
-        self.open()
-
-    def open(self) -> None:
-        if self._fh is None:
-            self._fh = open(self._path, "rb")
-            self._mmap = mmap.mmap(self._fh.fileno(), 0, access=mmap.ACCESS_READ)
-
-    def close(self) -> None:
-        if self._fh is not None:
-            self._fh.close()
-            self._fh = None
-        if self._mmap is not None:
-            self._mmap.close()
-            self._mmap = None
-
-    def __enter__(self) -> ND2Reader:
-        self.open()
-        return self
-
-    def __exit__(self, *_: Any) -> None:
-        self.close()
-
     @property
     def chunkmap(self) -> ChunkMap:
         """Load and return the chunkmap.
 
         a Chunkmap is mapping of chunk names (bytes) to (offset, size) pairs.
         {
             b'ImageTextInfoLV!': (13041664, 2128),
             b'ImageTextInfo!': (13037568, 1884),
             b'ImageMetadataSeq|0!': (237568, 33412),
             ...
         }
         """
         if not self._chunkmap:
-            if self._fh is None:
+            if self._fh is None:  # pragma: no cover
                 raise OSError("File not open")
             self._chunkmap = get_chunkmap(self._fh, error_radius=self._error_radius)
-        return self._chunkmap
+        return cast("ChunkMap", self._chunkmap)
 
-    @property
     def attributes(self) -> structures.Attributes:
         """Load and return the image attributes."""
         if self._attributes is None:
-            k = b"ImageAttributesLV!" if self.version >= (3, 0) else b"ImageAttributes!"
+            k = (
+                b"ImageAttributesLV!"
+                if self.version() >= (3, 0)
+                else b"ImageAttributes!"
+            )
             attrs = self._decode_chunk(k, strip_prefix=False)
             attrs = attrs.get("SLxImageAttributes", attrs)  # for v3 only
-            self._raw_attributes = cast("RawAttributesDict", attrs)
             raw_meta = self._cached_raw_metadata()  # ugly
             n_channels = raw_meta.get("sPicturePlanes", {}).get("uiCount", 1)
+            self._raw_attributes = cast("RawAttributesDict", attrs)
             self._attributes = load_attributes(self._raw_attributes, n_channels)
         return self._attributes
 
     def _load_chunk(self, name: bytes) -> bytes:
         """Load raw bytes from a specific chunk in the chunkmap.
 
         `name` must be a valid key in the chunkmap.
         """
-        if self._fh is None:
+        if self._fh is None:  # pragma: no cover
             raise OSError("File not open")
 
         try:
             offset = self.chunkmap[name][0]
         except KeyError as e:
             raise KeyError(
                 f"Chunk key {name!r} not found in chunkmap: {set(self.chunkmap)}"
@@ -174,41 +150,30 @@
             if data.startswith(b"<"):
                 decoded: Any = json_from_clx_variant(data, strip_prefix=strip_prefix)
             else:
                 decoded = json_from_clx_lite_variant(data, strip_prefix=strip_prefix)
             self._cached_decoded_chunks[name] = decoded
         return self._cached_decoded_chunks[name]
 
-    @property
-    def version(self) -> tuple[int, int]:
-        """Return the file format version as a tuple of ints."""
-        if self._version is None:
-            try:
-                self._version = get_version(self._fh or self._path)
-            except Exception:
-                self._version = (-1, -1)
-                raise
-        return self._version
-
     def _cached_raw_metadata(self) -> RawMetaDict:
         if self._raw_image_metadata is None:
             k = (
                 b"ImageMetadataSeqLV|0!"
-                if self.version >= (3, 0)
+                if self.version() >= (3, 0)
                 else b"ImageMetadataSeq|0!"
             )
             meta = self._decode_chunk(k, strip_prefix=False)
             meta = meta.get("SLxPictureMetadata", meta)  # for v3 only
             self._raw_image_metadata = cast("RawMetaDict", meta)
         return self._raw_image_metadata
 
     def _cached_global_metadata(self) -> GlobalMetadata:
         if not self._global_metadata:
             self._global_metadata = load_global_metadata(
-                attrs=self.attributes,
+                attrs=self.attributes(),
                 raw_meta=self._cached_raw_metadata(),
                 exp_loops=self.experiment(),
                 text_info=self.text_info(),
             )
             if self._global_metadata["time"]["absoluteJulianDayNumber"] < 1:
                 julian_day = os.stat(self._path).st_ctime / 86400.0 + 2440587.5
                 self._global_metadata["time"]["absoluteJulianDayNumber"] = julian_day
@@ -229,27 +194,27 @@
         loop_indices = self.loop_indices()[seq_index]
         return load_frame_metadata(
             global_meta, self.metadata(), self.experiment(), frame_time, loop_indices
         )
 
     def text_info(self) -> structures.TextInfo:
         if self._text_info is None:
-            k = b"ImageTextInfoLV!" if self.version >= (3, 0) else b"ImageTextInfo!"
+            k = b"ImageTextInfoLV!" if self.version() >= (3, 0) else b"ImageTextInfo!"
             if k not in self.chunkmap:
                 self._text_info = {}
             else:
                 info = self._decode_chunk(k, strip_prefix=False)
                 info = info.get("SLxImageTextInfo", info)  # for v3 only
                 self._raw_text_info = cast("RawTextInfoDict", info)
                 self._text_info = load_text_info(self._raw_text_info)
         return self._text_info
 
     def experiment(self) -> list[structures.ExpLoop]:
         if not self._experiment:
-            k = b"ImageMetadataLV!" if self.version >= (3, 0) else b"ImageMetadata!"
+            k = b"ImageMetadataLV!" if self.version() >= (3, 0) else b"ImageMetadata!"
             if k not in self.chunkmap:
                 self._experiment = []
             else:
                 exp = self._decode_chunk(k, strip_prefix=False)
                 exp = exp.get("SLxExperiment", exp)  # for v3 only
                 self._raw_experiment = cast("RawExperimentDict", exp)
                 self._experiment = load_experiment(0, self._raw_experiment)
@@ -291,34 +256,28 @@
         meta = self.metadata()
         if meta:
             ch = meta.channels
             if ch:
                 return ch[0].volume.axesCalibration
         return (1, 1, 1)
 
-    def channel_names(self) -> list[str]:
-        return [c.channel.name for c in self.metadata().channels or []]
-
     def _coords_from_seq_index(self, seq_index: int) -> tuple[int, ...]:
         """Convert a sequence index to a coordinate tuple."""
         coords: list[int] = []
         for loop in self.experiment():
             coords.append(seq_index % loop.count)
             seq_index //= loop.count
 
         return tuple(coords)
 
     def _coord_size(self) -> int:
         return len(self.experiment())
 
-    def _coord_info(self) -> list[tuple[int, str, int]]:
-        return [(i, x.type, x.count) for i, x in enumerate(self.experiment())]
-
     def _seq_count(self) -> int:
-        # this differs from self.attributes.SequenceCount in that it
+        # this differs from self.attributes().SequenceCount in that it
         # includes the actual number of frames in the experiment,
         # excluding "invalid" frames.
         return int(np.prod([x.count for x in self.experiment()]))
 
     @property
     def _frame_offsets(self) -> dict[int, int]:
         """Return map of frame number to offset in the file."""
@@ -329,25 +288,25 @@
             self._cached_frame_offsets = {
                 int(chunk_key[13:-1]): int(offset + data_offset)
                 for chunk_key, (offset, _) in sorted(self.chunkmap.items())
                 if chunk_key.startswith(b"ImageDataSeq|")
             }
         return self._cached_frame_offsets
 
-    def _read_image(self, index: int) -> np.ndarray:
+    def read_frame(self, index: int) -> np.ndarray:
         """Read a chunk directly without using SDK."""
         if index > self._seq_count():
             raise IndexError(f"Frame out of range: {index}")
-        if not self._fh:
+        if not self._fh:  # pragma: no cover
             raise ValueError("Attempt to read from closed nd2 file")
         offset = self._frame_offsets.get(index, None)
         if offset is None:
             return self._missing_frame(index)
 
-        if self.attributes.compressionType == "lossless":
+        if self.attributes().compressionType == "lossless":
             return self._read_compressed_frame(index)
 
         try:
             return np.ndarray(
                 shape=self._actual_frame_shape(),
                 dtype=self._dtype(),
                 buffer=self._mmap,
@@ -356,54 +315,52 @@
             )
         except TypeError:
             # If the chunkmap is wrong, and the mmap isn't long enough
             # for the requested offset & size, a TypeError is raised.
             return self._missing_frame(index)
 
     def _read_compressed_frame(self, index: int) -> np.ndarray:
-        import zlib
-
         ch = self._load_chunk(f"ImageDataSeq|{index}!".encode())
         return np.ndarray(
             shape=self._actual_frame_shape(),
             dtype=self._dtype(),
             buffer=zlib.decompress(ch[8:]),
             strides=self._strides,
         )
 
     def _missing_frame(self, index: int = 0) -> np.ndarray:
         # TODO: add other modes for filling missing data
         return np.zeros(self._raw_frame_shape(), self._dtype())
 
     def _raw_frame_shape(self) -> tuple[int, ...]:
         if self._raw_frame_shape_ is None:
-            attr = self.attributes
+            attr = self.attributes()
             ncomp = attr.componentCount
             self._raw_frame_shape_ = (
                 attr.heightPx,
                 (attr.widthBytes or 0) // self._bytes_per_pixel() // ncomp,
                 attr.channelCount or 1,
                 ncomp // (attr.channelCount or 1),
             )
         return self._raw_frame_shape_
 
     def _bytes_per_pixel(self) -> int:
-        return self.attributes.bitsPerComponentInMemory // 8
+        return self.attributes().bitsPerComponentInMemory // 8
 
     def _dtype(self) -> np.dtype:
         if self._dtype_ is None:
-            a = self.attributes
+            a = self.attributes()
             d = a.pixelDataType[0] if a.pixelDataType else "u"
             self._dtype_ = np.dtype(f"{d}{self._bytes_per_pixel()}")
         return self._dtype_
 
     @property
     def _strides(self) -> tuple[int, ...] | None:
         if self._strides_ is None:
-            a = self.attributes
+            a = self.attributes()
             widthP = a.widthPx
             widthB = a.widthBytes
             if not (widthP and widthB):
                 self._strides_ = None
             else:
                 bypc = self._bytes_per_pixel()
                 compCount = a.componentCount
@@ -416,23 +373,23 @@
                         compCount * bypc,
                         compCount // (a.channelCount or 1) * bypc,
                         bypc,
                     )
         return self._strides_
 
     def _actual_frame_shape(self) -> tuple[int, ...]:
-        attr = self.attributes
+        attr = self.attributes()
         return (
             attr.heightPx,
             attr.widthPx or 1,
             attr.channelCount or 1,
             attr.componentCount // (attr.channelCount or 1),
         )
 
-    def _custom_data(self) -> dict[str, Any]:
+    def custom_data(self) -> dict[str, Any]:
         return {
             k.decode()[14:-1]: self._decode_chunk(k)
             for k in self.chunkmap
             if k.startswith(b"CustomDataVar|")
         }
 
     def _acquisition_data(self) -> dict[str, Sequence[Any]]:
@@ -442,15 +399,15 @@
             "Time [s]": [0.0, 0.0, 0.0, ...],
             "Z-Series": [-1.0, 0., 1.0, ...],
         }
         """
         data: dict[str, np.ndarray | Sequence] = {}
         frame_times = self._cached_frame_times()
         if frame_times:
-            data[TIME_KEY] = [x / 1000 for x in frame_times]
+            data[_util.TIME_KEY] = [x / 1000 for x in frame_times]
 
         # FIXME: this whole thing is dumb... must be a better way
         experiment = self.experiment()
         for i, z_loop in enumerate(experiment):
             if not isinstance(z_loop, structures.ZStackLoop):
                 continue
 
@@ -468,23 +425,25 @@
                 for n, _loop in enumerate(experiment):
                     if n == z_idx:
                         return _zp[seq_index % _loop.count]
                     seq_index //= _loop.count
                 raise ValueError("Invalid sequence index or z_idx")
 
             seq_count = self._seq_count()
-            data[Z_SERIES_KEY] = np.array([_seq_z_pos(i) for i in range(seq_count)])
+            data[_util.Z_SERIES_KEY] = np.array(
+                [_seq_z_pos(i) for i in range(seq_count)]
+            )
 
         return data  # type: ignore [return-value]
 
     def _custom_tags(self) -> dict[str, Any]:
         """Return tags mentioned in in CustomDataVar|CustomDataV2_0.
 
         This is a dict of {header: [values]}, where
-        len([values]) == self.attributes.sequenceCount
+        len([values]) == self.attributes().sequenceCount
 
         {
             "Camera_ExposureTime1": [0.0, 0.0, 0.0, ...],
             "PFS_OFFSET": [-1.0, 0., 1.0, ...],
             "PFS_STATUS": [0, 0, 0, ...],
         }
         """
@@ -509,37 +468,47 @@
         # {
         #     'Tag0': {'ID': 'Camera_ExposureTime1', 'Type': 3, ... },
         #     'Tag1': {'ID': 'PFS_OFFSET', 'Type': 2, 'Group': 0, 'Size': 1, ...},
         #     'Tag2': {'ID': 'PFS_STATUS', 'Type': 2, 'Group': 0, 'Size': 1, ...},
         # }
         tags = cast("Iterable[RawTagDict]", cd["CustomTagDescription_v1.0"].values())
         for tag in tags:
-            if tag["Type"] == 1:
-                warnings.warn(
-                    f"{tag['Desc']!r} column skipped: "
-                    "(parsing string data is not yet implemented).  Please open an "
-                    "issue with this nd2 file at "
-                    "https://github.com/tlambert03/nd2/issues/new",
-                    stacklevel=2,
-                )
-                continue
-
             col_header = tag["Desc"]
             if col_header in data:  # pragma: no cover
                 # sourcery skip: hoist-if-from-if
                 col_header = tag["ID"]
                 if col_header in data:
                     col_header = f"{tag['Desc']} ({tag['ID']})"
 
             if tag["Unit"].strip():
                 col_header += f" [{tag['Unit']}]"
 
             buffer_ = self._load_chunk(f"CustomData|{tag['ID']}!".encode())
-            dtype = {3: np.float64, 2: np.int32}[tag["Type"]]
-            data[col_header] = np.frombuffer(buffer_, dtype=dtype, count=tag["Size"])
+            count = tag["Size"]
+            if tag["Type"] == 1:
+                # string data, so far I've only seen this as wide-strings of utf-16
+                # in 512 byte chunks. (I'm not sure if this is always the case)
+                try:
+                    chunk_size = len(buffer_) // count
+                    rows: Any = []
+                    for i in range(count):
+                        word = buffer_[i * chunk_size : (i + 1) * chunk_size]
+                        rows.append(word.decode("utf-16").split("\x00", 1)[0])
+                except Exception as e:  # pragma: no cover
+                    warnings.warn(
+                        f"Failed to parse {tag['Desc']!r} column: {e}. Please open an "
+                        "issue with this nd2 file at "
+                        "https://github.com/tlambert03/nd2/issues/new",
+                        stacklevel=2,
+                    )
+                    continue
+            else:
+                dtype = {3: np.float64, 2: np.int32}[tag["Type"]]
+                rows = np.frombuffer(buffer_, dtype=dtype, count=count)
+            data[col_header] = rows
 
         return data
 
     def _app_info(self) -> dict:
         """Return a dict of app info."""
         k = b"CustomDataVar|AppInfo_V1_0!"
         return self._decode_chunk(k) if k in self.chunkmap else {}
@@ -547,23 +516,145 @@
     def _acquisition_date(self) -> datetime.datetime | str | None:
         """Try to extract acquisition date.
 
         A best effort is made to extract a datetime object from the date string,
         but if that fails, the raw string is returned.  Use isinstance() to
         be safe.
         """
-        from nd2._util import parse_time
-
         date = self.text_info().get("date")
         if date:
             try:
-                return parse_time(date)
+                return _util.parse_time(date)
             except ValueError:
                 return date
 
         time = self._cached_global_metadata().get("time", {})
         jdn = time.get("absoluteJulianDayNumber")
         if jdn:
-            from nd2._util import jdn_to_datetime_utc
-
-            return jdn_to_datetime_utc(jdn)
+            return _util.jdn_to_datetime_utc(jdn)
         return None
+
+    def binary_data(self) -> BinaryLayers | None:
+        from nd2._binary import BinaryLayer, BinaryLayers, decode_binary_mask
+
+        chunk_key = b"CustomDataVar|BinaryMetadata_v1!"
+        if chunk_key not in self.chunkmap:
+            return None
+        binary_meta = self._decode_chunk(chunk_key, strip_prefix=True)
+
+        try:
+            items = cast("dict[str, BinaryMetaDict]", binary_meta["BinaryMetadata_v1"])
+        except KeyError:  # pragma: no cover
+            warnings.warn(
+                "Could not find 'BinaryMetadata_v1' tag, please open an "
+                "issue with this file at https://github.com/tlambert03/nd2/issues/new",
+                stacklevel=2,
+            )
+            return None
+
+        mask_items = []
+        coord_shape = tuple(x.count for x in self.experiment())
+        for _, item in sorted(items.items()):
+            # something like: RleZipBinarySequence_1bd900c
+            key = item["FileTag"]
+            _masks: list[np.ndarray | None] = []
+            for plane in range(self._seq_count()):
+                # this will be something like
+                # b'CustomDataSeq|RleZipBinarySequence_1bd900c|1153!
+                chunk_key = f"CustomDataSeq|{key}|{plane}!".encode()
+                data = self._load_chunk(chunk_key)[4:]
+                _masks.append(decode_binary_mask(data) if data else None)
+
+            mask_items.append(
+                BinaryLayer(
+                    data=_masks,
+                    file_tag=key,
+                    name=item["Name"],
+                    comp_name=item.get("CompName"),
+                    comp_order=item.get("CompOrder"),
+                    color_mode=item.get("ColorMode"),
+                    state=item.get("State"),
+                    color=item.get("Color"),
+                    layer_id=item.get("BinLayerID"),
+                    coordinate_shape=coord_shape,
+                )
+            )
+
+        return BinaryLayers(mask_items)
+
+    def events(
+        self, orient: Literal["records", "list", "dict"], null_value: Any
+    ) -> list | Mapping:
+        acq_data = self._acquisition_data()  # comes back as a dict of lists
+        acq_data.update(self._custom_tags())
+
+        img_events = self._img_exp_events()
+        if not img_events and orient == "list":
+            # by default, acq_data is already oriented as a dict of lists,
+            # so if we don't have any image events, we can just return it
+            return acq_data
+
+        # re-orient acq_data as a list of dicts, to combine with events
+        records = _util.convert_dict_of_lists_to_records(acq_data)
+        for e in img_events:
+            records.append({_util.TIME_KEY: e.time / 1000, "Events": e.description})
+
+        # sort by time
+        records.sort(key=lambda x: x.get(_util.TIME_KEY, 0))
+
+        if orient == "dict":
+            return _util.convert_records_to_dict_of_dicts(records, null_val=null_value)
+        elif orient == "list":
+            return _util.convert_records_to_dict_of_lists(records, null_val=null_value)
+        return records
+
+    def rois(self) -> list[ROI]:
+        key = b"CustomData|RoiMetadata_v1!"
+        if key not in self.chunkmap:
+            return []  # pragma: no cover
+
+        data = self._decode_chunk(key)
+        data = data.get("RoiMetadata_v1", {}).copy()
+        dicts: list[dict] = []
+        if "Global_Size" in data:
+            dicts.extend(data[f"Global_{i}"] for i in range(data["Global_Size"]))
+        if "2PerMPoint_Size" in data:
+            for i in range(data.get("2PerMPoint_Size", 0)):
+                item: dict = data[f"2PerMPoint_{i}"]
+                dicts.extend(item[str(idx)] for idx in range(item.get("Size", 0)))
+
+        try:
+            return [ROI._from_meta_dict(d) for d in dicts]
+        except Exception as e:  # pragma: no cover
+            raise ValueError(f"Could not parse ROI metadata: {e}") from e
+
+    def unstructured_metadata(
+        self,
+        strip_prefix: bool = True,
+        include: set[str] | None = None,
+        exclude: set[str] | None = None,
+    ) -> dict[str, Any]:
+        keys = {
+            k.decode()[:-1]
+            for k in self.chunkmap
+            if not k.startswith((b"ImageDataSeq", b"CustomData", ND2_FILE_SIGNATURE))
+        }
+
+        if include:
+            _keys: set[str] = set()
+            for i in include:
+                if i not in keys:
+                    warnings.warn(f"Key {i!r} not found in metadata", stacklevel=2)
+                else:
+                    _keys.add(i)
+            keys = _keys
+        if exclude:
+            keys = {k for k in keys if k not in exclude}
+
+        output: dict[str, Any] = {}
+        for key in sorted(keys):
+            name = f"{key}!".encode()
+            try:
+                output[key] = self._decode_chunk(name, strip_prefix=strip_prefix)
+            except Exception:  # pragma: no cover
+                output[key] = self._load_chunk(name)
+        return output
```

### Comparing `nd2-0.7.0/src/nd2/_pysdk/_sdk_types.py` & `nd2-0.7.1/src/nd2/_sdk_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -335,14 +335,24 @@
             3,  # Plugin
             4,  # Macro
         ]
         Size: int
         Desc: str
         Unit: str
 
+    class BinaryMetaDict(TypedDict):
+        BinLayerID: int
+        State: int
+        Color: int
+        CompOrder: int
+        Name: str
+        FileTag: str
+        CompName: str
+        ColorMode: int
+
     # These dicts are intermediate dicts created in the process of parsing raw meta
     # they mimic intermediate parsing done by the SDK... but needn't stay this way.
 
     AxisInterpretation = Literal["distance", "time"]
     CompressionType = Literal["lossless", "lossy", "none"]
     LoopTypeString = Literal[
         "Unknown",
```

### Comparing `nd2-0.7.0/tests/conftest.py` & `nd2-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/readlim_output.json` & `nd2-0.7.1/tests/readlim_output.json`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/samples_metadata.json` & `nd2-0.7.1/tests/samples_metadata.json`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_aicsimage.py` & `nd2-0.7.1/tests/test_aicsimage.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_binary.py` & `nd2-0.7.1/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_codspeed.py` & `nd2-0.7.1/tests/test_codspeed.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_dask_dispatch.py` & `nd2-0.7.1/tests/test_dask_dispatch.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_index.py` & `nd2-0.7.1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_metadata.py` & `nd2-0.7.1/tests/test_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import dask.array as da
 import pytest
 import xarray as xr
 from nd2 import ND2File, _util, structures
-from nd2._pysdk._chunk_decode import ND2_FILE_SIGNATURE
+from nd2._parse._chunk_decode import ND2_FILE_SIGNATURE
 
 sys.path.append(str(Path(__file__).parent.parent / "scripts"))
 from nd2_describe import get_nd2_stats  # noqa: E402
 
 if TYPE_CHECKING:
     from typing_extensions import Literal
 
@@ -21,17 +21,19 @@
 with open("tests/samples_metadata.json") as f:
     EXPECTED = json.load(f)
 
 DATA = Path(__file__).parent / "data"
 
 
 @pytest.mark.parametrize("path", EXPECTED, ids=lambda x: f'{x}_{EXPECTED[x]["ver"]}')
-def test_metadata_integrity(path: str):
+def test_metadata_integrity(path: str) -> None:
     """Test that the current API matches the expected output for sample data."""
     target = Path("tests/data") / path
+    if _util.is_legacy(target):
+        pytest.skip()
     name, stats = get_nd2_stats(target)
 
     # normalize serizalized stuff
     stats = json.loads(json.dumps(stats, default=str))
 
     for key in stats:
         # The SDK has a bug in position name fetching... we do it better, so just clear
@@ -44,22 +46,22 @@
     for exp in exps:
         for item in exp:
             if item["type"] == "XYPosLoop":
                 for point in item["parameters"]["points"]:
                     point.pop("name", None)
 
 
-def test_decode_all_chunks(new_nd2):
+def test_decode_all_chunks(new_nd2: Path) -> None:
     with ND2File(new_nd2) as f:
         for key in f._rdr.chunkmap:
             if not key.startswith((b"ImageDataSeq", b"CustomData", ND2_FILE_SIGNATURE)):
                 f._rdr._decode_chunk(key)
 
 
-def test_metadata_extraction(new_nd2: Path):
+def test_metadata_extraction(new_nd2: Path) -> None:
     assert ND2File.is_supported_file(new_nd2)
     with ND2File(new_nd2) as nd:
         assert repr(nd)
         assert nd.path == str(new_nd2)
         assert not nd.closed
 
         assert isinstance(nd._rdr._seq_count(), int)
@@ -99,14 +101,15 @@
 
         assert isinstance(nd.attributes, structures.Attributes)
 
         # # TODO: deal with typing when metadata is completely missing
         # assert isinstance(nd.metadata, structures.Metadata)
         assert isinstance(nd.experiment, list)
         assert isinstance(nd.text_info, dict)
+        assert isinstance(nd.metadata, structures.Metadata)
         xarr = nd.to_xarray()
         assert isinstance(xarr, xr.DataArray)
         assert isinstance(xarr.data, da.Array)
 
         with pytest.warns(UserWarning, match="not implemented"):
             nd.events()
 
@@ -171,7 +174,14 @@
 
     assert isinstance(events, list if orient == "records" else dict)
     if events and isinstance(events, dict):
         assert _util.TIME_KEY in events
 
     pd = pytest.importorskip("pandas")
     print(pd.DataFrame(events))
+
+
+def test_compressed_metadata() -> None:
+    with ND2File(DATA / "rois.nd2") as f:
+        chunk = f._rdr._decode_chunk(b"CustomData|CustomDescriptionV1_0!")
+        assert "CLxCustomDescription" in chunk
+        assert "Name" in chunk["CLxCustomDescription"]
```

### Comparing `nd2-0.7.0/tests/test_parse.py` & `nd2-0.7.1/tests/test_parse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
 from functools import lru_cache
 from pathlib import Path
 from typing import Any
 
 import pytest
 from nd2 import structures
-from nd2._pysdk import _parse
-from nd2._pysdk._pysdk import ND2Reader
+from nd2._parse import _parse
+from nd2.readers import ModernReader
 
 
 @lru_cache(maxsize=None)
 def readlim_output():
     TESTS = Path(__file__).parent
     return json.loads((TESTS / "readlim_output.json").read_text())
 
 
 def test_parse_raw_metadata(new_nd2: Path):
     expected = readlim_output()
     if new_nd2.name not in expected:
         pytest.skip(f"{new_nd2.name} not in readlim_output.json")
-    with ND2Reader(new_nd2) as rdr:
+    with ModernReader(new_nd2) as rdr:
         rdr._cached_global_metadata()  # force metadata to be read
         meta = {
             "Attributes": rdr._raw_attributes,
             "Experiment": rdr._raw_experiment,
             "Metadata": rdr._raw_image_metadata,
             "TextInfo": rdr._raw_text_info,
         }
```

### Comparing `nd2-0.7.0/tests/test_reader.py` & `nd2-0.7.1/tests/test_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from pathlib import Path
 
 import dask.array as da
 import numpy as np
 import pytest
 import xarray as xr
 from nd2 import ND2File, imread
-from nd2._util import AXIS
+from nd2._parse._chunk_decode import get_version
+from nd2._util import AXIS, is_supported_file
 from resource_backed_dask_array import ResourceBackedDaskArray
 
 DATA = Path(__file__).parent / "data"
 
 
 def test_read_safety(new_nd2: Path):
     with ND2File(new_nd2) as nd:
         for i in range(nd._frame_count):
-            nd._rdr._read_image(i)
+            nd._rdr.read_frame(i)
 
 
 def test_position(new_nd2: Path):
     """use position to extract a single stage position with asarray."""
     if new_nd2.stat().st_size > 250_000_000:
         pytest.skip("skipping read on big files")
     with ND2File(new_nd2) as nd:
@@ -261,7 +262,22 @@
     import gc
 
     f: ND2File | None = ND2File(single_nd2)
 
     with pytest.warns(UserWarning, match="ND2File file not closed"):
         f = None  # noqa: F841
         gc.collect()
+
+
+def test_file_handles(single_nd2: Path) -> None:
+    """Test that we can open a file with a file handle also"""
+    # just for coverage, since usually it will use the filehandle
+    assert get_version(single_nd2) == (3, 0)
+
+    with open(single_nd2, "rb") as fh:
+        assert is_supported_file(fh)
+        f = ND2File(fh)
+        assert f.path == str(single_nd2)
+        assert f.version == (3, 0)
+        assert isinstance(f.asarray(), np.ndarray)
+    assert fh.closed
+    assert f.closed
```

### Comparing `nd2-0.7.0/tests/test_readme.py` & `nd2-0.7.1/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/test_rescue.py` & `nd2-0.7.1/tests/test_rescue.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import nd2
 import numpy as np
 import pytest
-from nd2._pysdk._chunk_decode import get_chunkmap
+from nd2._parse._chunk_decode import get_chunkmap
 
 
 @pytest.fixture()
 def broken_nd2(tmp_path, single_nd2):
     with open(single_nd2, "rb") as f:
         data = f.read()
```

### Comparing `nd2-0.7.0/tests/test_xml.py` & `nd2-0.7.1/tests/test_xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 from typing import cast
 
-from nd2._clx_xml import json_from_clx_variant
+from nd2._parse._clx_xml import json_from_clx_variant
 
 XML = (Path(__file__).parent / "variant.xml").read_bytes()
 
 
 def test_parse_xml() -> None:
     result = cast(dict, json_from_clx_variant(XML))
     assert list(result) == [
```

### Comparing `nd2-0.7.0/tests/variant.xml` & `nd2-0.7.1/tests/variant.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/tests/variant_CustomDataV2_0.xml` & `nd2-0.7.1/tests/variant_CustomDataV2_0.xml`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/.gitignore` & `nd2-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/LICENSE` & `nd2-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nd2-0.7.0/pyproject.toml` & `nd2-0.7.1/pyproject.toml`

 * *Files identical despite different names*

