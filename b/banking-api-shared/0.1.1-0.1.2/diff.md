# Comparing `tmp/banking_api_shared-0.1.1.tar.gz` & `tmp/banking_api_shared-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banking_api_shared-0.1.1.tar", last modified: Sun Jul  9 20:00:27 2023, max compression
+gzip compressed data, was "banking_api_shared-0.1.2.tar", last modified: Sat Jul 15 16:42:39 2023, max compression
```

## Comparing `banking_api_shared-0.1.1.tar` & `banking_api_shared-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 20:00:27.935519 banking_api_shared-0.1.1/
--rw-rw-rw-   0        0        0      325 2023-07-09 20:00:27.933462 banking_api_shared-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-09 20:00:27.904757 banking_api_shared-0.1.1/banking_api_shared/
--rw-rw-rw-   0        0        0        0 2022-11-24 07:07:48.000000 banking_api_shared-0.1.1/banking_api_shared/__init__.py
--rw-rw-rw-   0        0        0      455 2023-07-09 19:51:27.000000 banking_api_shared-0.1.1/banking_api_shared/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-09 20:00:27.925295 banking_api_shared-0.1.1/banking_api_shared.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-09 20:00:27.000000 banking_api_shared-0.1.1/banking_api_shared.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      239 2023-07-09 20:00:27.000000 banking_api_shared-0.1.1/banking_api_shared.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 20:00:27.000000 banking_api_shared-0.1.1/banking_api_shared.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-07-09 20:00:27.000000 banking_api_shared-0.1.1/banking_api_shared.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-09 20:00:27.935519 banking_api_shared-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-07-09 19:51:27.000000 banking_api_shared-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:42:39.884466 banking_api_shared-0.1.2/
+-rw-rw-rw-   0        0        0      325 2023-07-15 16:42:39.884466 banking_api_shared-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 16:42:39.862064 banking_api_shared-0.1.2/banking_api_shared/
+-rw-rw-rw-   0        0        0        0 2022-11-24 07:07:48.000000 banking_api_shared-0.1.2/banking_api_shared/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-07-15 16:19:14.000000 banking_api_shared-0.1.2/banking_api_shared/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:42:39.884466 banking_api_shared-0.1.2/banking_api_shared.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-07-15 16:42:39.000000 banking_api_shared-0.1.2/banking_api_shared.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2023-07-15 16:42:39.000000 banking_api_shared-0.1.2/banking_api_shared.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:42:39.000000 banking_api_shared-0.1.2/banking_api_shared.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-15 16:42:39.000000 banking_api_shared-0.1.2/banking_api_shared.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:42:39.884466 banking_api_shared-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-07-15 16:29:39.000000 banking_api_shared-0.1.2/setup.py
```

### Comparing `banking_api_shared-0.1.1/setup.py` & `banking_api_shared-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,13 +8,13 @@
             'maintainer_email': 'edazizovv@gmail.com',
             'description': 'Shared extensions for banking_api project',
             'license': 'Proprietary',
             'url': 'https://github.com/edazizovv/oaiv',
             'download_url': 'https://github.com/edazizovv/oaiv',
             'packages': setuptools.find_packages(),
             'include_package_data': True,
-            'version': '0.1.1',
+            'version': '0.1.2',
             'long_description': '',
             'python_requires': '>=3.10',
             'install_requires': []}
 
 setup(**metadata)
```

