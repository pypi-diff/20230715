# Comparing `tmp/zimran-config-1.0.6.tar.gz` & `tmp/zimran-config-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-config-1.0.6.tar", last modified: Wed Feb 22 09:17:46 2023, max compression
+gzip compressed data, was "zimran-config-1.1.0.tar", last modified: Sat Jul 15 13:53:24 2023, max compression
```

## Comparing `zimran-config-1.0.6.tar` & `zimran-config-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:46.214745 zimran-config-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-22 09:17:46.210745 zimran-config-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-22 09:17:37.000000 zimran-config-1.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:17:46.214745 zimran-config-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-22 09:17:37.000000 zimran-config-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:46.210745 zimran-config-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-22 09:17:37.000000 zimran-config-1.0.6/tests/test_common_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:46.210745 zimran-config-1.0.6/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:46.210745 zimran-config-1.0.6/zimran/config/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-22 09:17:37.000000 zimran-config-1.0.6/zimran/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:46.210745 zimran-config-1.0.6/zimran_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-22 09:17:46.000000 zimran-config-1.0.6/zimran_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-22 09:17:46.000000 zimran-config-1.0.6/zimran_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:17:46.000000 zimran-config-1.0.6/zimran_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-22 09:17:46.000000 zimran-config-1.0.6/zimran_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-22 09:17:46.000000 zimran-config-1.0.6/zimran_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:53:24.649504 zimran-config-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-15 13:53:24.649504 zimran-config-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-15 13:53:14.000000 zimran-config-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 13:53:24.649504 zimran-config-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-15 13:53:14.000000 zimran-config-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:53:24.645504 zimran-config-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-15 13:53:14.000000 zimran-config-1.1.0/tests/test_common_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:53:24.645504 zimran-config-1.1.0/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:53:24.645504 zimran-config-1.1.0/zimran/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-15 13:53:14.000000 zimran-config-1.1.0/zimran/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 13:53:24.649504 zimran-config-1.1.0/zimran_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-15 13:53:24.000000 zimran-config-1.1.0/zimran_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-15 13:53:24.000000 zimran-config-1.1.0/zimran_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 13:53:24.000000 zimran-config-1.1.0/zimran_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 13:53:24.000000 zimran-config-1.1.0/zimran_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 13:53:24.000000 zimran-config-1.1.0/zimran_config.egg-info/top_level.txt
```

### Comparing `zimran-config-1.0.6/setup.py` & `zimran-config-1.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 setup(
     name='zimran-config',
     version=environ['GITHUB_REF_NAME'],
     description='Pydantic based configuration for FastAPI services',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['zimran.*']),
-    install_requires=['pydantic'],
+    install_requires=['pydantic-settings==2.0.*'],
     python_requires='>=3.10',
     zip_file=False,
 )
```

### Comparing `zimran-config-1.0.6/tests/test_common_settings.py` & `zimran-config-1.1.0/tests/test_common_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 SENTRY_DSN = 'https://public@sentry.example.com/1'
 
 
 def test_sentry_dsn(mocker: MockerFixture) -> None:
     mocker.patch.dict(environ, {'SENTRY_DSN': SENTRY_DSN})
     settings = CommonSettings()
-    assert settings.sentry_dsn == SENTRY_DSN
+    assert str(settings.sentry_dsn) == SENTRY_DSN
 
 
 @pytest.mark.parametrize('environment', [
     Environment.DEVELOPMENT, Environment.STAGING, Environment.PRODUCTION,
 ])
 def test_environment_ok(mocker: MockerFixture, environment: Environment) -> None:
     mocker.patch.dict(environ, {'SENTRY_DSN': SENTRY_DSN, 'ENVIRONMENT': environment})
```

