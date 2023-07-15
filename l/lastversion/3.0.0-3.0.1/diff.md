# Comparing `tmp/lastversion-3.0.0.tar.gz` & `tmp/lastversion-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lastversion-3.0.0.tar", last modified: Thu Jun 22 11:22:46 2023, max compression
+gzip compressed data, was "lastversion-3.0.1.tar", last modified: Sat Jul 15 14:26:20 2023, max compression
```

## Comparing `lastversion-3.0.0.tar` & `lastversion-3.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 11:22:46.956711 lastversion-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-06-22 11:22:31.000000 lastversion-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-22 11:22:31.000000 lastversion-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    26270 2023-06-22 11:22:46.956711 lastversion-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    19820 2023-06-22 11:22:31.000000 lastversion-3.0.0/README-ZH-CN.md
--rw-r--r--   0 runner    (1001) docker     (122)    25613 2023-06-22 11:22:31.000000 lastversion-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 11:22:46.952711 lastversion-3.0.0/lastversion/
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/BitBucketRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/FeedRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    27697 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/GitHubRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/GitLabRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    13751 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/GiteaRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/HelmChartRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/HolderFactory.py
--rw-r--r--   0 runner    (1001) docker     (122)      945 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/LocalVersionSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/MercurialRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)    13868 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/ProjectHolder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/PypiRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/SourceForgeRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/SystemRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     7804 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/Version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/WikipediaRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/WordPressPluginRepoSession.py
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/__about__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/argparse_version.py
--rw-r--r--   0 runner    (1001) docker     (122)    29274 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/lastversion.py
--rw-r--r--   0 runner    (1001) docker     (122)      681 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/spdx_id_to_rpmspec.py
--rw-r--r--   0 runner    (1001) docker     (122)    10860 2023-06-22 11:22:31.000000 lastversion-3.0.0/lastversion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 11:22:46.956711 lastversion-3.0.0/lastversion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    26270 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      920 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 11:22:46.000000 lastversion-3.0.0/lastversion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-22 11:22:46.956711 lastversion-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2676 2023-06-22 11:22:31.000000 lastversion-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 14:26:20.097404 lastversion-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-07-15 14:26:09.000000 lastversion-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-07-15 14:26:09.000000 lastversion-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    26270 2023-07-15 14:26:20.097404 lastversion-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    19820 2023-07-15 14:26:09.000000 lastversion-3.0.1/README-ZH-CN.md
+-rw-r--r--   0 runner    (1001) docker     (122)    25613 2023-07-15 14:26:09.000000 lastversion-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 14:26:20.097404 lastversion-3.0.1/lastversion/
+-rw-r--r--   0 runner    (1001) docker     (122)     1226 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/BitBucketRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3122 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/FeedRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27697 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/GitHubRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5033 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/GitLabRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13664 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/GiteaRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/HelmChartRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4080 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/HolderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (122)      945 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/LocalVersionSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1981 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/MercurialRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13868 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/ProjectHolder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3100 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/PypiRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1560 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/SourceForgeRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3979 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/SystemRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7900 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/Version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3619 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/WikipediaRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3099 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/WordPressPluginRepoSession.py
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1123 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/argparse_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29274 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/lastversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      681 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/spdx_id_to_rpmspec.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10860 2023-07-15 14:26:09.000000 lastversion-3.0.1/lastversion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-15 14:26:20.097404 lastversion-3.0.1/lastversion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    26270 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      923 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-15 14:26:20.000000 lastversion-3.0.1/lastversion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-15 14:26:20.101404 lastversion-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2833 2023-07-15 14:26:09.000000 lastversion-3.0.1/setup.py
```

### Comparing `lastversion-3.0.0/LICENSE` & `lastversion-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/PKG-INFO` & `lastversion-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastversion
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI tool to find the latest stable version of an arbitrary project
 Home-page: https://github.com/dvershinin/lastversion
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `lastversion-3.0.0/README-ZH-CN.md` & `lastversion-3.0.1/README-ZH-CN.md`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/README.md` & `lastversion-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/BitBucketRepoSession.py` & `lastversion-3.0.1/lastversion/BitBucketRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/FeedRepoSession.py` & `lastversion-3.0.1/lastversion/FeedRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/GitHubRepoSession.py` & `lastversion-3.0.1/lastversion/GitHubRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/GitLabRepoSession.py` & `lastversion-3.0.1/lastversion/GitLabRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/GiteaRepoSession.py` & `lastversion-3.0.1/lastversion/GiteaRepoSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,15 @@
         return full_name
 
     def __init__(self, repo, hostname):
         super(GiteaRepoSession, self).__init__()
         # dict holding repo/owner to feed contents of releases atom
         self.feed_contents = {}
         self.rate_limited_count = 0
-        self.api_token = os.getenv("GITHUB_API_TOKEN")
-        if not self.api_token:
-            self.api_token = os.getenv("GITHUB_TOKEN")
+        self.api_token = os.getenv("GITEA_API_TOKEN")
         self.hostname = hostname
         if not self.hostname:
             self.hostname = self.DEFAULT_HOSTNAME
         # Explicitly specify the API version that we want:
         self.headers.update({
             'Accept': 'application/vnd.github.v3+json'
         })
```

### Comparing `lastversion-3.0.0/lastversion/HelmChartRepoSession.py` & `lastversion-3.0.1/lastversion/HelmChartRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/HolderFactory.py` & `lastversion-3.0.1/lastversion/HolderFactory.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/LocalVersionSession.py` & `lastversion-3.0.1/lastversion/LocalVersionSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/MercurialRepoSession.py` & `lastversion-3.0.1/lastversion/MercurialRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/ProjectHolder.py` & `lastversion-3.0.1/lastversion/ProjectHolder.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/PypiRepoSession.py` & `lastversion-3.0.1/lastversion/PypiRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/SourceForgeRepoSession.py` & `lastversion-3.0.1/lastversion/SourceForgeRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/SystemRepoSession.py` & `lastversion-3.0.1/lastversion/SystemRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/Version.py` & `lastversion-3.0.1/lastversion/Version.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         # go through parts separated by dot, detect beta level, and weed out numberless info:
         parts_n = []
         for part in parts:
             # help devel releases to be correctly identified
             # https://www.python.org/dev/peps/pep-0440/#developmental-releases
             if part in ['devel', 'test', 'dev']:
                 part = 'dev0'
+            elif part in ['alpha']:
+                # "4.3.0-alpha"
+                part = 'a0'
             elif part in ['beta']:
                 # "4.3.0-beta"
                 part = 'b0'
             else:
                 # help post (patch) releases to be correctly identified (e.g. Magento 2.3.4-p2)
                 # p12 => post12
                 part = re.sub('^p(\\d+)$', 'post\\1', part, 1)
```

### Comparing `lastversion-3.0.0/lastversion/WikipediaRepoSession.py` & `lastversion-3.0.1/lastversion/WikipediaRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/WordPressPluginRepoSession.py` & `lastversion-3.0.1/lastversion/WordPressPluginRepoSession.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/__init__.py` & `lastversion-3.0.1/lastversion/__init__.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/argparse_version.py` & `lastversion-3.0.1/lastversion/argparse_version.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/lastversion.py` & `lastversion-3.0.1/lastversion/lastversion.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/spdx_id_to_rpmspec.py` & `lastversion-3.0.1/lastversion/spdx_id_to_rpmspec.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion/utils.py` & `lastversion-3.0.1/lastversion/utils.py`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion.egg-info/PKG-INFO` & `lastversion-3.0.1/lastversion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lastversion
-Version: 3.0.0
+Version: 3.0.1
 Summary: A CLI tool to find the latest stable version of an arbitrary project
 Home-page: https://github.com/dvershinin/lastversion
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `lastversion-3.0.0/lastversion.egg-info/SOURCES.txt` & `lastversion-3.0.1/lastversion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lastversion-3.0.0/lastversion.egg-info/requires.txt` & `lastversion-3.0.1/lastversion.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 requests>=2.6.1
 packaging
-cachecontrol==0.12.6
+cachecontrol<=0.12.11
 lockfile
 appdirs
 python-dateutil
 PyYAML
 tqdm
 six
 beautifulsoup4
@@ -16,15 +16,15 @@
 
 [:python_version >= "3.0.0"]
 feedparser
 
 [build]
 requests>=2.6.1
 packaging
-cachecontrol==0.12.6
+cachecontrol<=0.12.11
 lockfile
 appdirs
 python-dateutil
 PyYAML
 tqdm
 six
 beautifulsoup4
@@ -50,15 +50,15 @@
 mkdocs-material
 mkdocstrings
 markdown-include
 
 [tests]
 requests>=2.6.1
 packaging
-cachecontrol==0.12.6
+cachecontrol<=0.12.11
 lockfile
 appdirs
 python-dateutil
 PyYAML
 tqdm
 six
 beautifulsoup4
```

### Comparing `lastversion-3.0.0/setup.py` & `lastversion-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 
 
 install_requires = [
     # require at least requests==2.6.1 due to cachecontrol's bug:
     # https://github.com/ionrock/cachecontrol/issues/137
     'requests>=2.6.1',
     'packaging',
-    # latest 0.12.12 uses filelock instead of lockfile,
-    # we have to update our packaging before switching to it
-    'cachecontrol==0.12.6',
+    # Cachecontrol 0.12.12 uses filelock instead of lockfile, and reverts to lockfile in 0.12.14.
+    # Newer versions use filelock, but most distros package cachecontrol 0.12.11.
+    # Ideally we can specify 0.12.14, but pip doesn't allow this, so just pin to what we can
+    'cachecontrol<=0.12.11',
     'lockfile',
     'appdirs',
     # feedparser 6 dropped Python 2 support
     'feedparser <= 5.2.1; python_version < "3.0.0"',
     'feedparser; python_version >= "3.0.0"',
     'python-dateutil',
     'PyYAML',
```

