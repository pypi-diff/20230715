# Comparing `tmp/oras-0.1.2.tar.gz` & `tmp/oras-0.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.2.tar", last modified: Sat Jul 15 18:42:09 2023, max compression
+gzip compressed data, was "oras-0.1.20.tar", last modified: Sat Jul 15 19:34:24 2023, max compression
```

## Comparing `oras-0.1.2.tar` & `oras-0.1.20.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.734842 oras-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-15 18:41:35.000000 oras-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-15 18:41:35.000000 oras-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-07-15 18:42:09.734842 oras-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5239 2023-07-15 18:41:35.000000 oras-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/
--rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-15 18:41:35.000000 oras-0.1.2/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-15 18:41:35.000000 oras-0.1.2/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-15 18:41:35.000000 oras-0.1.2/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-15 18:41:35.000000 oras-0.1.2/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-15 18:41:35.000000 oras-0.1.2/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-15 18:41:35.000000 oras-0.1.2/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-15 18:41:35.000000 oras-0.1.2/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/main/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 18:41:35.000000 oras-0.1.2/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-15 18:41:35.000000 oras-0.1.2/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-15 18:41:35.000000 oras-0.1.2/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (122)    35813 2023-07-15 18:41:35.000000 oras-0.1.2/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-15 18:41:35.000000 oras-0.1.2/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/artifact.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 18:41:35.000000 oras-0.1.2/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.734842 oras-0.1.2/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-15 18:41:35.000000 oras-0.1.2/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (122)      984 2023-07-15 18:41:35.000000 oras-0.1.2/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 18:42:09.730842 oras-0.1.2/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6082 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 18:42:05.000000 oras-0.1.2/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-15 18:42:09.000000 oras-0.1.2/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-15 18:41:35.000000 oras-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-15 18:42:09.734842 oras-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-15 18:41:35.000000 oras-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.291754 oras-0.1.20/
+-rw-r--r--   0 runner    (1001) docker     (122)    11343 2023-07-15 19:33:55.000000 oras-0.1.20/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-07-15 19:33:55.000000 oras-0.1.20/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-15 19:34:24.291754 oras-0.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5596 2023-07-15 19:33:55.000000 oras-0.1.20/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.287754 oras-0.1.20/oras/
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-07-15 19:33:55.000000 oras-0.1.20/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-07-15 19:33:55.000000 oras-0.1.20/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7530 2023-07-15 19:33:55.000000 oras-0.1.20/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3812 2023-07-15 19:33:55.000000 oras-0.1.20/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2200 2023-07-15 19:33:55.000000 oras-0.1.20/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1787 2023-07-15 19:33:55.000000 oras-0.1.20/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8737 2023-07-15 19:33:55.000000 oras-0.1.20/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.287754 oras-0.1.20/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 19:33:55.000000 oras-0.1.20/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-07-15 19:33:55.000000 oras-0.1.20/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4470 2023-07-15 19:33:55.000000 oras-0.1.20/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35813 2023-07-15 19:33:55.000000 oras-0.1.20/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-07-15 19:33:55.000000 oras-0.1.20/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.287754 oras-0.1.20/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/artifact.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      185 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     5066 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4235 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3930 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.291754 oras-0.1.20/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-15 19:33:55.000000 oras-0.1.20/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.291754 oras-0.1.20/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-15 19:33:55.000000 oras-0.1.20/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10673 2023-07-15 19:33:55.000000 oras-0.1.20/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1609 2023-07-15 19:33:55.000000 oras-0.1.20/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      985 2023-07-15 19:33:55.000000 oras-0.1.20/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 19:34:24.287754 oras-0.1.20/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6440 2023-07-15 19:34:24.000000 oras-0.1.20/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-15 19:34:24.000000 oras-0.1.20/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 19:34:24.000000 oras-0.1.20/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 19:34:20.000000 oras-0.1.20/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-07-15 19:34:24.000000 oras-0.1.20/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-15 19:34:24.000000 oras-0.1.20/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-15 19:33:55.000000 oras-0.1.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-15 19:34:24.291754 oras-0.1.20/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3370 2023-07-15 19:33:55.000000 oras-0.1.20/setup.py
```

### Comparing `oras-0.1.2/LICENSE` & `oras-0.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/PKG-INFO` & `oras-0.1.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.2
+Version: 0.1.20
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -62,14 +62,15 @@
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.2 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.20 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -23,13 +23,13 @@
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
 [Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
  Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
      ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
                 Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
                   ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
-     ð»     ð� Ananya      ð»
-                          Gupta
-                           ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
+     ð»     ð� Ananya      ð»   Marius
+                          Gupta                  Bertram
+                           ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.2/README.md` & `oras-0.1.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -37,14 +37,15 @@
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -12,13 +12,13 @@
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
 [Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
  Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
      ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
                 Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
                   ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
-     ð»     ð� Ananya      ð»
-                          Gupta
-                           ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
+     ð»     ð� Ananya      ð»   Marius
+                          Gupta                  Bertram
+                           ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.2/oras/auth.py` & `oras-0.1.20/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/client.py` & `oras-0.1.20/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/container.py` & `oras-0.1.20/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/decorator.py` & `oras-0.1.20/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/defaults.py` & `oras-0.1.20/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/logger.py` & `oras-0.1.20/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/main/login.py` & `oras-0.1.20/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/oci.py` & `oras-0.1.20/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/provider.py` & `oras-0.1.20/oras/provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/schemas.py` & `oras-0.1.20/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/tests/test_oras.py` & `oras-0.1.20/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/tests/test_provider.py` & `oras-0.1.20/oras/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/tests/test_utils.py` & `oras-0.1.20/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/utils/fileio.py` & `oras-0.1.20/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/utils/request.py` & `oras-0.1.20/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/oras/version.py` & `oras-0.1.20/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.2"
+__version__ = "0.1.20"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.2/oras.egg-info/PKG-INFO` & `oras-0.1.20/oras.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.2
+Version: 0.1.20
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-11-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-12-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -62,14 +62,15 @@
       <td align="center" valign="top" width="14.28%"><a href="wolfv.github.io"><img src="https://avatars.githubusercontent.com/u/885054?v=4?s=100" width="100px;" alt="Wolf Vollprecht"/><br /><sub><b>Wolf Vollprecht</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=wolfv" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/shizhMSFT"><img src="https://avatars.githubusercontent.com/u/32161882?v=4?s=100" width="100px;" alt="Shiwei Zhang"/><br /><sub><b>Shiwei Zhang</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=shizhMSFT" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jhlmco"><img src="https://avatars.githubusercontent.com/u/126677738?v=4?s=100" width="100px;" alt="jhlmco"/><br /><sub><b>jhlmco</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=jhlmco" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Ananya2003Gupta"><img src="https://avatars.githubusercontent.com/u/90386813?v=4?s=100" width="100px;" alt="Ananya Gupta"/><br /><sub><b>Ananya Gupta</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=Ananya2003Gupta" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/sunnycarter"><img src="https://avatars.githubusercontent.com/u/36891339?v=4?s=100" width="100px;" alt="sunnycarter"/><br /><sub><b>sunnycarter</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=sunnycarter" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mariusbertram"><img src="https://avatars.githubusercontent.com/u/10505884?v=4?s=100" width="100px;" alt="Marius Bertram"/><br /><sub><b>Marius Bertram</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=mariusbertram" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.2 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.20 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python  [![All Contributors](https://img.shields.io/badge/
-all_contributors-11-orange.svg?style=flat-square)](#contributors-)  ![ORAS
+all_contributors-12-orange.svg?style=flat-square)](#contributors-)  ![ORAS
 Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
@@ -23,13 +23,13 @@
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
 [Vanessasaurus] [Lachlan  [Steve      [Josh     [Bridget   [Matt      [Wolf
  Vanessasaurus  Evenson] Lasker]    Dolitsky]   Kromhout] Warner]  Vollprecht]
      ð»   Lachlan   Steve   Josh_Dolitsky  Bridget    Matt      Wolf
                 Evenson   Lasker      ð»  Kromhout   Warner  Vollprecht
                   ð�  ð»               ð»  ð�   ð»
-[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]
- Shiwei_Zhang    jhlmco   Gupta]   sunnycarter
-     ð»     ð� Ananya      ð»
-                          Gupta
-                           ð»
+[Shiwei_Zhang]  [jhlmco] [Ananya  [sunnycarter]  [Marius
+ Shiwei_Zhang    jhlmco   Gupta]   sunnycarter  Bertram]
+     ð»     ð� Ananya      ð»   Marius
+                          Gupta                  Bertram
+                           ð»               ð»
    ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.2/oras.egg-info/SOURCES.txt` & `oras-0.1.20/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.2/setup.py` & `oras-0.1.20/setup.py`

 * *Files identical despite different names*

