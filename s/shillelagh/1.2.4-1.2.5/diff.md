# Comparing `tmp/shillelagh-1.2.4.tar.gz` & `tmp/shillelagh-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.4.tar", last modified: Mon May 15 20:08:08 2023, max compression
+gzip compressed data, was "shillelagh-1.2.5.tar", last modified: Fri Jul 14 22:08:44 2023, max compression
```

## Comparing `shillelagh-1.2.4.tar` & `shillelagh-1.2.5.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.645756 shillelagh-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 20:07:44.000000 shillelagh-1.2.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-05-15 20:07:44.000000 shillelagh-1.2.4/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-15 20:07:44.000000 shillelagh-1.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-05-15 20:07:44.000000 shillelagh-1.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-15 20:07:44.000000 shillelagh-1.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 20:07:44.000000 shillelagh-1.2.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 20:08:08.645756 shillelagh-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-15 20:07:44.000000 shillelagh-1.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.617755 shillelagh-1.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-15 20:07:44.000000 shillelagh-1.2.4/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-15 20:07:44.000000 shillelagh-1.2.4/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-15 20:07:44.000000 shillelagh-1.2.4/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-15 20:07:44.000000 shillelagh-1.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-15 20:07:44.000000 shillelagh-1.2.4/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-15 20:08:08.645756 shillelagh-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 20:07:44.000000 shillelagh-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.613755 shillelagh-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.625755 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-15 20:07:44.000000 shillelagh-1.2.4/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.621755 shillelagh-1.2.4/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 20:08:08.000000 shillelagh-1.2.4/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-05-15 20:07:44.000000 shillelagh-1.2.4/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.613755 shillelagh-1.2.4/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.629755 shillelagh-1.2.4/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-05-15 20:07:44.000000 shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.633756 shillelagh-1.2.4/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.637755 shillelagh-1.2.4/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.641755 shillelagh-1.2.4/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:08:08.645756 shillelagh-1.2.4/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-15 20:07:44.000000 shillelagh-1.2.4/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.977698 shillelagh-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-14 22:08:32.000000 shillelagh-1.2.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-07-14 22:08:32.000000 shillelagh-1.2.5/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-14 22:08:32.000000 shillelagh-1.2.5/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-14 22:08:32.000000 shillelagh-1.2.5/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-14 22:08:32.000000 shillelagh-1.2.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-14 22:08:32.000000 shillelagh-1.2.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-14 22:08:44.977698 shillelagh-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-07-14 22:08:32.000000 shillelagh-1.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-14 22:08:32.000000 shillelagh-1.2.5/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-14 22:08:32.000000 shillelagh-1.2.5/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-14 22:08:32.000000 shillelagh-1.2.5/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-14 22:08:32.000000 shillelagh-1.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.961698 shillelagh-1.2.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-07-14 22:08:32.000000 shillelagh-1.2.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-14 22:08:44.977698 shillelagh-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 22:08:32.000000 shillelagh-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.953698 shillelagh-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-14 22:08:32.000000 shillelagh-1.2.5/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.965698 shillelagh-1.2.5/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 22:08:44.000000 shillelagh-1.2.5/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-07-14 22:08:32.000000 shillelagh-1.2.5/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.957698 shillelagh-1.2.5/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-14 22:08:32.000000 shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.969698 shillelagh-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14748 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.973698 shillelagh-1.2.5/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:08:44.977698 shillelagh-1.2.5/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 22:08:32.000000 shillelagh-1.2.5/tests/types_test.py
```

### Comparing `shillelagh-1.2.4/.coveragerc` & `shillelagh-1.2.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/pull_request_template.md` & `shillelagh-1.2.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/workflows/python-integration.yml` & `shillelagh-1.2.5/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.5/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/workflows/python-package.yml` & `shillelagh-1.2.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.github/workflows/python-publish.yml` & `shillelagh-1.2.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.gitignore` & `shillelagh-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.pre-commit-config.yaml` & `shillelagh-1.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/.readthedocs.yml` & `shillelagh-1.2.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/ARCHITECTURE.rst` & `shillelagh-1.2.5/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/CHANGELOG.rst` & `shillelagh-1.2.5/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.5 - 2023-07-14
+==========================
+
+- System adapter now supports memory (virtual/swap) queries (#369 and #372)
+
 Version 1.2.4 - 2023-05-15
 ==========================
 
 - Relax dependency for ``requests-cache`` correctly (#362)
 
 Version 1.2.3 - 2023-05-15
 ==========================
```

### Comparing `shillelagh-1.2.4/CODE_OF_CONDUCT.md` & `shillelagh-1.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/CONTRIBUTING.rst` & `shillelagh-1.2.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/LICENSE.txt` & `shillelagh-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/Makefile` & `shillelagh-1.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/PKG-INFO` & `shillelagh-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.4
+Version: 1.2.5
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.4/README.rst` & `shillelagh-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/Makefile` & `shillelagh-1.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/adapters.rst` & `shillelagh-1.2.5/docs/adapters.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/conf.py` & `shillelagh-1.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/development.rst` & `shillelagh-1.2.5/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/install.rst` & `shillelagh-1.2.5/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/docs/usage.rst` & `shillelagh-1.2.5/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/examples/csvfile.py` & `shillelagh-1.2.5/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/examples/dataframe.py` & `shillelagh-1.2.5/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/examples/datasette.py` & `shillelagh-1.2.5/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/examples/generic_json.py` & `shillelagh-1.2.5/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/examples/weatherapi.py` & `shillelagh-1.2.5/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/requirements/base.txt` & `shillelagh-1.2.5/requirements/base.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,21 +15,25 @@
     # via requests
 greenlet==2.0.2
     # via
     #   shillelagh
     #   sqlalchemy
 idna==3.3
     # via requests
+importlib-metadata==6.7.0
+    # via shillelagh
 packaging==23.0
     # via shillelagh
 python-dateutil==2.8.2
     # via shillelagh
-requests==2.28.1
+requests==2.31.0
     # via shillelagh
 six==1.16.0
     # via python-dateutil
 sqlalchemy==1.4.39
     # via shillelagh
 typing-extensions==4.3.0
     # via shillelagh
 urllib3==1.26.10
     # via requests
+zipp==3.15.0
+    # via importlib-metadata
```

### Comparing `shillelagh-1.2.4/requirements/test.txt` & `shillelagh-1.2.5/requirements/test.txt`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,16 @@
     # via shillelagh
 identify==2.5.2
     # via pre-commit
 idna==3.3
     # via
     #   requests
     #   yarl
+importlib-metadata==6.7.0
+    # via shillelagh
 iniconfig==1.1.1
     # via pytest
 isort==5.10.1
     # via pylint
 jmespath==1.0.1
     # via
     #   boto3
@@ -151,15 +153,15 @@
     #   shillelagh
 pytz==2022.1
     # via pandas
 pyyaml==6.0
     # via
     #   pre-commit
     #   shillelagh
-requests==2.28.1
+requests==2.31.0
     # via
     #   requests-cache
     #   requests-mock
     #   shillelagh
 requests-cache==1.0.1
     # via shillelagh
 requests-mock==1.9.3
@@ -213,11 +215,13 @@
     # via html5lib
 wheel==0.37.1
     # via pip-tools
 wrapt==1.14.1
     # via astroid
 yarl==1.8.1
     # via shillelagh
+zipp==3.15.0
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `shillelagh-1.2.4/setup.cfg` & `shillelagh-1.2.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0
 install_requires = 
-	importlib-metadata; python_version<"3.8"
+	importlib-metadata; python_version<"3.10"
 	apsw>=3.9.2
 	python_dateutil>=2.8.1
-	requests>=2.25.1
+	requests>=2.31.0
 	sqlalchemy>=1.3
 	greenlet>=2.0.2  # needed for Python 3.11 w/o memory leak
 	typing_extensions>=3.7.4.3
 	packaging
 python_requires = >=3.8
 obsoletes = 
 	gsheetsdb
@@ -68,15 +68,14 @@
 	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=7.2.0
 	requests-cache>=0.7.1
 	requests-mock>=1.8.0
-	requests>=2.25.1
 	tabulate==0.8.9
 	yarl>=1.8.1
 all = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	beautifulsoup4>=4.11.1
 	boto3>=1.24.28
@@ -95,15 +94,14 @@
 	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
 	pytest-mock>=3.5.1
 	pytest>=6.2.2
 	requests-cache>=0.7.1
 	requests-mock>=1.8.0
-	requests>=2.25.1
 	tabulate==0.8.9
 docs = 
 	sphinx>=4.0.1
 console = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	prompt_toolkit>=3
@@ -116,15 +114,14 @@
 	prison>=0.2.1
 	requests-cache>=0.7.1
 	yarl>=1.8.1
 githubapi = 
 	jsonpath-python>=1.0.5
 gsheetsapi = 
 	google-auth>=1.23.0
-	requests>=2.23.0
 htmltableapi = 
 	beautifulsoup4>=4.11.1
 	html5lib>=1.1
 	pandas>=1.2.2
 pandasmemory = 
 	pandas>=1.2.2
 s3selectapi = 
@@ -165,14 +162,15 @@
 	--cov shillelagh --cov-report=term-missing:skip-covered
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
+pythonpath = src
 
 [coverage:report]
 fail_under = 100
 
 [aliases]
 dists = bdist_wheel
```

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.5/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/base.py` & `shillelagh-1.2.5/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.5/src/shillelagh/adapters/file/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.5/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.5/src/shillelagh/adapters/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Inspired by SQLAlchemy's ``PluginLoader``.
 """
 
 import logging
 from collections import defaultdict
 from typing import Dict, List, Optional, Type, cast
 
-from pkg_resources import iter_entry_points
+from importlib_metadata import entry_points
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import InterfaceError
 
 _logger = logging.getLogger(__name__)
 
 
@@ -25,15 +25,15 @@
 class AdapterLoader:
     """
     Adapter registry, allowing new adapters to be registered.
     """
 
     def __init__(self):
         self.loaders = defaultdict(list)
-        for entry_point in iter_entry_points("shillelagh.adapter"):
+        for entry_point in entry_points(group="shillelagh.adapter"):
             self.loaders[entry_point.name].append(entry_point.load)
 
     def load(self, name: str, safe: bool = False, warn: bool = False) -> Type[Adapter]:
         """
         Load a given entry point by its name.
         """
         if safe and len(self.loaders[name]) > 1:
```

### Comparing `shillelagh-1.2.4/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.5/src/shillelagh/backends/apsw/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import apsw
-from packaging.version import Version
 
 from shillelagh import functions
 from shillelagh.adapters.base import Adapter
 from shillelagh.adapters.registry import registry
 from shillelagh.backends.apsw.vt import VTModule, type_map
 from shillelagh.exceptions import (  # nopycln: import; pylint: disable=redefined-builtin
     DatabaseError,
@@ -37,14 +36,15 @@
     NotSupportedError,
     OperationalError,
     ProgrammingError,
     Warning,
 )
 from shillelagh.fields import Blob, Field
 from shillelagh.lib import (
+    best_index_object_available,
     combine_args_kwargs,
     escape_identifier,
     find_adapter,
     serialize,
 )
 from shillelagh.types import (
     BINARY,
@@ -444,15 +444,15 @@
         apsw_connection_kwargs = apsw_connection_kwargs or {}
         self._connection = apsw.Connection(path, **apsw_connection_kwargs)
         self.isolation_level = isolation_level
         self.schema = schema
 
         # register adapters
         for adapter in adapters:
-            if Version(apsw.apswversion()) >= Version("3.41.0.0"):
+            if best_index_object_available():
                 self._connection.createmodule(
                     adapter.__name__,
                     VTModule(adapter),
                     use_bestindex_object=adapter.supports_requested_columns,
                 )
             else:
                 self._connection.createmodule(adapter.__name__, VTModule(adapter))
```

### Comparing `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.5/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.5/src/shillelagh/backends/apsw/vt.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     Set,
     Tuple,
     Type,
     cast,
 )
 
 import apsw
-from packaging.version import Version
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.fields import (
     Blob,
     FastISODateTime,
     Field,
@@ -38,25 +37,26 @@
     Order,
     RowID,
     String,
     StringDuration,
     StringInteger,
 )
 from shillelagh.filters import Filter, Operator
-from shillelagh.lib import deserialize
+from shillelagh.lib import best_index_object_available, deserialize
 from shillelagh.typing import (
     Constraint,
     Index,
+    OrderBy,
     RequestedOrder,
     Row,
     SQLiteConstraint,
     SQLiteValidType,
 )
 
-if Version(apsw.apswversion()) >= Version("3.41.0.0"):  # pragma: no cover
+if best_index_object_available():  # pragma: no cover
     from apsw.ext import index_info_to_dict
 else:  # pragma: no cover
     apsw.IndexInfo = Any  # for type annotation
 
     # pylint: disable=unused-argument
     def index_info_to_dict(index_info: apsw.IndexInfo) -> None:
         """
@@ -223,15 +223,15 @@
         elif operator == Operator.OFFSET:
             offset = constraint
 
     return limit, offset
 
 
 def get_order(
-    orderbys: List[Tuple[int, bool]],
+    orderbys: List[OrderBy],
     column_names: List[str],
 ) -> List[Tuple[str, RequestedOrder]]:
     """
     Return a list of column names and sort order from a SQLite orderbys.
     """
     return [
         (
@@ -314,15 +314,14 @@
 
     Each row has a unique 64 bit integer rowid with the Cursor routines operating
     on this number, as well as some of the Table routines such as UpdateChangeRow.
     """
 
     def __init__(self, adapter: Adapter):
         self.adapter = adapter
-        self.requested_columns: Optional[Set[str]] = None
 
     def get_create_table(self, tablename: str) -> str:
         """
         Return the table's ``CREATE TABLE`` statement.
         """
         columns = self.adapter.get_columns()
         if not columns:
@@ -330,24 +329,21 @@
 
         quoted_columns = {k.replace('"', '""'): v for k, v in columns.items()}
         formatted_columns = ", ".join(
             f'"{k}" {v.type}' for (k, v) in quoted_columns.items()
         )
         return f'CREATE TABLE "{tablename}" ({formatted_columns})'
 
-    def BestIndex(  # pylint: disable=too-many-locals
+    def _build_index(  # pylint: disable=too-many-locals
         self,
         constraints: List[Tuple[int, SQLiteConstraint]],
-        orderbys: List[Tuple[int, bool]],
-    ) -> Tuple[List[Constraint], int, str, bool, float]:
+        orderbys: List[OrderBy],
+    ) -> Tuple[List[Constraint], int, List[Index], List[OrderBy], bool, float]:
         """
-        Build an index for a given set of constraints and order bys.
-
-        The purpose of this method is to ask if you have the ability to determine if
-        a row meets certain constraints that doesn’t involve visiting every row.
+        Helper function to build index.
         """
         columns = self.adapter.get_columns()
         column_names = list(columns.keys())
         column_types = list(columns.values())
 
         # currently the index number is not used for anything; instead, we encode the
         # the index as JSON in ``index_name``
@@ -384,59 +380,101 @@
         # estimate query cost
         order = get_order(orderbys, column_names)
         estimated_cost = self.adapter.get_cost(filtered_columns, order)
 
         # is the data being returned in the requested order? if not, SQLite will have
         # to sort it
         orderby_consumed = True
-        orderbys_to_process: List[Tuple[int, bool]] = []
+        orderbys_to_process: List[OrderBy] = []
         for column_index, descending in orderbys:
             requested_order = Order.DESCENDING if descending else Order.ASCENDING
             column_type = column_types[column_index]
             if column_type.order == Order.ANY:
                 orderbys_to_process.append((column_index, descending))
             elif column_type.order != requested_order:
                 orderby_consumed = False
                 break
 
-        # serialize the indexes to str so it can be used later when filtering the data
-        index_name = json.dumps([indexes, orderbys_to_process])
+        return (
+            constraints_used,
+            index_number,
+            indexes,
+            orderbys_to_process,
+            orderby_consumed,
+            estimated_cost,
+        )
+
+    def BestIndex(  # pylint: disable=too-many-locals
+        self,
+        constraints: List[Tuple[int, SQLiteConstraint]],
+        orderbys: List[OrderBy],
+    ) -> Tuple[List[Constraint], int, str, bool, float]:
+        """
+        Build an index for a given set of constraints and order bys.
+
+        The purpose of this method is to ask if you have the ability to determine if
+        a row meets certain constraints that doesn’t involve visiting every row.
+        """
+        (
+            constraints_used,
+            index_number,
+            indexes,
+            orderbys_to_process,
+            orderby_consumed,
+            estimated_cost,
+        ) = self._build_index(constraints, orderbys)
+
+        index_name = json.dumps(
+            {"indexes": indexes, "orderbys_to_process": orderbys_to_process},
+        )
 
         return (
             constraints_used,
             index_number,
             index_name,
             orderby_consumed,
             estimated_cost,
         )
 
-    def BestIndexObject(self, index_info: apsw.IndexInfo) -> bool:
+    def BestIndexObject(  # pylint: disable=too-many-locals
+        self,
+        index_info: apsw.IndexInfo,
+    ) -> bool:
         """
         Alternative to ``BestIndex`` that allows returning only selected columns.
         """
         columns = self.adapter.get_columns()
         column_names = list(columns.keys())
-        self.requested_columns = {column_names[i] for i in index_info.colUsed}
 
         index_info_dict = index_info_to_dict(index_info)
         constraints = [
             (constraint.get("iColumn", -1), constraint["op"])
             for constraint in index_info_dict["aConstraint"]
         ]
         orderbys = [
             (orderby["iColumn"], orderby["desc"])
             for orderby in index_info_dict["aOrderBy"]
         ]
         (
             constraints_used,
             index_number,
-            index_name,
+            indexes,
+            orderbys_to_process,
             orderby_consumed,
             estimated_cost,
-        ) = self.BestIndex(constraints, orderbys)
+        ) = self._build_index(constraints, orderbys)
+
+        requested_columns = sorted({column_names[i] for i in index_info.colUsed})
+        index_name = json.dumps(
+            {
+                "indexes": indexes,
+                "orderbys_to_process": orderbys_to_process,
+                "requested_columns": requested_columns,
+            },
+        )
 
         for i, constraint in enumerate(constraints_used):
             if isinstance(constraint, tuple):
                 index_info.set_aConstraintUsage_argvIndex(i, constraint[0] + 1)
                 index_info.set_aConstraintUsage_omit(i, constraint[1])
         index_info.idxNum = index_number
         index_info.idxStr = index_name
@@ -445,15 +483,15 @@
 
         return True
 
     def Open(self) -> "VTCursor":
         """
         Returns a cursor object.
         """
-        return VTCursor(self.adapter, self.requested_columns)
+        return VTCursor(self.adapter)
 
     def Disconnect(self) -> None:
         """
         The opposite of VTModule.Connect().
 
         This method is called when a reference to a virtual table is no longer used,
         but VTTable.Destroy() will be called when the table is no longer used.
@@ -501,17 +539,16 @@
 
 
 class VTCursor:
     """
     An object for iterating over a table.
     """
 
-    def __init__(self, adapter: Adapter, requested_columns: Optional[Set[str]] = None):
+    def __init__(self, adapter: Adapter):
         self.adapter = adapter
-        self.requested_columns = requested_columns
 
         self.data: Iterator[Tuple[Any, ...]]
         self.current_row: Tuple[Any, ...]
         self.eof = False
 
     def Filter(  # pylint: disable=too-many-locals
         self,
@@ -526,16 +563,16 @@
         and the order to sort the results) and ``constraintargs`` into a pair of
         ``bounds`` and ``order``. These are then passed to the ``get_rows`` method of
         the adapter, to filter and sort the data.
         """
         columns: Dict[str, Field] = self.adapter.get_columns()
         column_names: List[str] = list(columns.keys())
         index = json.loads(indexname)
-        indexes: List[Index] = index[0]
-        orderbys: List[Tuple[int, bool]] = index[1]
+        indexes: List[Index] = index["indexes"]
+        orderbys: List[OrderBy] = index["orderbys_to_process"]
 
         # compute bounds for each column
         all_bounds = get_all_bounds(indexes, constraintargs, columns)
         limit, offset = get_limit_offset(indexes, constraintargs)
         bounds = get_bounds(columns, all_bounds)
 
         # compute requested order
@@ -543,16 +580,16 @@
 
         # limit and offset were introduced in 1.1, and not all adapters support it
         kwargs: Dict[str, Any] = {}
         if self.adapter.supports_limit:
             kwargs["limit"] = limit
         if self.adapter.supports_offset:
             kwargs["offset"] = offset
-        if self.adapter.supports_requested_columns:
-            kwargs["requested_columns"] = self.requested_columns
+        if "requested_columns" in index:
+            kwargs["requested_columns"] = set(index["requested_columns"])
 
         rows = self.adapter.get_rows(bounds, order, **kwargs)
         rows = convert_rows_to_sqlite(columns, rows)
 
         # if a given column is not present, replace it with ``None``
         self.data = (
             tuple(row.get(name) for name in ["rowid", *column_names]) for row in rows
```

### Comparing `shillelagh-1.2.4/src/shillelagh/console.py` & `shillelagh-1.2.5/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/exceptions.py` & `shillelagh-1.2.5/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/fields.py` & `shillelagh-1.2.5/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/filters.py` & `shillelagh-1.2.5/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/functions.py` & `shillelagh-1.2.5/src/shillelagh/functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Custom functions available to the SQL backend.
 """
 import json
 import time
 from typing import Any, Dict, List, Type
 
-import pkg_resources
+from importlib_metadata import distribution
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.lib import find_adapter
 
 __all__ = ["sleep", "get_metadata", "version"]
 
 
@@ -67,8 +67,8 @@
 
         sql> SELECT VERSION();
         VERSION()
         -----------
         0.7.4
 
     """
-    return pkg_resources.get_distribution("shillelagh").version
+    return str(distribution("shillelagh").version)
```

### Comparing `shillelagh-1.2.4/src/shillelagh/lib.py` & `shillelagh-1.2.5/src/shillelagh/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,29 @@
 import base64
 import inspect
 import itertools
 import json
 import marshal
 import math
 import operator
-from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    TypeVar,
+)
+
+import apsw
+from packaging.version import Version
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ImpossibleFilterError, ProgrammingError
 from shillelagh.fields import Boolean, Field, Float, Integer, Order, String
 from shillelagh.filters import (
     Equal,
     Filter,
@@ -389,28 +403,38 @@
 def is_not_null(column: Any, _: Any) -> bool:
     """
     Operator for ``IS NOT NULL``.
     """
     return column is not None
 
 
-def filter_data(
+def filter_data(  # pylint: disable=too-many-arguments
     data: Iterator[Row],
     bounds: Dict[str, Filter],
     order: List[Tuple[str, RequestedOrder]],
     limit: Optional[int] = None,
     offset: Optional[int] = None,
+    requested_columns: Optional[Set[str]] = None,
 ) -> Iterator[Row]:
     """
     Apply filtering and sorting to a stream of rows.
 
     This is used mostly as an exercise. It's probably much more efficient to
     simply declare fields without any filtering/sorting and let the backend
     (SQLite, eg) handle it.
     """
+    data = (
+        {
+            k: v
+            for k, v in row.items()
+            if requested_columns is None or k in requested_columns
+        }
+        for row in data
+    )
+
     for column_name, filter_ in bounds.items():
 
         def apply_filter(
             data: Iterator[Row],
             operator_: Callable[[Any, Any], bool],
             column_name: str,
             value: Any,
@@ -539,7 +563,14 @@
 def flatten(row: Row) -> Row:
     """
     Function that converts JSON to strings, to flatten rows.
     """
     return {
         k: json.dumps(v) if isinstance(v, (list, dict)) else v for k, v in row.items()
     }
+
+
+def best_index_object_available() -> bool:
+    """
+    Check if support for best index object is available.
+    """
+    return bool(Version(apsw.apswversion()) >= Version("3.41.0.0"))
```

### Comparing `shillelagh-1.2.4/src/shillelagh/types.py` & `shillelagh-1.2.5/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh/typing.py` & `shillelagh-1.2.5/src/shillelagh/typing.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 # A row of data
 Row = Dict[str, Any]
 
 # An index is a tuple with a column index and an operator to filter it
 Index = Tuple[int, SQLiteConstraint]
 
+OrderBy = Tuple[int, bool]
 RequestedOrder = Union[Literal[Order.ASCENDING], Literal[Order.DESCENDING]]
 
 SQLiteValidType = Union[None, int, float, str, bytes]
 
 
 # Cursor description
 Description = Optional[
```

### Comparing `shillelagh-1.2.4/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.5/src/shillelagh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.4
+Version: 1.2.5
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.4/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.5/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.5/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.5/src/shillelagh.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 apsw>=3.9.2
 python_dateutil>=2.8.1
-requests>=2.25.1
+requests>=2.31.0
 sqlalchemy>=1.3
 greenlet>=2.0.2
 typing_extensions>=3.7.4.3
 packaging
 
-[:python_version < "3.8"]
+[:python_version < "3.10"]
 importlib-metadata
 
 [all]
 PyYAML>=5.4
 appdirs>=1.4.4
 beautifulsoup4>=4.11.1
 boto3>=1.24.28
@@ -29,15 +29,14 @@
 pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=6.2.2
 requests-cache>=0.7.1
 requests-mock>=1.8.0
-requests>=2.25.1
 tabulate==0.8.9
 
 [console]
 PyYAML>=5.4
 appdirs>=1.4.4
 prompt_toolkit>=3
 pygments>=2.8
@@ -56,15 +55,14 @@
 yarl>=1.8.1
 
 [githubapi]
 jsonpath-python>=1.0.5
 
 [gsheetsapi]
 google-auth>=1.23.0
-requests>=2.23.0
 
 [htmltableapi]
 beautifulsoup4>=4.11.1
 html5lib>=1.1
 pandas>=1.2.2
 
 [pandasmemory]
@@ -101,13 +99,12 @@
 pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
 pytest-mock>=3.5.1
 pytest>=7.2.0
 requests-cache>=0.7.1
 requests-mock>=1.8.0
-requests>=2.25.1
 tabulate==0.8.9
 yarl>=1.8.1
 
 [weatherapi]
 requests-cache>=0.7.1
```

### Comparing `shillelagh-1.2.4/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.5/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.5/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.5/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.5/tests/adapters/api/generic_json_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/github_test.py` & `shillelagh-1.2.5/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.5/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.5/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.5/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.5/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.5/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/base_test.py` & `shillelagh-1.2.5/tests/adapters/base_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Test for shillelagh.adapter.base.
 """
 from datetime import datetime
-from typing import List
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 
 import pytest
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.adapters.registry import AdapterLoader
 from shillelagh.backends.apsw.db import connect
 from shillelagh.exceptions import NotSupportedError
 from shillelagh.fields import DateTime, Order
-from shillelagh.filters import Equal, Range
-from shillelagh.typing import Row
+from shillelagh.filters import Equal, Filter, Range
+from shillelagh.typing import RequestedOrder, Row
 
 from ..fakes import FakeAdapter
 
 
 class FakeAdapterWithDateTime(FakeAdapter):
 
     """
@@ -180,23 +180,40 @@
 
     class CustomFakeAdapter(FakeAdapter):
 
         """
         Custom ``FakeAdapter`` with more data.
         """
 
+        supports_limit = False
+        supports_offset = False
+
         def __init__(self):
             super().__init__()
 
             self.data = [
                 {"rowid": 0, "name": "Alice", "age": 20, "pets": 0},
                 {"rowid": 1, "name": "Bob", "age": 23, "pets": 3},
                 {"rowid": None, "name": "Charlie", "age": 6, "pets": 1},
             ]
 
+        def get_data(  # pylint: disable=too-many-arguments
+            self,
+            bounds: Dict[str, Filter],
+            order: List[Tuple[str, RequestedOrder]],
+            limit: Optional[int] = None,
+            offset: Optional[int] = None,
+            requested_columns: Optional[Set[str]] = None,
+            **kwargs: Any
+        ) -> Iterator[Row]:
+            """
+            Return all data.
+            """
+            return iter(self.data)
+
     class FakeAdapterWithLimitOnly(CustomFakeAdapter):
 
         """
         An adapter that only supports limit (like ``s3select``)
         """
 
         scheme = "limit"
```

### Comparing `shillelagh-1.2.4/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.5/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.5/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/adapters/registry_test.py` & `shillelagh-1.2.5/tests/adapters/registry_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/backends/apsw/db_test.py` & `shillelagh-1.2.5/tests/backends/apsw/db_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,21 +486,27 @@
     # pylint: disable=redefined-outer-name, invalid-name
     apsw = mocker.patch("shillelagh.backends.apsw.db.apsw")
     VTModule = mocker.patch("shillelagh.backends.apsw.db.VTModule")
     adapter = mocker.MagicMock()
     adapter.__name__ = "some_adapter"
     adapter.supports_requested_columns = True
 
-    apsw.apswversion.return_value = "3.41.0.0"
+    mocker.patch(
+        "shillelagh.backends.apsw.db.best_index_object_available",
+        return_value=True,
+    )
     Connection(":memory:", [adapter], {})
     apsw.Connection().createmodule.assert_called_with(
         "some_adapter",
         VTModule(adapter),
         use_bestindex_object=True,
     )
 
-    apsw.apswversion.return_value = "3.40.1.0"
+    mocker.patch(
+        "shillelagh.backends.apsw.db.best_index_object_available",
+        return_value=False,
+    )
     Connection(":memory:", [adapter], {})
     apsw.Connection().createmodule.assert_called_with(
         "some_adapter",
         VTModule(adapter),
     )
```

### Comparing `shillelagh-1.2.4/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.5/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.5/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.5/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.5/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.5/tests/backends/apsw/vt_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=c-extension-no-member
 """
 Tests for shillelagh.backends.apsw.vt.
 """
 import datetime
+import json
 from typing import Any, Dict, Iterable
 
 import apsw
 import pytest
 from pytest_mock import MockerFixture
 
 from shillelagh.backends.apsw.vt import (
@@ -98,18 +99,19 @@
             (-1, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # INVALID, just for coverage
         ],
         [(1, False)],  # ORDER BY name ASC
     )
     assert result == (
         [(0, True), None, (1, True), (2, True)],
         42,
-        (
-            f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}], "
-            f"[0, {apsw.SQLITE_INDEX_CONSTRAINT_LE}], [-1, 73]], "
-            "[[1, false]]]"
+        json.dumps(
+            {
+                "indexes": [[1, 2], [0, 8], [-1, 73]],
+                "orderbys_to_process": [[1, False]],
+            },
         ),
         True,
         666,
     )
 
 
 def test_virtual_best_index_object(mocker: MockerFixture) -> None:
@@ -129,19 +131,17 @@
         "aOrderBy": [{"iColumn": 1, "desc": False}],
     }
 
     adapter = FakeAdapter()
     adapter.supports_limit = True
 
     table = VTTable(adapter)
-    assert table.requested_columns is None
 
     result = table.BestIndexObject(index_info)
     assert result is True
-    assert table.requested_columns == {"age", "pets"}
 
     index_info.set_aConstraintUsage_argvIndex.assert_has_calls(
         [
             mocker.call(0, 1),
             mocker.call(2, 2),
             mocker.call(3, 3),
         ],
@@ -150,18 +150,20 @@
         [
             mocker.call(0, True),
             mocker.call(2, True),
             mocker.call(3, True),
         ],
     )
     assert index_info.idxNum == 42
-    assert index_info.idxStr == (
-        f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}], "
-        f"[0, {apsw.SQLITE_INDEX_CONSTRAINT_LE}], [-1, 73]], "
-        "[[1, false]]]"
+    assert index_info.idxStr == json.dumps(
+        {
+            "indexes": [[1, 2], [0, 8], [-1, 73]],
+            "orderbys_to_process": [[1, False]],
+            "requested_columns": ["age", "pets"],
+        },
     )
     assert index_info.orderByConsumed is True
     assert index_info.estimatedCost == 666
 
 
 def test_virtual_best_index_static_order_not_consumed() -> None:
     """
@@ -175,15 +177,15 @@
             (0, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # age <=
         ],
         [(1, False)],  # ORDER BY name ASC
     )
     assert result == (
         [(0, False), None, None],
         42,
-        f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}]], []]",
+        json.dumps({"indexes": [[1, 2]], "orderbys_to_process": []}),
         True,
         666,
     )
 
 
 def test_virtual_best_index_static_order_not_consumed_descending() -> None:
     """
@@ -197,30 +199,36 @@
             (0, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # age <=
         ],
         [(0, True)],  # ORDER BY age DESC
     )
     assert result == (
         [(0, False), None, None],
         42,
-        f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}]], []]",
+        json.dumps({"indexes": [[1, 2]], "orderbys_to_process": []}),
         False,
         666,
     )
 
 
 def test_virtual_best_index_operator_not_supported() -> None:
     """
     Test ``BestIndex`` with an unsupported operator.
     """
     table = VTTable(FakeAdapter())
     result = table.BestIndex(
         [(1, apsw.SQLITE_INDEX_CONSTRAINT_MATCH)],  # name LIKE?
         [(1, False)],  # ORDER BY name ASC
     )
-    assert result == ([None], 42, "[[], [[1, false]]]", True, 666)
+    assert result == (
+        [None],
+        42,
+        json.dumps({"indexes": [], "orderbys_to_process": [[1, False]]}),
+        True,
+        666,
+    )
 
 
 def test_virtual_best_index_order_consumed() -> None:
     """
     Test ``BestIndex`` when the adapter can consume the order.
     """
     table = VTTable(FakeAdapter())
@@ -231,18 +239,15 @@
             (0, apsw.SQLITE_INDEX_CONSTRAINT_LE),  # age <=
         ],
         [(0, True)],  # ORDER BY age DESC
     )
     assert result == (
         [(0, True), None, (1, True)],
         42,
-        (
-            f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}], "
-            f"[0, {apsw.SQLITE_INDEX_CONSTRAINT_LE}]], [[0, true]]]"
-        ),
+        json.dumps({"indexes": [[1, 2], [0, 8]], "orderbys_to_process": [[0, True]]}),
         True,
         666,
     )
 
 
 def test_virtual_disconnect() -> None:
     """
@@ -312,15 +317,15 @@
 
 def test_cursor() -> None:
     """
     Test the cursor.
     """
     table = VTTable(FakeAdapter())
     cursor = table.Open()
-    cursor.Filter(42, "[[], []]", [])
+    cursor.Filter(42, json.dumps({"indexes": [], "orderbys_to_process": []}), [])
     assert cursor.current_row == (0, 20, "Alice", "0")
     assert cursor.Rowid() == 0
     assert cursor.Column(0) == 20
 
     cursor.Next()
     assert cursor.current_row == (1, 23, "Bob", "3")
 
@@ -332,59 +337,95 @@
 
 def test_cursor_with_constraints() -> None:
     """
     Test filtering a cursor.
     """
     table = VTTable(FakeAdapter())
     cursor = table.Open()
-    cursor.Filter(42, f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}]], []]", ["Alice"])
+    cursor.Filter(
+        42,
+        json.dumps({"indexes": [[1, 2]], "orderbys_to_process": []}),
+        ["Alice"],
+    )
     assert cursor.current_row == (0, 20, "Alice", "0")
 
     assert not cursor.Eof()
     cursor.Next()
     assert cursor.Eof()
 
 
+def test_cursor_with_constraints_with_requested_columns() -> None:
+    """
+    Test filtering a cursor with requested_columns.
+    """
+    table = VTTable(FakeAdapter())
+    cursor = table.Open()
+    cursor.Filter(
+        42,
+        json.dumps(
+            {
+                "indexes": [[1, 2]],
+                "orderbys_to_process": [],
+                "requested_columns": ["name"],
+            },
+        ),
+        ["Alice"],
+    )
+    assert cursor.current_row == (None, None, "Alice", None)
+
+    assert not cursor.Eof()
+    cursor.Next()
+    assert cursor.Eof()
+
+
 def test_cursor_with_constraints_invalid_filter() -> None:
     """
     Test passing an invalid constraint to a cursor.
     """
     table = VTTable(FakeAdapter())
     cursor = table.Open()
 
     with pytest.raises(Exception) as excinfo:
         cursor.Filter(
             42,
-            f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_MATCH}]], []]",
+            json.dumps({"indexes": [[1, 64]], "orderbys_to_process": []}),
             ["Alice"],
         )
 
     assert str(excinfo.value) == "Invalid constraint passed: 64"
 
 
 def test_cursor_with_constraints_no_filters() -> None:
     """
     Test passing a constraint to an adapter that cannot be filtered.
     """
     table = VTTable(FakeAdapterNoFilters())
     cursor = table.Open()
     with pytest.raises(Exception) as excinfo:
-        cursor.Filter(42, f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_EQ}]], []]", ["Alice"])
+        cursor.Filter(
+            42,
+            json.dumps({"indexes": [[1, 2]], "orderbys_to_process": []}),
+            ["Alice"],
+        )
 
     assert str(excinfo.value) == "No valid filter found"
 
 
 def test_cursor_with_constraints_only_equal() -> None:
     """
     Test passing a constraint not supported by the adapter.
     """
     table = VTTable(FakeAdapterOnlyEqual())
     cursor = table.Open()
     with pytest.raises(Exception) as excinfo:
-        cursor.Filter(42, f"[[[1, {apsw.SQLITE_INDEX_CONSTRAINT_GE}]], []]", ["Alice"])
+        cursor.Filter(
+            42,
+            json.dumps({"indexes": [[1, 32]], "orderbys_to_process": []}),
+            ["Alice"],
+        )
 
     assert str(excinfo.value) == "No valid filter found"
 
 
 def test_adapter_with_no_columns() -> None:
     """
     Test creating a table without columns.
```

### Comparing `shillelagh-1.2.4/tests/conftest.py` & `shillelagh-1.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/console_test.py` & `shillelagh-1.2.5/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/__init__.py` & `shillelagh-1.2.5/tests/fakes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Fake objects to simplify testing.
 """
 
 import json
 import os
 import urllib.parse
-from typing import Any, Dict, Iterator, List, Optional, Tuple, Type
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Type
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.fields import Float, Integer, Order, String
 from shillelagh.filters import Equal, Filter, Range
 from shillelagh.lib import filter_data
 from shillelagh.typing import RequestedOrder, Row
 
@@ -36,16 +36,17 @@
     A simple adapter that keeps data in memory.
     """
 
     scheme = "dummy"
 
     safe = True
 
-    supports_limit = False
-    supports_offset = False
+    supports_limit = True
+    supports_offset = True
+    supports_requested_columns = True
 
     age = Float(filters=[Range], order=Order.ANY, exact=True)
     name = String(filters=[Equal], order=Order.ANY, exact=True)
     pets = Integer(order=Order.ANY)
 
     @classmethod
     def supports(cls, uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
@@ -60,21 +61,31 @@
         super().__init__()
 
         self.data = [
             {"rowid": 0, "name": "Alice", "age": 20, "pets": 0},
             {"rowid": 1, "name": "Bob", "age": 23, "pets": 3},
         ]
 
-    def get_data(
+    def get_data(  # pylint: disable=too-many-arguments
         self,
         bounds: Dict[str, Filter],
         order: List[Tuple[str, RequestedOrder]],
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+        requested_columns: Optional[Set[str]] = None,
         **kwargs: Any,
-    ) -> Iterator[Dict[str, Any]]:
-        yield from filter_data(iter(self.data), bounds, order)
+    ) -> Iterator[Row]:
+        yield from filter_data(
+            iter(self.data),
+            bounds,
+            order,
+            limit,
+            offset,
+            requested_columns,
+        )
 
     def insert_data(self, row: Row) -> int:
         row_id: Optional[int] = row["rowid"]
         if row_id is None:
             max_rowid = max(row["rowid"] for row in self.data) if self.data else 0
             row["rowid"] = row_id = max_rowid + 1
```

### Comparing `shillelagh-1.2.4/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.5/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.5/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.5/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.5/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.5/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.5/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/datasette_results.json` & `shillelagh-1.2.5/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/github_response.json` & `shillelagh-1.2.5/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/github_single_response.json` & `shillelagh-1.2.5/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/incidents.json` & `shillelagh-1.2.5/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.5/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/fields_test.py` & `shillelagh-1.2.5/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/filters_test.py` & `shillelagh-1.2.5/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/functions_test.py` & `shillelagh-1.2.5/tests/functions_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Tests for shillelagh.functions.
 """
 import json
 
 import apsw
-import pkg_resources
 import pytest
+from importlib_metadata import distribution
 from pytest_mock import MockerFixture
 
 from shillelagh.adapters.registry import AdapterLoader
 from shillelagh.backends.apsw.db import connect
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.functions import get_metadata
 
@@ -69,11 +69,11 @@
 def test_version_from_sql() -> None:
     """
     Test calling ``version`` from SQL.
     """
     connection = connect(":memory:")
     cursor = connection.cursor()
     cursor.execute("SELECT version()")
-    shillelagh_version = pkg_resources.get_distribution("shillelagh").version
+    shillelagh_version = distribution("shillelagh").version
     apsw_version = apsw.apswversion()  # pylint: disable=c-extension-no-member
     version = f"{shillelagh_version} (apsw {apsw_version})"
     assert cursor.fetchall() == [(version,)]
```

### Comparing `shillelagh-1.2.4/tests/lib_test.py` & `shillelagh-1.2.5/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.4/tests/types_test.py` & `shillelagh-1.2.5/tests/types_test.py`

 * *Files identical despite different names*

