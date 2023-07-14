# Comparing `tmp/preset-cli-0.2.2.tar.gz` & `tmp/preset-cli-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.2.tar", last modified: Wed Jul  5 22:23:30 2023, max compression
+gzip compressed data, was "preset-cli-0.2.3.tar", last modified: Fri Jul 14 22:32:32 2023, max compression
```

## Comparing `preset-cli-0.2.2.tar` & `preset-cli-0.2.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.719186 preset-cli-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.695186 preset-cli-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 22:23:19.000000 preset-cli-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-05 22:23:19.000000 preset-cli-0.2.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-07-05 22:23:19.000000 preset-cli-0.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-05 22:23:19.000000 preset-cli-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-05 22:23:19.000000 preset-cli-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-05 22:23:19.000000 preset-cli-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-05 22:23:30.719186 preset-cli-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-05 22:23:19.000000 preset-cli-0.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-05 22:23:19.000000 preset-cli-0.2.2/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 22:23:19.000000 preset-cli-0.2.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-05 22:23:19.000000 preset-cli-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.699186 preset-cli-0.2.2/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 22:23:19.000000 preset-cli-0.2.2/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-05 22:23:19.000000 preset-cli-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-05 22:23:19.000000 preset-cli-0.2.2/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-05 22:23:19.000000 preset-cli-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-05 22:23:30.719186 preset-cli-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-05 22:23:19.000000 preset-cli-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.691186 preset-cli-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20169 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.707186 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 22:23:19.000000 preset-cli-0.2.2/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.703186 preset-cli-0.2.2/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-05 22:23:30.000000 preset-cli-0.2.2/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47038 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/password_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/auth/preset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.711186 preset-cli-0.2.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:30.715186 preset-cli-0.2.2/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-05 22:23:19.000000 preset-cli-0.2.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.536189 preset-cli-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 22:32:20.000000 preset-cli-0.2.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-14 22:32:20.000000 preset-cli-0.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-14 22:32:20.000000 preset-cli-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 22:32:20.000000 preset-cli-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 22:32:20.000000 preset-cli-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-14 22:32:32.552189 preset-cli-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-14 22:32:20.000000 preset-cli-0.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 22:32:20.000000 preset-cli-0.2.3/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 22:32:20.000000 preset-cli-0.2.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 22:32:20.000000 preset-cli-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:32:20.000000 preset-cli-0.2.3/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 22:32:20.000000 preset-cli-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-14 22:32:32.552189 preset-cli-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-14 22:32:20.000000 preset-cli-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53266 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tox.ini
```

### Comparing `preset-cli-0.2.2/.coveragerc` & `preset-cli-0.2.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.3/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/.github/workflows/python-package.yml` & `preset-cli-0.2.3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/.github/workflows/python-publish.yml` & `preset-cli-0.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/.gitignore` & `preset-cli-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/.pre-commit-config.yaml` & `preset-cli-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/CHANGELOG.rst` & `preset-cli-0.2.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
 Changelog
 =========
 
+Next
+====
+
+Version 0.2.3 - 2023-07-14
+==========================
+
+- Adjustments to dbt marshmallow schemas to avoid integration errors (`#225 <https://github.com/preset-io/backend-sdk/pull/225>_`).
+
 Version 0.2.2 - 2023-07-05
 ==========================
 
 - ``certification`` and additional ``extra`` information is now synced from dbt models (`#213 <https://github.com/preset-io/backend-sdk/pull/213>`_ and `#215 <https://github.com/preset-io/backend-sdk/pull/215>`_).
 - Improved the ``exposures`` sync (`#221 <https://github.com/preset-io/backend-sdk/pull/221>`_).
 - The ``--preserve-columns`` flag can now be used to preserve ``groupby`` and ``filterable`` values for existing columns during a dbt sync (`#221 <https://github.com/preset-io/backend-sdk/pull/221>`_).
 - The search for roles during the ``sync roles`` command now uses ``Equals`` comparison, instead of ``Starts with`` (`#222 <https://github.com/preset-io/backend-sdk/pull/222>`_).
```

### Comparing `preset-cli-0.2.2/CONTRIBUTING.rst` & `preset-cli-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/Makefile` & `preset-cli-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/PKG-INFO` & `preset-cli-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.2/README.rst` & `preset-cli-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/dev-requirements.txt` & `preset-cli-0.2.3/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/docs/Makefile` & `preset-cli-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/docs/conf.py` & `preset-cli-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/docs/images/export_dashboards.png` & `preset-cli-0.2.3/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/docs/index.rst` & `preset-cli-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.3/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.3/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/requirements.txt` & `preset-cli-0.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/setup.cfg` & `preset-cli-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/setup.py` & `preset-cli-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.3/src/preset_cli/api/clients/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,33 +357,33 @@
     """
     Schema for a repository.
     """
 
     id = fields.Integer()
     account_id = fields.Integer()
     remote_url = fields.String()
-    remote_backend = fields.String()
+    remote_backend = fields.String(allow_none=True)
     git_clone_strategy = PostelEnumField(GitCloneStrategy)
     deploy_key_id = fields.Integer()
-    github_installation_id = fields.Integer()
+    github_installation_id = fields.Integer(allow_none=True)
     state = fields.Integer()
     created_at = fields.DateTime()
     updated_at = fields.DateTime()
 
     # not present in the spec
-    full_name = fields.String()
+    full_name = fields.String(allow_none=True)
     repository_credentials_id = fields.Integer(allow_none=True)
     gitlab = fields.String(allow_none=True)
     name = fields.String()
-    pull_request_url_template = fields.String()
+    pull_request_url_template = fields.String(allow_none=True)
     git_provider_id = fields.Integer()
     git_provider = fields.String(allow_none=True)
     project_id = fields.Integer()
     deploy_key = fields.Nested(DeployKeySchema)
-    github_repo = fields.String()
+    github_repo = fields.String(allow_none=True)
 
 
 class ProjectSchema(PostelSchema):
     """
     Schema for a dbt project.
     """
 
@@ -397,18 +397,18 @@
     repository_id = fields.Integer()
     state = fields.Integer()
     created_at = fields.DateTime()
     updated_at = fields.DateTime()
 
     # not present in the spec
     group_permissions = fields.List(fields.Nested(GroupPermissionSchema))
-    docs_job = fields.String(allow_none=True)
+    docs_job = fields.Nested("JobSchema", allow_none=True)
     docs_job_id = fields.Integer(allow_none=True)
     freshness_job_id = fields.Integer(allow_none=True)
-    freshness_job = fields.String(allow_none=True)
+    freshness_job = fields.Nested("JobSchema", allow_none=True)
     skipped_setup = fields.Boolean()
 
 
 class TriggerSchema(PostelSchema):
     """
     Schema for a job trigger.
     """
@@ -463,22 +463,38 @@
     """
 
     type = PostelEnumField(TimeType, required=True)
     interval = fields.Integer(allow_none=True)
     hours = fields.List(fields.Integer(), allow_none=True)
 
 
+class StringOrSchema(fields.Field):
+    """
+    Dynamic schema constructor for fields that could have a string or another schema
+    """
+
+    def __init__(self, nested_schema, *args, **kwargs):
+        self.nested_schema = nested_schema
+        super().__init__(*args, **kwargs)
+
+    def _deserialize(self, value, attr, data, **kwargs):
+        if isinstance(value, str):
+            return value
+
+        return self.nested_schema().load(value)
+
+
 class ScheduleSchema(PostelSchema):
     """
     Schema for a job schedule.
     """
 
     cron = fields.String()
-    date = fields.Nested(DateSchema, required=True)
-    time = fields.Nested(TimeSchema, required=True)
+    date = StringOrSchema(DateSchema, required=True)
+    time = StringOrSchema(TimeSchema, required=True)
 
 
 class ExecutionSchema(PostelSchema):
     """
     Schema for a job execution.
     """
 
@@ -492,28 +508,29 @@
 
     id = fields.Integer(allow_none=True)
     account_id = fields.Integer()
     project_id = fields.Integer()
     environment_id = fields.Integer()
     name = fields.String()
     dbt_version = fields.String(allow_none=True)
+    raw_dbt_version = fields.String(allow_none=True)
     triggers = fields.Nested(TriggerSchema)
     execute_steps = fields.List(fields.String())
     settings = fields.Nested(SettingsSchema)
     state = fields.Integer()
     generate_docs = fields.Boolean()
     schedule = fields.Nested(ScheduleSchema)
 
     # not present in the spec
     lifecycle_webhooks_url = fields.String(allow_none=True)
     cron_humanized = fields.String()
     created_at = fields.DateTime()
-    next_run = fields.DateTime()
+    next_run = fields.DateTime(allow_none=True)
     lifecycle_webhooks = fields.Boolean()
-    next_run_humanized = fields.String()
+    next_run_humanized = fields.String(allow_none=True)
     deferring_job_definition_id = fields.Integer(allow_none=True)
     deactivated = fields.Boolean()
     is_deferrable = fields.Boolean()
     updated_at = fields.DateTime()
     execution = fields.Nested(ExecutionSchema)
     run_failure_count = fields.Integer()
     run_generate_sources = fields.Boolean()
```

### Comparing `preset-cli-0.2.2/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.3/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.3/src/preset_cli/api/clients/superset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.3/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/auth/lib.py` & `preset-cli-0.2.3/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/auth/main.py` & `preset-cli-0.2.3/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/auth/password.py` & `preset-cli-0.2.3/src/preset_cli/auth/password.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/auth/preset.py` & `preset-cli-0.2.3/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/main.py` & `preset-cli-0.2.3/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/export.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/dbt/metrics.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/exceptions.py` & `preset-cli-0.2.3/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli/lib.py` & `preset-cli-0.2.3/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.3/src/preset_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.2
+Version: 0.2.3
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.2/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.3/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.3/src/preset_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/api/clients/dbt_test.py` & `preset-cli-0.2.3/tests/api/clients/dbt_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -275,16 +275,74 @@
                         "git_provider_id": 33120,
                         "gitlab": None,
                         "git_provider": None,
                     },
                     "group_permissions": [],
                     "docs_job_id": None,
                     "freshness_job_id": None,
-                    "docs_job": None,
-                    "freshness_job": None,
+                    "docs_job": {
+                        "execution": {"timeout_seconds": 0},
+                        "generate_docs": True,
+                        "run_generate_sources": False,
+                        "id": 108380,
+                        "account_id": 72449,
+                        "project_id": 134905,
+                        "environment_id": 107605,
+                        "name": "Test job",
+                        "dbt_version": "1.0.0",
+                        "raw_dbt_version": None,
+                        "created_at": "2022-07-25T22:00:11.943460+00:00",
+                        "updated_at": "2022-07-26T22:36:23.862370+00:00",
+                        "execute_steps": ["dbt run", "dbt test"],
+                        "state": 1,
+                        "deactivated": False,
+                        "run_failure_count": 0,
+                        "triggers": {
+                            "github_webhook": False,
+                            "git_provider_webhook": False,
+                            "custom_branch_only": False,
+                            "schedule": True,
+                        },
+                        "settings": {"threads": 4, "target_name": "default"},
+                        "schedule": {
+                            "cron": "0 * * * *",
+                            "date": "days_of_week",
+                            "time": "every_hour",
+                        },
+                    },
+                    "freshness_job": {
+                        "execution": {"timeout_seconds": 0},
+                        "generate_docs": True,
+                        "run_generate_sources": False,
+                        "id": 108380,
+                        "account_id": 72449,
+                        "project_id": 134905,
+                        "environment_id": 107605,
+                        "name": "Test job",
+                        "dbt_version": "1.0.0",
+                        "raw_dbt_version": None,
+                        "created_at": "2022-07-25T22:00:11.943460+00:00",
+                        "updated_at": "2022-07-26T22:36:23.862370+00:00",
+                        "execute_steps": ["dbt run", "dbt test"],
+                        "state": 1,
+                        "deactivated": False,
+                        "run_failure_count": 0,
+                        "triggers": {
+                            "github_webhook": False,
+                            "git_provider_webhook": False,
+                            "custom_branch_only": False,
+                            "schedule": True,
+                        },
+                        "settings": {"threads": 4, "target_name": "default"},
+                        "schedule": {
+                            "cron": "0 * * * *",
+                            "date": "days_of_week",
+                            "time": "every_hour",
+                        },
+                    },
                 },
                 {
                     "name": "jaffle_shop",
                     "account_id": 72449,
                     "repository_id": 85563,
                     "connection_id": 79281,
                     "id": 134905,
@@ -426,17 +484,111 @@
                     52,
                     26,
                     669562,
                     tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
                 ),
                 "name": "Bigquery",
             },
-            "docs_job": None,
+            "docs_job": {
+                "execution": {"timeout_seconds": 0},
+                "generate_docs": True,
+                "run_generate_sources": False,
+                "id": 108380,
+                "account_id": 72449,
+                "project_id": 134905,
+                "environment_id": 107605,
+                "name": "Test job",
+                "dbt_version": "1.0.0",
+                "raw_dbt_version": None,
+                "created_at": datetime.datetime(
+                    2022,
+                    7,
+                    25,
+                    22,
+                    00,
+                    11,
+                    943460,
+                    tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+                ),
+                "updated_at": datetime.datetime(
+                    2022,
+                    7,
+                    26,
+                    22,
+                    36,
+                    23,
+                    862370,
+                    tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+                ),
+                "execute_steps": ["dbt run", "dbt test"],
+                "state": 1,
+                "deactivated": False,
+                "run_failure_count": 0,
+                "triggers": {
+                    "github_webhook": False,
+                    "git_provider_webhook": False,
+                    "custom_branch_only": False,
+                    "schedule": True,
+                },
+                "settings": {"threads": 4, "target_name": "default"},
+                "schedule": {
+                    "cron": "0 * * * *",
+                    "date": "days_of_week",
+                    "time": "every_hour",
+                },
+            },
             "freshness_job_id": None,
-            "freshness_job": None,
+            "freshness_job": {
+                "execution": {"timeout_seconds": 0},
+                "generate_docs": True,
+                "run_generate_sources": False,
+                "id": 108380,
+                "account_id": 72449,
+                "project_id": 134905,
+                "environment_id": 107605,
+                "name": "Test job",
+                "dbt_version": "1.0.0",
+                "raw_dbt_version": None,
+                "created_at": datetime.datetime(
+                    2022,
+                    7,
+                    25,
+                    22,
+                    00,
+                    11,
+                    943460,
+                    tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+                ),
+                "updated_at": datetime.datetime(
+                    2022,
+                    7,
+                    26,
+                    22,
+                    36,
+                    23,
+                    862370,
+                    tzinfo=datetime.timezone(datetime.timedelta(0), "+0000"),
+                ),
+                "execute_steps": ["dbt run", "dbt test"],
+                "state": 1,
+                "deactivated": False,
+                "run_failure_count": 0,
+                "triggers": {
+                    "github_webhook": False,
+                    "git_provider_webhook": False,
+                    "custom_branch_only": False,
+                    "schedule": True,
+                },
+                "settings": {"threads": 4, "target_name": "default"},
+                "schedule": {
+                    "cron": "0 * * * *",
+                    "date": "days_of_week",
+                    "time": "every_hour",
+                },
+            },
             "id": 113498,
             "connection_id": 79280,
             "account_id": 72449,
             "repository": {
                 "gitlab": None,
                 "deploy_key_id": 84338,
                 "account_id": 72449,
```

### Comparing `preset-cli-0.2.2/tests/api/clients/preset_test.py` & `preset-cli-0.2.3/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/api/clients/superset_test.py` & `preset-cli-0.2.3/tests/api/clients/superset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/auth/jwt_test.py` & `preset-cli-0.2.3/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/auth/lib_test.py` & `preset-cli-0.2.3/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/auth/main_test.py` & `preset-cli-0.2.3/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/auth/password_test.py` & `preset-cli-0.2.3/tests/auth/password_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/auth/preset_test.py` & `preset-cli-0.2.3/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/main_test.py` & `preset-cli-0.2.3/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/export_test.py` & `preset-cli-0.2.3/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/import_test.py` & `preset-cli-0.2.3/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/main_test.py` & `preset-cli-0.2.3/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sql_test.py` & `preset-cli-0.2.3/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/manifest.json`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/dbt/metrics_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/dbt/metrics_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.3/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tests/lib_test.py` & `preset-cli-0.2.3/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.2/tox.ini` & `preset-cli-0.2.3/tox.ini`

 * *Files identical despite different names*

