# Comparing `tmp/pecan-1.5.0.tar.gz` & `tmp/pecan-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pecan-1.5.0.tar", last modified: Fri Jul 14 15:07:04 2023, max compression
+gzip compressed data, was "pecan-1.5.1.tar", last modified: Sat Jul 15 14:48:01 2023, max compression
```

## Comparing `pecan-1.5.0.tar` & `pecan-1.5.1.tar`

### file list

```diff
@@ -1,162 +1,160 @@
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.495615 pecan-1.5.0/
--rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-14 15:06:47.000000 pecan-1.5.0/AUTHORS
--rw-r--r--   0 rpetrello   (502) staff       (20)     1505 2023-07-14 15:06:47.000000 pecan-1.5.0/LICENSE
--rw-r--r--   0 rpetrello   (502) staff       (20)      287 2023-07-14 15:06:47.000000 pecan-1.5.0/MANIFEST.in
--rw-r--r--   0 rpetrello   (502) staff       (20)     1280 2023-07-14 15:07:04.495684 pecan-1.5.0/PKG-INFO
--rw-r--r--   0 rpetrello   (502) staff       (20)     1239 2023-07-14 15:06:47.000000 pecan-1.5.0/README.rst
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.479584 pecan-1.5.0/bin/
--rw-r--r--   0 rpetrello   (502) staff       (20)      135 2023-07-14 15:06:47.000000 pecan-1.5.0/bin/pecan
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.481579 pecan-1.5.0/pecan/
--rw-r--r--   0 rpetrello   (502) staff       (20)     5028 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483112 pecan-1.5.0/pecan/commands/
--rw-r--r--   0 rpetrello   (502) staff       (20)      175 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4695 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/base.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1656 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/create.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6827 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/serve.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5525 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/commands/shell.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483239 pecan-1.5.0/pecan/compat/
--rw-r--r--   0 rpetrello   (502) staff       (20)      692 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/compat/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     7196 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/configuration.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    32093 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/core.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5826 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/decorators.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      182 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/deploy.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.483368 pecan-1.5.0/pecan/ext/
--rw-r--r--   0 rpetrello   (502) staff       (20)      133 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/ext/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2573 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/extensions.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    12809 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/hooks.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4909 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/jsonify.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1670 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/log.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.484348 pecan-1.5.0/pecan/middleware/
--rw-r--r--   0 rpetrello   (502) staff       (20)       73 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2978 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/debug.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2560 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/errordocument.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6948 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/recursive.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5588 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/middleware/static.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    15361 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/rest.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    11597 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/routing.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.484485 pecan-1.5.0/pecan/scaffolds/
--rw-r--r--   0 rpetrello   (502) staff       (20)     3982 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485010 pecan-1.5.0/pecan/scaffolds/base/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485396 pecan-1.5.0/pecan/scaffolds/base/+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/app.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485767 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      629 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/root.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.485940 pecan-1.5.0/pecan/scaffolds/base/+package+/model/
--rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/model/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.486374 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/
--rw-r--r--   0 rpetrello   (502) staff       (20)      273 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/error.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      865 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/index.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      448 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/templates/layout.html
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.486918 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      563 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      691 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_units.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       27 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/MANIFEST.in
--rw-r--r--   0 rpetrello   (502) staff       (20)     1490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/config.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.465188 pecan-1.5.0/pecan/scaffolds/base/public/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487055 pecan-1.5.0/pecan/scaffolds/base/public/css/
--rw-r--r--   0 rpetrello   (502) staff       (20)      569 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/public/css/style.css
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487185 pecan-1.5.0/pecan/scaffolds/base/public/images/
--rw-r--r--   0 rpetrello   (502) staff       (20)    20596 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/public/images/logo.png
--rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/setup.cfg_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/base/setup.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487605 pecan-1.5.0/pecan/scaffolds/rest-api/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.487986 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      339 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/app.py_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488228 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1085 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/root.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      496 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/errors.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488364 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/model/
--rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/model/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.488900 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      384 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)     1174 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_units.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1311 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/config.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/setup.cfg_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/scaffolds/rest-api/setup.py_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)     7084 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/secure.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     8391 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/templating.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1711 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/testing.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.490891 pecan-1.5.0/pecan/tests/
--rw-r--r--   0 rpetrello   (502) staff       (20)      197 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.491407 pecan-1.5.0/pecan/tests/config_fixtures/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.491664 pecan-1.5.0/pecan/tests/config_fixtures/bad/
--rw-r--r--   0 rpetrello   (502) staff       (20)       36 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/bad/importerror.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/bad/module_and_underscore.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      439 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/config.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       21 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/empty.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       12 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/foobar.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      338 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/config_fixtures/forcedict.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492166 pecan-1.5.0/pecan/tests/middleware/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492434 pecan-1.5.0/pecan/tests/middleware/static_fixtures/
--rw-r--r--   0 rpetrello   (502) staff       (20)     6976 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/static_fixtures/self.png
--rw-r--r--   0 rpetrello   (502) staff       (20)      473 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/static_fixtures/text.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)     3002 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_errordocument.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5499 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_recursive.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2390 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/middleware/test_static.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4467 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_builder.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492561 pecan-1.5.0/pecan/tests/scaffold_fixtures/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/__init__.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492669 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492801 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/bar/
--rw-r--r--   0 rpetrello   (502) staff       (20)       17 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/bar/spam.txt_tmpl
--rw-r--r--   0 rpetrello   (502) staff       (20)       15 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/content_sub/foo_tmpl
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.492937 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493068 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/spam.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/file_sub/foo_+package+
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493194 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.493323 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/bar/
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/bar/spam.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/scaffold_fixtures/simple/foo
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.495480 pecan-1.5.0/pecan/tests/templates/
--rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/__init__.py
--rw-r--r--   0 rpetrello   (502) staff       (20)      207 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      139 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      128 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_colors_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      143 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_login_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      116 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_login_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       75 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      147 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_invalid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      152 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_invalid_custom.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       57 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/form_name_valid.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      472 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/genshi.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/genshi_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      115 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/jinja.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      163 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/jinja_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      109 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/kajiki.html
--rw-r--r--   0 rpetrello   (502) staff       (20)      108 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/mako.html
--rw-r--r--   0 rpetrello   (502) staff       (20)       46 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/templates/mako_bad.html
--rw-r--r--   0 rpetrello   (502) staff       (20)    73374 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_base.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1611 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_commands.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    12788 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_conf.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     2915 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_generic.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    51501 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_hooks.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     6648 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_jsonify.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    49620 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_no_thread_locals.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    44973 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_rest.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     5189 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_scaffolds.py
--rw-r--r--   0 rpetrello   (502) staff       (20)    17728 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_secure.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1421 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_templating.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     4239 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/tests/test_util.py
--rw-r--r--   0 rpetrello   (502) staff       (20)     1498 2023-07-14 15:06:47.000000 pecan-1.5.0/pecan/util.py
-drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-14 15:07:04.482478 pecan-1.5.0/pecan.egg-info/
--rw-r--r--   0 rpetrello   (502) staff       (20)     1280 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/PKG-INFO
--rw-r--r--   0 rpetrello   (502) staff       (20)     4349 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/SOURCES.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/dependency_links.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)      393 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/entry_points.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/not-zip-safe
--rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/requires.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-14 15:07:04.000000 pecan-1.5.0/pecan.egg-info/top_level.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-14 15:06:47.000000 pecan-1.5.0/requirements.txt
--rw-r--r--   0 rpetrello   (502) staff       (20)      209 2023-07-14 15:07:04.495947 pecan-1.5.0/setup.cfg
--rw-r--r--   0 rpetrello   (502) staff       (20)     3167 2023-07-14 15:06:47.000000 pecan-1.5.0/setup.py
--rw-r--r--   0 rpetrello   (502) staff       (20)       94 2023-07-14 15:06:47.000000 pecan-1.5.0/test-requirements.txt
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.144340 pecan-1.5.1/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-15 14:41:22.000000 pecan-1.5.1/AUTHORS
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1505 2023-07-15 14:41:22.000000 pecan-1.5.1/LICENSE
+-rw-r--r--   0 rpetrello   (502) staff       (20)      287 2023-07-15 14:41:22.000000 pecan-1.5.1/MANIFEST.in
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1303 2023-07-15 14:48:01.144419 pecan-1.5.1/PKG-INFO
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1239 2023-07-15 14:41:22.000000 pecan-1.5.1/README.rst
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.121570 pecan-1.5.1/pecan/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5028 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.128999 pecan-1.5.1/pecan/commands/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      175 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/commands/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4783 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/commands/base.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1656 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/commands/create.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6827 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/commands/serve.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5525 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/commands/shell.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.129195 pecan-1.5.1/pecan/compat/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      692 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/compat/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     7196 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/configuration.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    32093 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/core.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5826 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/decorators.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      182 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/deploy.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.129384 pecan-1.5.1/pecan/ext/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      133 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/ext/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2573 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/extensions.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    12809 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/hooks.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4909 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/jsonify.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1670 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/log.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.130458 pecan-1.5.1/pecan/middleware/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       73 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/middleware/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2978 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/middleware/debug.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2560 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/middleware/errordocument.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6948 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/middleware/recursive.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5588 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/middleware/static.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    15361 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/rest.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    11597 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/routing.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.130617 pecan-1.5.1/pecan/scaffolds/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3982 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.131297 pecan-1.5.1/pecan/scaffolds/base/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.131656 pecan-1.5.1/pecan/scaffolds/base/+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      262 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/app.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.131976 pecan-1.5.1/pecan/scaffolds/base/+package+/controllers/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/controllers/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      629 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/controllers/root.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.132154 pecan-1.5.1/pecan/scaffolds/base/+package+/model/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/model/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.132679 pecan-1.5.1/pecan/scaffolds/base/+package+/templates/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      273 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/templates/error.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      865 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/templates/index.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      448 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/templates/layout.html
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.133411 pecan-1.5.1/pecan/scaffolds/base/+package+/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      563 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/tests/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      691 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/+package+/tests/test_units.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       27 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/MANIFEST.in
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1490 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/config.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.115422 pecan-1.5.1/pecan/scaffolds/base/public/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.133564 pecan-1.5.1/pecan/scaffolds/base/public/css/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      569 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/public/css/style.css
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.133717 pecan-1.5.1/pecan/scaffolds/base/public/images/
+-rw-r--r--   0 rpetrello   (502) staff       (20)    20596 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/public/images/logo.png
+-rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/setup.cfg_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/base/setup.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.134229 pecan-1.5.1/pecan/scaffolds/rest-api/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.134648 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      339 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/app.py_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.134905 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/controllers/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/controllers/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1085 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/controllers/root.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      496 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/errors.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.135057 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/model/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      463 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/model/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.135685 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      384 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1174 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      113 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/test_units.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1311 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/config.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)       92 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/setup.cfg_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)      490 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/scaffolds/rest-api/setup.py_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)     7084 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/secure.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     8391 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/templating.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1711 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/testing.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.138174 pecan-1.5.1/pecan/tests/
+-rw-r--r--   0 rpetrello   (502) staff       (20)      197 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.138774 pecan-1.5.1/pecan/tests/config_fixtures/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.139068 pecan-1.5.1/pecan/tests/config_fixtures/bad/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       36 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/bad/importerror.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/bad/module_and_underscore.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      439 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/config.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       21 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/empty.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       12 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/foobar.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      338 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/config_fixtures/forcedict.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.139630 pecan-1.5.1/pecan/tests/middleware/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.139948 pecan-1.5.1/pecan/tests/middleware/static_fixtures/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6976 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/static_fixtures/self.png
+-rw-r--r--   0 rpetrello   (502) staff       (20)      473 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/static_fixtures/text.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3002 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/test_errordocument.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5499 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/test_recursive.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2390 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/middleware/test_static.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4467 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_builder.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140096 pecan-1.5.1/pecan/tests/scaffold_fixtures/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/__init__.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140201 pecan-1.5.1/pecan/tests/scaffold_fixtures/content_sub/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140360 pecan-1.5.1/pecan/tests/scaffold_fixtures/content_sub/bar/
+-rw-r--r--   0 rpetrello   (502) staff       (20)       17 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/content_sub/bar/spam.txt_tmpl
+-rw-r--r--   0 rpetrello   (502) staff       (20)       15 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/content_sub/foo_tmpl
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140520 pecan-1.5.1/pecan/tests/scaffold_fixtures/file_sub/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140673 pecan-1.5.1/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/file_sub/bar_+package+/spam.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/file_sub/foo_+package+
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140831 pecan-1.5.1/pecan/tests/scaffold_fixtures/simple/
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.140978 pecan-1.5.1/pecan/tests/scaffold_fixtures/simple/bar/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/simple/bar/spam.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        4 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/scaffold_fixtures/simple/foo
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.144173 pecan-1.5.1/pecan/tests/templates/
+-rw-r--r--   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/__init__.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)      207 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_colors.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      139 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_colors_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      128 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_colors_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      143 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_login_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      116 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_login_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       75 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_name.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      147 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_name_invalid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      152 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_name_invalid_custom.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       57 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/form_name_valid.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      472 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/genshi.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      518 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/genshi_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      115 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/jinja.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      163 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/jinja_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      109 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/kajiki.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)      108 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/mako.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)       46 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/templates/mako_bad.html
+-rw-r--r--   0 rpetrello   (502) staff       (20)    73385 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_base.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1611 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_commands.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    12788 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_conf.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     2915 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_generic.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    51501 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_hooks.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     6650 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_jsonify.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    49620 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_no_thread_locals.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    44973 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_rest.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     5189 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_scaffolds.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)    17728 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_secure.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1421 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_templating.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4239 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/tests/test_util.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1498 2023-07-15 14:41:22.000000 pecan-1.5.1/pecan/util.py
+drwxr-xr-x   0 rpetrello   (502) staff       (20)        0 2023-07-15 14:48:01.128033 pecan-1.5.1/pecan.egg-info/
+-rw-r--r--   0 rpetrello   (502) staff       (20)     1303 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/PKG-INFO
+-rw-r--r--   0 rpetrello   (502) staff       (20)     4339 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/SOURCES.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/dependency_links.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)      350 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/entry_points.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        1 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/not-zip-safe
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/requires.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)        6 2023-07-15 14:48:01.000000 pecan-1.5.1/pecan.egg-info/top_level.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)       48 2023-07-15 14:41:22.000000 pecan-1.5.1/requirements.txt
+-rw-r--r--   0 rpetrello   (502) staff       (20)      209 2023-07-15 14:48:01.144696 pecan-1.5.1/setup.cfg
+-rw-r--r--   0 rpetrello   (502) staff       (20)     3190 2023-07-15 14:44:27.000000 pecan-1.5.1/setup.py
+-rw-r--r--   0 rpetrello   (502) staff       (20)       94 2023-07-15 14:41:22.000000 pecan-1.5.1/test-requirements.txt
```

### Comparing `pecan-1.5.0/LICENSE` & `pecan-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/PKG-INFO` & `pecan-1.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pecan
-Version: 1.5.0
+Version: 1.5.1
 Summary: A WSGI object-dispatching web framework, designed to be lean and fast, with few dependencies.
 Home-page: http://github.com/pecan/pecan
 Author: Jonathan LaCour
 Author-email: info@pecanpy.org
 License: BSD
 Keywords: web framework wsgi object-dispatch http
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -20,14 +19,12 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE
 License-File: AUTHORS
-
-UNKNOWN
-
```

### Comparing `pecan-1.5.0/README.rst` & `pecan-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/__init__.py` & `pecan-1.5.1/pecan/__init__.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/commands/base.py` & `pecan-1.5.1/pecan/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,17 @@
                 if isinstance(arg.get('name'), str):
                     sub.add_argument(arg.pop('name'), **arg)
                 elif isinstance(arg.get('name'), list):
                     sub.add_argument(*arg.pop('name'), **arg)
 
     def run(self, args):
         ns = self.parser.parse_args(args)
+        if ns.command_name is None:
+            self.run(['--help'])
+            return
         self.commands[ns.command_name]().run(ns)
 
     @classmethod
     def handle_command_line(cls):  # pragma: nocover
         runner = CommandRunner()
         runner.run(sys.argv[1:])
```

### Comparing `pecan-1.5.0/pecan/commands/create.py` & `pecan-1.5.1/pecan/commands/create.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/commands/serve.py` & `pecan-1.5.1/pecan/commands/serve.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/commands/shell.py` & `pecan-1.5.1/pecan/commands/shell.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/compat/__init__.py` & `pecan-1.5.1/pecan/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/configuration.py` & `pecan-1.5.1/pecan/configuration.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/core.py` & `pecan-1.5.1/pecan/core.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/decorators.py` & `pecan-1.5.1/pecan/decorators.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/extensions.py` & `pecan-1.5.1/pecan/extensions.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/hooks.py` & `pecan-1.5.1/pecan/hooks.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/jsonify.py` & `pecan-1.5.1/pecan/jsonify.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/log.py` & `pecan-1.5.1/pecan/log.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/middleware/debug.py` & `pecan-1.5.1/pecan/middleware/debug.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/middleware/errordocument.py` & `pecan-1.5.1/pecan/middleware/errordocument.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/middleware/recursive.py` & `pecan-1.5.1/pecan/middleware/recursive.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/middleware/static.py` & `pecan-1.5.1/pecan/middleware/static.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/rest.py` & `pecan-1.5.1/pecan/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
                     controller,
                     remainder[fixed_args + 1:],
                     request
                 )
 
     def _handle_unknown_method(self, method, remainder, request=None):
         '''
-        Routes undefined actions (like RESET) to the appropriate controller.
+        Routes undefined actions (like TRACE) to the appropriate controller.
         '''
         if request is None:
             self._raise_method_deprecation_warning(self._handle_unknown_method)
 
         # try finding a post_{custom} or {custom} method first
         controller = self._find_controller('post_%s' % method, method)
         if controller:
```

### Comparing `pecan-1.5.0/pecan/routing.py` & `pecan-1.5.1/pecan/routing.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/__init__.py` & `pecan-1.5.1/pecan/scaffolds/__init__.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/+package+/controllers/root.py` & `pecan-1.5.1/pecan/scaffolds/base/+package+/controllers/root.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/+package+/templates/index.html` & `pecan-1.5.1/pecan/scaffolds/base/+package+/templates/index.html`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/base/+package+/tests/__init__.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/config.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/base/+package+/tests/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/base/+package+/tests/test_functional.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/config.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/base/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/public/css/style.css` & `pecan-1.5.1/pecan/scaffolds/base/public/css/style.css`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/base/public/images/logo.png` & `pecan-1.5.1/pecan/scaffolds/base/public/images/logo.png`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/controllers/root.py` & `pecan-1.5.1/pecan/scaffolds/rest-api/+package+/controllers/root.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/__init__.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/rest-api/+package+/tests/test_functional.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/scaffolds/rest-api/config.py_tmpl` & `pecan-1.5.1/pecan/scaffolds/rest-api/config.py_tmpl`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/secure.py` & `pecan-1.5.1/pecan/secure.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/templating.py` & `pecan-1.5.1/pecan/templating.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/testing.py` & `pecan-1.5.1/pecan/testing.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/middleware/static_fixtures/self.png` & `pecan-1.5.1/pecan/tests/middleware/static_fixtures/self.png`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/middleware/test_errordocument.py` & `pecan-1.5.1/pecan/tests/middleware/test_errordocument.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/middleware/test_recursive.py` & `pecan-1.5.1/pecan/tests/middleware/test_recursive.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/middleware/test_static.py` & `pecan-1.5.1/pecan/tests/middleware/test_static.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/scaffold_builder.py` & `pecan-1.5.1/pecan/tests/scaffold_builder.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/templates/genshi_bad.html` & `pecan-1.5.1/pecan/tests/templates/genshi_bad.html`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_base.py` & `pecan-1.5.1/pecan/tests/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     pass
 
 
 class TestAppRoot(PecanTestCase):
 
     def test_controller_lookup_by_string_path(self):
         app = Pecan('pecan.tests.test_base.SampleRootController')
-        assert app.root and isinstance(app.root, SampleRootController)
+        assert app.root and app.root.__class__.__name__ == 'SampleRootController'
 
 
 class TestEmptyContent(PecanTestCase):
     @property
     def app_(self):
         class RootController(object):
             @expose()
```

### Comparing `pecan-1.5.0/pecan/tests/test_commands.py` & `pecan-1.5.1/pecan/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_conf.py` & `pecan-1.5.1/pecan/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_generic.py` & `pecan-1.5.1/pecan/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_hooks.py` & `pecan-1.5.1/pecan/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_jsonify.py` & `pecan-1.5.1/pecan/tests/test_jsonify.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                 ('id', 1),
                 ('first_name', 'Jonathan'),
                 ('last_name', 'LaCour')
             ])
         )
         self.result_proxy.append(
             FakeRowProxy([
-                ('id', 2), ('first_name', 'Yoann'), ('last_name', 'Roman')
+                ('id', 2), ('first_name', 'Ryan'), ('last_name', 'Petrello')
             ]))
         self.row_proxy = FakeRowProxy([
             ('id', 1), ('first_name', 'Jonathan'), ('last_name', 'LaCour')
         ])
 
     def create_sa_proxies(self):
```

### Comparing `pecan-1.5.0/pecan/tests/test_no_thread_locals.py` & `pecan-1.5.1/pecan/tests/test_no_thread_locals.py`

 * *Files 0% similar despite different names*

```diff
@@ -885,16 +885,16 @@
 
             @expose()
             def delete(self, req, resp, id):
                 del self.data[int(id)]
                 return 'DELETED'
 
             @expose()
-            def reset(self, req, resp):
-                return 'RESET'
+            def trace(self, req, resp):
+                return 'TRACE'
 
             @expose()
             def post_options(self, req, resp):
                 return 'OPTIONS'
 
             @expose()
             def options(self, req, resp):
@@ -963,22 +963,22 @@
 
     def test_delete_with_method_parameter_and_post(self):
         r = self.app_.post('/things/3?_method=DELETE')
         assert r.status_int == 200
         assert r.body == b'DELETED'
 
     def test_custom_method_type(self):
-        r = self.app_.request('/things', method='RESET')
+        r = self.app_.request('/things', method='TRACE')
         assert r.status_int == 200
-        assert r.body == b'RESET'
+        assert r.body == b'TRACE'
 
     def test_custom_method_type_with_method_parameter(self):
-        r = self.app_.get('/things?_method=RESET')
+        r = self.app_.get('/things?_method=TRACE')
         assert r.status_int == 200
-        assert r.body == b'RESET'
+        assert r.body == b'TRACE'
 
     def test_options(self):
         r = self.app_.request('/things', method='OPTIONS')
         assert r.status_int == 200
         assert r.body == b'OPTIONS'
 
     def test_options_with_method_parameter(self):
```

### Comparing `pecan-1.5.0/pecan/tests/test_rest.py` & `pecan-1.5.1/pecan/tests/test_rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 
             @expose()
             def delete(self, id):
                 del self.data[int(id)]
                 return 'DELETED'
 
             @expose()
-            def reset(self):
-                return 'RESET'
+            def trace(self):
+                return 'TRACE'
 
             @expose()
             def post_options(self):
                 return 'OPTIONS'
 
             @expose()
             def options(self):
@@ -190,23 +190,23 @@
         assert r.body == b'DELETED'
 
         # make sure it works
         r = app.get('/things')
         assert r.status_int == 200
         assert len(loads(r.body.decode())['items']) == 3
 
-        # test "RESET" custom action
-        r = app.request('/things', method='RESET')
+        # test "TRACE" custom action
+        r = app.request('/things', method='TRACE')
         assert r.status_int == 200
-        assert r.body == b'RESET'
+        assert r.body == b'TRACE'
 
-        # test "RESET" custom action with _method parameter
-        r = app.get('/things?_method=RESET')
+        # test "TRACE" custom action with _method parameter
+        r = app.get('/things?_method=TRACE')
         assert r.status_int == 200
-        assert r.body == b'RESET'
+        assert r.body == b'TRACE'
 
         # test the "OPTIONS" custom action
         r = app.request('/things', method='OPTIONS')
         assert r.status_int == 200
         assert r.body == b'OPTIONS'
 
         # test the "OPTIONS" custom action with the _method parameter
@@ -852,18 +852,18 @@
         r = app.get('/things/1?_method=DELETE', status=405)
         assert r.status_int == 405
 
         # test delete with _method parameter and POST
         r = app.post('/things/1?_method=DELETE', status=405)
         assert r.status_int == 405
 
-        # test "RESET" custom action
+        # test "TRACE" custom action
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
-            r = app.request('/things', method='RESET', status=405)
+            r = app.request('/things', method='TRACE', status=405)
             assert r.status_int == 405
 
     def test_nested_rest_with_missing_intermediate_id(self):
 
         class BarsController(RestController):
 
             data = [['zero-zero', 'zero-one'], ['one-zero', 'one-one']]
```

### Comparing `pecan-1.5.0/pecan/tests/test_scaffolds.py` & `pecan-1.5.1/pecan/tests/test_scaffolds.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_secure.py` & `pecan-1.5.1/pecan/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_templating.py` & `pecan-1.5.1/pecan/tests/test_templating.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/tests/test_util.py` & `pecan-1.5.1/pecan/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan/util.py` & `pecan-1.5.1/pecan/util.py`

 * *Files identical despite different names*

### Comparing `pecan-1.5.0/pecan.egg-info/PKG-INFO` & `pecan-1.5.1/pecan.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pecan
-Version: 1.5.0
+Version: 1.5.1
 Summary: A WSGI object-dispatching web framework, designed to be lean and fast, with few dependencies.
 Home-page: http://github.com/pecan/pecan
 Author: Jonathan LaCour
 Author-email: info@pecanpy.org
 License: BSD
 Keywords: web framework wsgi object-dispatch http
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: MacOS :: MacOS X
@@ -20,14 +19,12 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 License-File: LICENSE
 License-File: AUTHORS
-
-UNKNOWN
-
```

### Comparing `pecan-1.5.0/pecan.egg-info/SOURCES.txt` & `pecan-1.5.1/pecan.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 test-requirements.txt
-bin/pecan
 pecan/__init__.py
 pecan/configuration.py
 pecan/core.py
 pecan/decorators.py
 pecan/deploy.py
 pecan/extensions.py
 pecan/hooks.py
```

### Comparing `pecan-1.5.0/setup.py` & `pecan-1.5.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import platform
 
 from setuptools import setup, find_packages
 
-version = '1.5.0'
+version = '1.5.1'
 
 #
 # determine requirements
 #
 with open('requirements.txt') as reqs:
     requirements = [
         line for line in reqs.read().split('\n')
@@ -68,25 +68,25 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: WSGI',
         'Topic :: Software Development :: Libraries :: Application Frameworks'
     ],
     keywords='web framework wsgi object-dispatch http',
     author='Jonathan LaCour',
     author_email='info@pecanpy.org',
     url='http://github.com/pecan/pecan',
     license='BSD',
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests']),
     include_package_data=True,
-    scripts=['bin/pecan'],
     zip_safe=False,
     install_requires=requirements,
     tests_require=tests_require,
     test_suite='pecan',
     entry_points="""
     [pecan.command]
     serve = pecan.commands:ServeCommand
```

