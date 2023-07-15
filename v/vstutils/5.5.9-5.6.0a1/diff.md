# Comparing `tmp/vstutils-5.5.9.tar.gz` & `tmp/vstutils-5.6.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.5.9.tar", last modified: Wed Jun 28 03:53:22 2023, max compression
+gzip compressed data, was "vstutils-5.6.0a1.tar", last modified: Sat Jul 15 01:14:31 2023, max compression
```

## Comparing `vstutils-5.5.9.tar` & `vstutils-5.6.0a1.tar`

### file list

```diff
@@ -1,253 +1,254 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.022120 vstutils-5.5.9/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.5.9/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.5.9/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.5.9/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-28 03:53:22.022120 vstutils-5.5.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:27.000000 vstutils-5.5.9/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:31:00.000000 vstutils-5.5.9/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.5.9/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.5.9/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.5.9/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:01.000000 vstutils-5.5.9/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:06.000000 vstutils-5.5.9/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-14 22:04:13.000000 vstutils-5.5.9/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      506 2023-06-28 03:44:06.000000 vstutils-5.5.9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-28 03:53:22.022120 vstutils-5.5.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.5.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.954120 vstutils-5.5.9/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-28 03:44:06.000000 vstutils-5.5.9/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.966120 vstutils-5.5.9/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:54.000000 vstutils-5.5.9/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:43.000000 vstutils-5.5.9/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:43.000000 vstutils-5.5.9/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:13.000000 vstutils-5.5.9/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:17:53.000000 vstutils-5.5.9/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:54.000000 vstutils-5.5.9/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.970120 vstutils-5.5.9/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.970120 vstutils-5.5.9/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    28314 2023-06-22 02:12:27.000000 vstutils-5.5.9/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:13.000000 vstutils-5.5.9/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:17:53.000000 vstutils-5.5.9/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:54.000000 vstutils-5.5.9/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3544 2023-06-28 03:44:06.000000 vstutils-5.5.9/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:06.000000 vstutils-5.5.9/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:04.000000 vstutils-5.5.9/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.938120 vstutils-5.5.9/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.970120 vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.970120 vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.974120 vstutils-5.5.9/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.5.9/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.974120 vstutils-5.5.9/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.974120 vstutils-5.5.9/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:54.000000 vstutils-5.5.9/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.5.9/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.5.9/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:28.000000 vstutils-5.5.9/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.978120 vstutils-5.5.9/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:54.000000 vstutils-5.5.9/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2023-06-24 04:44:36.000000 vstutils-5.5.9/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:54.000000 vstutils-5.5.9/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:54.000000 vstutils-5.5.9/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:17:53.000000 vstutils-5.5.9/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55979 2023-06-27 04:42:54.000000 vstutils-5.5.9/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:31:00.000000 vstutils-5.5.9/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.942119 vstutils-5.5.9/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.994120 vstutils-5.5.9/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126387 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38355 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    73740 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536116 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    87131 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355745 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1032776 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/957.js
--rw-r--r--   0 root         (0) root         (0)     2030 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/957.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    81737 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303699 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3621 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   435785 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.994120 vstutils-5.5.9/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.994120 vstutils-5.5.9/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:17:53.000000 vstutils-5.5.9/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.998120 vstutils-5.5.9/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.5.9/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.5.9/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.5.9/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.5.9/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.002120 vstutils-5.5.9/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.5.9/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.5.9/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.002120 vstutils-5.5.9/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.002120 vstutils-5.5.9/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.5.9/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.006120 vstutils-5.5.9/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.010120 vstutils-5.5.9/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.014120 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.014120 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.014120 vstutils-5.5.9/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.014120 vstutils-5.5.9/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.5.9/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.018120 vstutils-5.5.9/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.5.9/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.018120 vstutils-5.5.9/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.022120 vstutils-5.5.9/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.022120 vstutils-5.5.9/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.022120 vstutils-5.5.9/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.5.9/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:22.022120 vstutils-5.5.9/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.5.9/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.5.9/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.5.9/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.9/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-14 22:04:13.000000 vstutils-5.5.9/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.5.9/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.5.9/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 03:53:21.954120 vstutils-5.5.9/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4427 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7664 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 03:53:21.000000 vstutils-5.5.9/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4429 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2389 2023-06-22 02:12:26.000000 vstutils-5.6.0a1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-30 04:31:11.000000 vstutils-5.6.0a1/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-30 04:31:11.000000 vstutils-5.6.0a1/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-30 04:31:11.000000 vstutils-5.6.0a1/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-06-28 03:44:04.000000 vstutils-5.6.0a1/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-07-15 01:14:31.963730 vstutils-5.6.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16558 2023-06-21 00:04:50.000000 vstutils-5.6.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.911730 vstutils-5.6.0a1/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-15 01:09:51.000000 vstutils-5.6.0a1/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.919730 vstutils-5.6.0a1/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:52.000000 vstutils-5.6.0a1/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29458 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:42.000000 vstutils-5.6.0a1/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:42.000000 vstutils-5.6.0a1/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13794 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.6.0a1/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3234 2023-06-27 04:42:52.000000 vstutils-5.6.0a1/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.923730 vstutils-5.6.0a1/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.923730 vstutils-5.6.0a1/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1911 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    29661 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:14:38.000000 vstutils-5.6.0a1/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5667 2023-06-27 04:42:52.000000 vstutils-5.6.0a1/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3554 2023-06-30 04:31:11.000000 vstutils-5.6.0a1/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-06-28 03:44:04.000000 vstutils-5.6.0a1/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:03.000000 vstutils-5.6.0a1/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.899730 vstutils-5.6.0a1/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.923730 vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.923730 vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.927730 vstutils-5.6.0a1/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3487 2023-06-23 05:26:08.000000 vstutils-5.6.0a1/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.927730 vstutils-5.6.0a1/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.927730 vstutils-5.6.0a1/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2023-06-27 04:42:52.000000 vstutils-5.6.0a1/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     3661 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/vstutils/management/commands/rpc_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10594 2023-06-30 04:31:11.000000 vstutils-5.6.0a1/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.931730 vstutils-5.6.0a1/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:53.000000 vstutils-5.6.0a1/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25952 2023-07-14 05:18:36.000000 vstutils-5.6.0a1/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:53.000000 vstutils-5.6.0a1/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:53.000000 vstutils-5.6.0a1/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:14:38.000000 vstutils-5.6.0a1/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55656 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:57.000000 vstutils-5.6.0a1/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.899730 vstutils-5.6.0a1/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.943730 vstutils-5.6.0a1/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126387 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      170 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38355 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    73740 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536116 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    87131 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      218 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355745 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1032776 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/957.js
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/957.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    81737 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303699 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   439098 2023-07-15 01:14:30.000000 vstutils-5.6.0a1/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5092 2023-07-14 07:52:41.000000 vstutils-5.6.0a1/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.6.0a1/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.947730 vstutils-5.6.0a1/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.951730 vstutils-5.6.0a1/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.951730 vstutils-5.6.0a1/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.955730 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.955730 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.955730 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.955730 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:20.000000 vstutils-5.6.0a1/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18312 2023-07-08 04:27:47.000000 vstutils-5.6.0a1/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.959730 vstutils-5.6.0a1/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16335 2023-07-14 05:18:36.000000 vstutils-5.6.0a1/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    24130 2023-07-14 05:18:36.000000 vstutils-5.6.0a1/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    19158 2023-07-14 05:18:36.000000 vstutils-5.6.0a1/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.6.0a1/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-15 03:16:12.000000 vstutils-5.6.0a1/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      979 2023-06-21 03:04:37.000000 vstutils-5.6.0a1/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:37:08.000000 vstutils-5.6.0a1/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 01:14:31.915730 vstutils-5.6.0a1/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4429 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7707 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1835 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 01:14:31.000000 vstutils-5.6.0a1/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.5.9/LICENSE` & `vstutils-5.6.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/MANIFEST.in` & `vstutils-5.6.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/NOTICE` & `vstutils-5.6.0a1/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/PKG-INFO` & `vstutils-5.6.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.9
+Version: 5.6.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.9/README.rst` & `vstutils-5.6.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/setup.cfg` & `vstutils-5.6.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/setup.py` & `vstutils-5.6.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/actions.py` & `vstutils-5.6.0a1/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/admin.py` & `vstutils-5.6.0a1/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/auth.py` & `vstutils-5.6.0a1/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/base.py` & `vstutils-5.6.0a1/vstutils/api/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,21 +510,24 @@
             f'_'
             f'{request.COOKIES.get(settings.LANGUAGE_COOKIE_NAME, settings.LANGUAGE_CODE)}'
         )
 
     def _get_etag(self, model_class, request):
         return f'"{self.get_etag_value(model_class, request)}"'
 
+    def should_check_action(self, method):
+        return method in getattr(self, 'etag_match_methods', {method})
+
     def check_etag(self, request, model_class=None):
         should_check, header_name, exception, operation_handler = False, "", Exception(), str.__eq__
         if request.method in {"GET", "HEAD"}:
             should_check = True
             exception = self.NotModifiedException("")
             header_name = "If-None-Match"
-        elif request.method in getattr(self, 'etag_match_methods', {request.method}):
+        elif self.should_check_action(request.method):
             should_check = True
             exception = self.PreconditionFailedException("")
             header_name = "If-Match"
             operation_handler = str.__ne__
 
         if not should_check:
             # For non-standart request methods
```

### Comparing `vstutils-5.5.9/vstutils/api/decorators.py` & `vstutils-5.6.0a1/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/decorators.pyi` & `vstutils-5.6.0a1/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/doc_generator.py` & `vstutils-5.6.0a1/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/endpoint.py` & `vstutils-5.6.0a1/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/fields.py` & `vstutils-5.6.0a1/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/filter_backends.py` & `vstutils-5.6.0a1/vstutils/api/filter_backends.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
                 'in': openapi.IN_QUERY,
                 'description': force_str(self.ordering_description),
                 'minItems': 1,
                 'uniqueItems': True,
                 'collectionFormat': 'csv',
                 'schema': {
                     'type': openapi.TYPE_ARRAY,
-                    'title': _(force_str(self.ordering_title)),
+                    'x-title': _(force_str(self.ordering_title)),
                     'items': {
                         'type': openapi.TYPE_STRING,
                         'format': 'ordering_choices',
                         'enum': tuple(self._get_fields_for_schema(view)),
                     },
                 },
             },
```

### Comparing `vstutils-5.5.9/vstutils/api/filters.py` & `vstutils-5.6.0a1/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/health.py` & `vstutils-5.6.0a1/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/meta.py` & `vstutils-5.6.0a1/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/metrics.py` & `vstutils-5.6.0a1/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0001_initial.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.6.0a1/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/models.py` & `vstutils-5.6.0a1/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/parsers.py` & `vstutils-5.6.0a1/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/permissions.py` & `vstutils-5.6.0a1/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/renderers.py` & `vstutils-5.6.0a1/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/responses.py` & `vstutils-5.6.0a1/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/responses.pyi` & `vstutils-5.6.0a1/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/routers.py` & `vstutils-5.6.0a1/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/routers.pyi` & `vstutils-5.6.0a1/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/schema/generators.py` & `vstutils-5.6.0a1/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/schema/info.py` & `vstutils-5.6.0a1/vstutils/api/schema/info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 # pylint: disable=import-error
 from collections import OrderedDict
 
 import django
 from django.conf import settings
 from django.urls import reverse_lazy
 from rest_framework import __version__ as drf_version  # type: ignore
+from fastapi import __version__ as fastapi_version  # type: ignore
 from drf_yasg import openapi, __version__ as drf_yasg_version  # type: ignore
+try:
+    import celery
+except ImportError:  # nocv
+    celery = None
 
 from ... import __version__ as vstutils_version
 
 
 x_versions = OrderedDict()  # type: OrderedDict
 x_versions['application'] = settings.PROJECT_VERSION
 x_versions['library'] = settings.PROJECT_LIB_VERSION
 x_versions['vstutils'] = vstutils_version
 x_versions['django'] = django.__version__
 x_versions['djangorestframework'] = drf_version
 x_versions['drf_yasg'] = drf_yasg_version
+x_versions['fastapi'] = fastapi_version
+
+if celery is not None:
+    x_versions['celery'] = celery.__version__  # type: ignore
 
 api_info_dict = OrderedDict(
     title=settings.PROJECT_GUI_NAME,
     default_version=settings.VST_API_VERSION,
     description=settings.SWAGGER_API_DESCRIPTION,
     terms_of_service=settings.TERMS_URL,
     contact=openapi.Contact(**settings.CONTACT),
```

### Comparing `vstutils-5.5.9/vstutils/api/schema/inspectors.py` & `vstutils-5.6.0a1/vstutils/api/schema/inspectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.http import FileResponse
 from django.db import models
 from django.utils.functional import cached_property
 from drf_yasg.inspectors.base import FieldInspector, FilterInspector, NotHandled
 from drf_yasg.inspectors.field import ReferencingSerializerInspector, decimal_field_type
 from drf_yasg import openapi
 from drf_yasg.inspectors.query import CoreAPICompatInspector, force_real_str, coreschema  # type: ignore
+from rest_framework.pagination import BasePagination
 from rest_framework.fields import Field, JSONField, DecimalField, ListField, empty
 from rest_framework.serializers import Serializer
 
 from .. import fields, serializers, validators
 from ...models.base import get_first_match_name
 from ...utils import raise_context_decorator_with_default
 
@@ -567,15 +568,38 @@
             stacklevel=2,
         )
         return {
             f.name: f
             for f in self.view.get_queryset().model._meta.fields
         }
 
+    def build_paginated_property(self, value: dict):
+        # Need to remove useless params from schema
+        value.pop('example', None)
+        if 'nullable' in value:
+            value['x-nullable'] = value.pop('nullable')
+        return openapi.Schema(**value)
+
+    def get_paginated_response(self, paginator: BasePagination, response_schema: Any):
+        try:
+            paginator_schema = paginator.get_paginated_response_schema(response_schema)
+            properties = {
+                k: self.build_paginated_property(v)
+                for k, v in paginator_schema.pop('properties').items()
+            }
+            return openapi.Schema(
+                **paginator_schema,
+                properties=properties
+            )
+        except:  # nocv
+            return NotHandled
+
     def param_to_schema(self, param):
+        if 'title' in param:
+            param['x-title'] = param.pop('title')  # nocv
         return openapi.Parameter(
             name=param['name'],
             in_=param['in'],
             description=param.get('description'),
             required=param.get('required', False),
             **param['schema'],
         )
@@ -729,14 +753,22 @@
             schema['x-translate-model'] = translate_model
 
         if hide_not_required:
             schema['x-hide-not-required'] = bool(hide_not_required)
 
         schema._handled = True  # pylint: disable=protected-access
 
+        # TODO: return it when swagger become openapi 3.0.1
+        # if isinstance(field, ModelSerializer) \
+        #         and hasattr(field, 'Meta') \
+        #         and hasattr(field.Meta, 'model') \
+        #         and field.Meta.model._meta.pk.name in schema_properties:
+        #     schema.setdefault('required', [])
+        #     schema['required'].insert(0, field.Meta.model._meta.pk.name)
+
     def field_to_swagger_object(self, field: Any, swagger_object_type: Any, use_references: Any, **kwargs: Any):
         if isinstance(field, FileResponse):
             return openapi.Schema(type='file')
 
         result = super().field_to_swagger_object(field, swagger_object_type, use_references, **kwargs)
 
         if result != NotHandled:
```

### Comparing `vstutils-5.5.9/vstutils/api/schema/schema.py` & `vstutils-5.6.0a1/vstutils/api/schema/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,24 +2,68 @@
 from copy import copy
 from warnings import warn
 
 from django.http import FileResponse
 from rest_framework import status
 from drf_yasg.inspectors.view import SwaggerAutoSchema
 from drf_yasg.app_settings import swagger_settings
-from drf_yasg.openapi import Operation
+from drf_yasg.openapi import Schema, Response, Operation, Parameter, IN_HEADER, TYPE_STRING
 
 from ... import utils
 from ...models.base import get_proxy_labels
 from ..decorators import NestedWithAppendMixin
-from ..base import detail_actions
+from ..base import detail_actions, CachableHeadMixin
 from . import inspectors as vst_inspectors
 
 
-class VSTAutoSchema(SwaggerAutoSchema):
+class ExtendedSwaggerAutoSchema(SwaggerAutoSchema):
+    def get_query_parameters(self):
+        result = super().get_query_parameters()
+        if isinstance(self.view, CachableHeadMixin):
+            if self.method == 'GET':
+                result += [
+                    Parameter(
+                        name='If-None-Match',
+                        in_=IN_HEADER,
+                        required=False,
+                        type=TYPE_STRING,
+                    )
+                ]
+
+            elif self.view.should_check_action(self.method):
+                result += [
+                    Parameter(
+                        name='If-Match',
+                        in_=IN_HEADER,
+                        required=False,
+                        type=TYPE_STRING,
+                    )
+                ]
+
+        return result
+
+    def get_response_schemas(self, response_serializers):
+        responses = super().get_response_schemas(response_serializers)
+        if isinstance(self.view, CachableHeadMixin) and self.view.is_main_action:
+            for response in responses:
+                if response.startswith('2') or response == 'default':
+                    responses[response]['headers'] = responses[response].get('headers', {})
+                    responses[response]['headers'].setdefault(
+                        'Etag', Schema(type=TYPE_STRING)
+                    )
+            if self.method == 'GET' and (st := str(self.view.NotModifiedException.status_code)) not in responses:
+                responses[st] = Response(description="Not Modified")
+            elif self.view.should_check_action(self.method):
+                responses[str(self.view.PreconditionFailedException.status_code)] = Response(
+                    description="Precondition Failed"
+                )
+        return responses
+
+
+class VSTAutoSchema(ExtendedSwaggerAutoSchema):
     paginator_inspectors = [
         vst_inspectors.ArrayFilterQueryInspector,
     ] + swagger_settings.DEFAULT_PAGINATOR_INSPECTORS
     field_inspectors = [
         vst_inspectors.CommaMultiSelectFieldInspector,
         vst_inspectors.FkFieldInspector,
         vst_inspectors.DynamicJsonTypeFieldInspector,
```

### Comparing `vstutils-5.5.9/vstutils/api/serializers.py` & `vstutils-5.6.0a1/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/throttling.py` & `vstutils-5.6.0a1/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/validators.py` & `vstutils-5.6.0a1/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/api/views.py` & `vstutils-5.6.0a1/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/asgi.py` & `vstutils-5.6.0a1/vstutils/asgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     @application.get(f'/{settings.API_URL}/live/')
     async def api_live_check():
         return ORJSONResponse({"status": "ok"})
 
 
 @application.middleware('http')
 async def add_server_timing_header(request: Request, call_next):
-    start_time = time.time()
+    start_time = time.monotonic()
     response = await call_next(request)
-    response.headers['Server-Timing'] = f'total;dur={round((time.time()-start_time)*1000, 2)}'
+    response.headers['Server-Timing'] = f'total;dur={round((time.monotonic()-start_time)*1000, 2)}'
     return response
 
 
 if not any(m.path == '/' for m in application.routes):
     application.mount("/", ASGIHandler())
```

### Comparing `vstutils-5.5.9/vstutils/asgi_worker.py` & `vstutils-5.6.0a1/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/auth.py` & `vstutils-5.6.0a1/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/auth.pyi` & `vstutils-5.6.0a1/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/celery_beat_scheduler.py` & `vstutils-5.6.0a1/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.6.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/environment.py` & `vstutils-5.6.0a1/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/exceptions.py` & `vstutils-5.6.0a1/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/gui/context.py` & `vstutils-5.6.0a1/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/gui/forms.py` & `vstutils-5.6.0a1/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/gui/pwa_manifest.py` & `vstutils-5.6.0a1/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/gui/views.py` & `vstutils-5.6.0a1/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/ldap_utils.py` & `vstutils-5.6.0a1/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/_base.py` & `vstutils-5.6.0a1/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/celery_inspect.py` & `vstutils-5.6.0a1/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/dockerrun.py` & `vstutils-5.6.0a1/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/newproject.py` & `vstutils-5.6.0a1/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/run_task.py` & `vstutils-5.6.0a1/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/runrpc.py` & `vstutils-5.6.0a1/vstutils/management/commands/runrpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import sys
-from subprocess import check_call
+import warnings
+
+from django.core.management import call_command
 
 from ._base import DockerCommand
-from .web import get_celery_command
 
 
 class Command(DockerCommand):
     help = "Run Celery for web-application"
 
     def add_arguments(self, parser):
         super().add_arguments(parser)
@@ -18,26 +18,17 @@
         parser.add_argument(
             '--nomigrate',
             action='store_false', dest='migrate', default=True,
             help="Do NOT run docker command for migration of databases.",
         )
 
     def handle(self, *args, **opts):
+        warnings.warn('This command is deprecated and will removed in 6.x releases. Use "run_worker" instead.',
+                      category=DeprecationWarning,
+                      stacklevel=2)
         super().handle(*args, **opts)
 
-        if opts['migrate']:
-            self.migrate(opts)  # nocv
-
         cmd_args = dict(
             arg.split('=')
             for arg in args
         )
-
-        cmd = f'{sys.executable} -m {get_celery_command(**cmd_args)}'
-        self._print(f'Execute: {cmd}')
-        sys.exit(check_call(
-            cmd,
-            stdout=sys.stdout,
-            stderr=sys.stderr,
-            stdin=sys.stdin,
-            shell=True,  # nosec
-        ))
+        call_command('rpc_worker', migrate=opts['migrate'], **cmd_args)
```

### Comparing `vstutils-5.5.9/vstutils/management/commands/runserver.py` & `vstutils-5.6.0a1/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/management/commands/web.py` & `vstutils-5.6.0a1/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/middleware.py` & `vstutils-5.6.0a1/vstutils/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 class QueryTimingLogger:
     __slots__ = ('queries_time',)
 
     def __init__(self):
         self.queries_time = 0
 
     def __call__(self, execute, sql, params, many, context):
-        start = time.time()
+        start = time.monotonic()
         try:
             return execute(sql, params, many, context)
         finally:
-            self.queries_time += time.time() - start
+            self.queries_time += time.monotonic() - start
 
 
 class BaseMiddleware(BaseVstObject):
     """
     Middleware base class for handling:
 
     * Incoming requests by :meth:`.BaseMiddleware.request_handler()`;
@@ -271,20 +271,22 @@
     def get_response_handler(self, request: HttpRequest) -> ResponseHandlerType:
         if request.user.need_twofa and self.check_url_name(request):  # type: ignore
             return redirect(self.redirect_name)
         return super().get_response_handler(request)
 
 
 class FrontendChangesNotifications(BaseMiddleware):
-    __slots__ = ('notificator_class',)
+    __slots__ = ('notificator',)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.notificator_class = apps.get_app_config('vstutils_api').module.notificator_class
+        self.notificator = apps.get_app_config('vstutils_api').module.notificator_class([])
 
-    def get_response_handler(self, request: HttpRequest) -> ResponseHandlerType:
-        # pylint: disable=invalid-overridden-method
-        if settings.CENTRIFUGO_CLIENT_KWARGS and request.path != f'/{settings.API_URL}/health/':
-            with self.notificator_class([]) as notificator:
-                request.notificator = notificator  # type: ignore
-                return super().get_response_handler(request)
-        return super().get_response_handler(request)
+    def request_handler(self, request: HttpRequest) -> HttpRequest:
+        if self.notificator.is_usable():
+            request.notificator = self.notificator
+        return request
+
+    def handler(self, request: HttpRequest, response: HttpResponse) -> HttpResponse:
+        if self.notificator.is_usable():
+            request.notificator.send()
+        return response
```

### Comparing `vstutils-5.5.9/vstutils/models/__init__.py` & `vstutils-5.6.0a1/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/models/base.py` & `vstutils-5.6.0a1/vstutils/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,31 +267,31 @@
                 receiver(post_save, sender=label)(update_cache_for_model_related)
                 receiver(post_delete, sender=label)(update_cache_for_model_related)
         return model_class
 
     def get_proxy_labels(cls):
         return get_proxy_labels(cls)  # nocv
 
-    def get_api_cache_name(cls, pk=None):
-        return f'api_caching_table_{cls._meta.db_table}' + (f'_{pk}' if pk is not None else "")
+    def get_api_cache_name(cls, postfix=None):
+        if postfix not in {None, '__postfix__'}:
+            postfix = f'{cls.get_etag_value("__postfix__")}_{postfix}'
+        return f'etag_table_{cls._meta.db_table}' + (f'_{postfix}' if postfix is not None else "")
 
     def get_etag_value(cls, pk=None):
         # pylint: disable=no-value-for-parameter
-        if pk and django_caches['etag'].get(f'clear_{cls.get_api_cache_name()}') == 1:
-            return cls.set_etag_value(pk)
         return str(django_caches['etag'].get_or_set(cls.get_api_cache_name(pk), str(uuid.uuid4())))
 
     def set_etag_value(cls, pk=None):
         # pylint: disable=no-value-for-parameter
         new_value = str(uuid.uuid4())
         django_caches['etag'].set(cls.get_api_cache_name(), new_value)
         if pk:
             django_caches['etag'].set(cls.get_api_cache_name(pk), new_value)
         else:
-            django_caches['etag'].set(f'clear_{cls.get_api_cache_name()}', 1)
+            django_caches['etag'].set(cls.get_api_cache_name("__postfix__"), new_value)
         return new_value
 
     @classproperty
     @lru_cache()
     def generated_view(cls):
         # pylint: disable=no-value-for-parameter
         return cls.get_view_class()
```

### Comparing `vstutils-5.5.9/vstutils/models/cent_notify.py` & `vstutils-5.6.0a1/vstutils/models/cent_notify.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 class JsonEncoder(json.JSONEncoder):
     def default(self, o):
         return str(o)  # nocv
 
 
 class Notificator:
+    __slots__ = ('queue', 'cent_client', 'label', '_signals', '__weakref__')
     client_class = CentrifugoClient
 
     queue: _t.List[_t.Tuple[_t.Sequence[_t.Text], _t.Any]]
     cent_client: CentrifugoClient
     label: _t.Text
 
     _json_renderer = ORJSONRenderer()
@@ -121,8 +122,7 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.is_usable():
             self.send()
-            self.disconnect_all()
```

### Comparing `vstutils-5.5.9/vstutils/models/custom_model.py` & `vstutils-5.6.0a1/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/models/custom_model.pyi` & `vstutils-5.6.0a1/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/models/decorators.py` & `vstutils-5.6.0a1/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/models/fields.py` & `vstutils-5.6.0a1/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/models/queryset.py` & `vstutils-5.6.0a1/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/settings.ini` & `vstutils-5.6.0a1/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/settings.py` & `vstutils-5.6.0a1/vstutils/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1061,28 +1061,22 @@
 # Rest Api settings
 # http://www.django-rest-framework.org/api-guide/settings/
 ##############################################################
 PAGE_LIMIT: int = web["page_limit"]
 REST_FRAMEWORK: _t.Dict = {
     'DEFAULT_AUTHENTICATION_CLASSES': (
         'rest_framework.authentication.SessionAuthentication',
-        'rest_framework.authentication.BasicAuthentication',
-        'rest_framework.authentication.TokenAuthentication',
     ),
     'DEFAULT_RENDERER_CLASSES': (
         "vstutils.api.renderers.ORJSONRenderer",
         "vstutils.api.renderers.MsgpackRenderer",
-        'rest_framework.renderers.BrowsableAPIRenderer',
-        'rest_framework.renderers.MultiPartRenderer',
     ),
     'DEFAULT_PARSER_CLASSES': (
         "drf_orjson_renderer.parsers.ORJSONParser",
         "vstutils.api.parsers.MsgpackParser",
-        'rest_framework.parsers.FormParser',
-        'rest_framework.parsers.MultiPartParser'
     ),
     'DEFAULT_PERMISSION_CLASSES': [
         'vstutils.api.permissions.IsAuthenticatedOpenApiRequest'
     ],
     "ORJSON_RENDERER_OPTIONS": (
         orjson.OPT_NON_STR_KEYS,
         orjson.OPT_SERIALIZE_DATACLASS,
@@ -1420,15 +1414,15 @@
 # Centrifugo settings
 CENTRIFUGO_CLIENT_KWARGS = config['centrifugo'].all()
 CENTRIFUGO_PUBLIC_HOST = CENTRIFUGO_CLIENT_KWARGS.pop('public_address', None) or CENTRIFUGO_CLIENT_KWARGS.get('address')
 NOTIFICATOR_CLIENT_CLASS = web.get(
     'notificator_client_class',
     fallback='vstutils.models.cent_notify.Notificator'
 )
-SUBSCRIPTIONS_PREFIX = CENTRIFUGO_CLIENT_KWARGS.pop('subscriptions_prefix', f'{VST_PROJECT}.update')
+SUBSCRIPTIONS_PREFIX = CENTRIFUGO_CLIENT_KWARGS.pop('subscriptions_prefix', f'{VST_PROJECT_LIB}.update')
 
 THROTTLE = config['throttle'].all()
 
 
 # Storage settings
 def get_default_storage_class():
     if LIBCLOUD_PROVIDERS.get('default'):
```

### Comparing `vstutils-5.5.9/vstutils/static/bundle/281.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/296.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/345.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/368.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/421.js` & `vstutils-5.6.0a1/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.6.0a1/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/618.js` & `vstutils-5.6.0a1/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/683.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/686.js` & `vstutils-5.6.0a1/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/742.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.6.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/755.js` & `vstutils-5.6.0a1/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/826.chunk.js` & `vstutils-5.6.0a1/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.6.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/844.js` & `vstutils-5.6.0a1/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/957.js` & `vstutils-5.6.0a1/vstutils/static/bundle/957.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/957.js.LICENSE.txt` & `vstutils-5.6.0a1/vstutils/static/bundle/957.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/app_loader.js` & `vstutils-5.6.0a1/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/base.js` & `vstutils-5.6.0a1/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.6.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.6.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/output.json` & `vstutils-5.6.0a1/vstutils/static/bundle/output.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964192708333334%*

 * *Differences: {"'entrypoints'": "{'spa': {'assets': {0: {'size': 439098}}, 'assetsSize': 2919268}}"}*

```diff
@@ -26,15 +26,15 @@
             "filteredAuxiliaryAssets": 0,
             "name": "base"
         },
         "spa": {
             "assets": [
                 {
                     "name": "vstutils.js",
-                    "size": 435785
+                    "size": 439098
                 },
                 {
                     "name": "755.js",
                     "size": 87131
                 },
                 {
                     "name": "421.js",
@@ -57,15 +57,15 @@
                     "size": 1032776
                 },
                 {
                     "name": "spa.js",
                     "size": 3621
                 }
             ],
-            "assetsSize": 2915955,
+            "assetsSize": 2919268,
             "auxiliaryAssetsSize": 117924,
             "filteredAssets": 0,
             "filteredAuxiliaryAssets": 2,
             "name": "spa"
         }
     },
     "errors": []
```

### Comparing `vstutils-5.5.9/vstutils/static/bundle/spa.js` & `vstutils-5.6.0a1/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static/bundle/vstutils.js` & `vstutils-5.6.0a1/vstutils/static/bundle/vstutils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -806,15 +806,15 @@
                         }
                     }
                 },
                 B = n(45393),
                 N = {};
             N.styleTagTransform = g(), N.setAttributes = f(), N.insert = c().bind(null, "head"), N.domAPI = u(), N.insertStyleElement = m(), o()(B.Z, N), B.Z && B.Z.locals && B.Z.locals;
             var D = (0, y.Z)(O, V, [], !1, null, "39bac637", null).exports,
-                L = function() {
+                j = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("div", {
                         staticClass: "sidebar"
                     }, [t("nav", {
                         staticClass: "mt-2"
@@ -827,16 +827,16 @@
                         }
                     }, e._l(e.menu, (function(i, s) {
                         return t(n.SidebarItem, e._b({
                             key: s
                         }, "SidebarItem", i, !1))
                     })), 1), e._v(" "), e._t("bottom")], 2)])
                 };
-            L._withStripped = !0;
-            var j = n(70538),
+            j._withStripped = !0;
+            var L = n(70538),
                 q = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("li", {
                         staticClass: "nav-item",
                         class: {
@@ -898,15 +898,15 @@
                             on: {
                                 open: n.onOpen
                             }
                         }, "SidebarItem", i, !1))
                     })), 1) : e._e()], 1)
                 };
             q._withStripped = !0;
-            var $ = (0, j.defineComponent)({
+            var $ = (0, L.defineComponent)({
                     __name: "SidebarItem",
                     props: {
                         name: null,
                         to: null,
                         href: null,
                         sublinks: null,
                         icon: null,
@@ -915,20 +915,20 @@
                     emits: ["open"],
                     setup(e, t) {
                         let {
                             emit: n
                         } = t;
                         const i = e,
                             s = (0, Z.getApp)(),
-                            a = (0, j.computed)((() => {
+                            a = (0, L.computed)((() => {
                                 var e;
                                 return ((null === (e = i.sublinks) || void 0 === e ? void 0 : e.length) || 0) > 0
                             })),
-                            r = (0, j.ref)(!1);
-                        return (0, j.onMounted)((() => {
+                            r = (0, L.ref)(!1);
+                        return (0, L.onMounted)((() => {
                             if (i.to) {
                                 const e = s.router;
                                 e.resolve(i.to).route.fullPath === e.currentRoute.fullPath && n("open")
                             }
                         })), {
                             __sfc: !0,
                             props: i,
@@ -947,33 +947,33 @@
                                     action: i.emptyAction
                                 })
                             }
                         }
                     }
                 }),
                 U = (0, y.Z)($, q, [], !1, null, null, null).exports,
-                H = (0, j.defineComponent)({
+                H = (0, L.defineComponent)({
                     __name: "Sidebar",
                     props: {
                         menu: null
                     },
                     setup(e) {
-                        return (0, j.onMounted)((() => {
+                        return (0, L.onMounted)((() => {
                             "ontouchstart" in window && S("body").swipe({
                                 swipe: (e, t) => ("right" === t ? M() : "left" === t && I(), !0),
                                 threshold: 150,
                                 preventDefaultEvents: !1
                             })
                         })), {
                             __sfc: !0,
                             SidebarItem: U
                         }
                     }
                 }),
-                G = (0, y.Z)(H, L, [], !1, null, null, null).exports,
+                G = (0, y.Z)(H, j, [], !1, null, null, null).exports,
                 z = n(84160),
                 W = n(60751)
         },
         28445: function(e, t, n) {
             n.d(t, {
                 B: function() {
                     return l
@@ -1093,15 +1093,15 @@
                 ModelFields: function() {
                     return s.Z
                 },
                 OneEntity: function() {
                     return i.Z
                 }
             });
-            var i = n(89045),
+            var i = n(68217),
                 s = n(13034)
         },
         14514: function(e, t) {
             const n = {
                 name: "FieldLabelIdMixin",
                 props: ["field", "wrapper_opt", "value", "data"],
                 computed: {
@@ -1231,15 +1231,15 @@
                 rating: function() {
                     return i
                 }
             });
             var i = {};
             n.r(i), n.d(i, {
                 RatingField: function() {
-                    return j
+                    return L
                 }
             });
             var s = n(66044),
                 a = n(87444),
                 r = n(93378);
             class o extends r.Ki {}
             var l = function() {
@@ -1454,15 +1454,15 @@
                             },
                             on: {
                                 change: e => this.$emit("set-value", e)
                             }
                         })
                     }
                 },
-                L = {
+                j = {
                     components: {
                         field_content_readonly: D,
                         field_content_edit: {
                             mixins: [D],
                             data: () => ({
                                 edit: !0
                             })
@@ -1472,20 +1472,20 @@
                     mixins: [a.BaseFieldMixin],
                     methods: {
                         setValue(e) {
                             this.field.nullable && e === this.value && (e = null), this._emitSetValueSignal(e)
                         }
                     }
                 };
-            class j extends o {
+            class L extends o {
                 constructor(e) {
                     super(e), this.min = this.props.min_value, this.max = this.props.max_value, this.step = this.props.step, this.style = this.props.style, this.color = this.props.color || "#ffb100", this.faClass = this.props.fa_class
                 }
                 static get mixins() {
-                    return [L]
+                    return [j]
                 }
                 getEmptyValue() {
                     return this.nullable ? null : this.min
                 }
             }
             var q = n(33364);
             const $ = {
@@ -2170,15 +2170,15 @@
                 le: function() {
                     return z
                 },
                 zr: function() {
                     return A
                 },
                 cO: function() {
-                    return j
+                    return L
                 },
                 t$: function() {
                     return E
                 },
                 pi: function() {
                     return _
                 },
@@ -2197,15 +2197,15 @@
                 vQ: function() {
                     return D
                 },
                 vZ: function() {
                     return w
                 },
                 lS: function() {
-                    return L
+                    return j
                 },
                 Xv: function() {
                     return H
                 },
                 _q: function() {
                     return P
                 },
@@ -2663,21 +2663,21 @@
                     } catch (e) {
                         console.warning("Was not possible to copy text: ", e)
                     }
                     document.body.removeChild(t)
                 } else navigator.clipboard.writeText(e || "").catch(console.warn)
             }
 
-            function L(e) {
+            function j(e) {
                 let t;
                 t = "" === e.mediaType ? e.content : "data:".concat(e.mediaType || "text/plain", ";base64,").concat(e.content);
                 const n = document.createElement("a");
                 n.href = t, n.download = e.name, n.click()
             }
-            const j = {
+            const L = {
                 LIST: "LIST",
                 PAGE: "PAGE",
                 PAGE_NEW: "PAGE_NEW",
                 PAGE_EDIT: "PAGE_EDIT",
                 PAGE_REMOVE: "PAGE_REMOVE",
                 ACTION: "ACTION"
             };
@@ -3358,16 +3358,16 @@
                             }
                         }
                         const E = _,
                             I = w,
                             B = _ && _.type === a.ViewTypes.LIST,
                             N = !I && C,
                             D = N && !r[r.length - 1].includes("{"),
-                            L = B && N && r[r.length - 1].includes("{");
-                        if (L && (_.objects.models[a.RequestTypes.RETRIEVE] = C.modelsList, C.objects = _.objects, S)) {
+                            j = B && N && r[r.length - 1].includes("{");
+                        if (j && (_.objects.models[a.RequestTypes.RETRIEVE] = C.modelsList, C.objects = _.objects, S)) {
                             const e = S.isPartial ? a.RequestTypes.PARTIAL_UPDATE : a.RequestTypes.UPDATE;
                             _.objects.models[e] = S.modelsList, S.objects = _.objects
                         }
                         if (I && k && (w.objects.models[a.RequestTypes.CREATE] = k.modelsList, k.objects = w.objects), D && (C.mixins.push(d), C.objects = new o.SingleEntityQueryset(C.path, {
                                 [a.RequestTypes.RETRIEVE]: C.modelsList
                             }, {}, T), k && (k.mixins.push(d), C.objects.models[a.RequestTypes.CREATE] = k.modelsList, k.objects = C.objects), S)) {
                             S.mixins.push(d);
@@ -3379,15 +3379,15 @@
                                 title: w.params.title,
                                 appendFragment: w.params.name
                             }), A && S && C && (t.delete(S.path), t.set(C.path, S), S.path = C.path, S.isEditStyleOnly = !0, C = S), E && D && !C.hidden && _.sublinks.set(C.name, {
                                 name: C.name,
                                 title: C.title,
                                 href: C.path,
                                 isFileResponse: C.isFileResponse
-                            }), C && L && (_.pageView = C, C.listView = _, S && (S.listView = _)), S) {
+                            }), C && j && (_.pageView = C, C.listView = _, S && (S.listView = _)), S) {
                             const e = (0, a.mergeDeep)({}, this.dictionary.paths.operations.page_edit.save),
                                 t = (0, a.mergeDeep)({}, this.dictionary.paths.operations.page_edit.reload);
                             S.actions.set(e.name, e), S.actions.set(t.name, t)
                         }
                         if (S && !A && !S.hidden) {
                             const e = (0, a.mergeDeep)({
                                 view: S
@@ -3409,15 +3409,15 @@
                                 const e = (0, a.mergeDeep)({}, this.dictionary.paths.operations.list.add);
                                 t.actions.set(e.name, e)
                             }
                         }
                         if (!Z || !E || null !== (p = Z.view) && void 0 !== p && p.hidden || (_.actions.set(Z.name, Z), Z.isMultiAction && [a.ViewTypes.PAGE, a.ViewTypes.PAGE_EDIT].includes(_.type) && _.listView && (Z.isEmpty ? _.listView.multiActions.set(Z.name, Z) : _.listView.multiActions.set(Z.name, {
                                 ...Z,
                                 component: x
-                            }))), L) {
+                            }))), j) {
                             const t = e.replace(/^\/|\/$/g, "").split("/").last.replace("{", "").replace("}", "");
                             for (const e of [C, S]) e && (e.pkParamName = t)
                         }
                         if (S && !S.isEditStyleOnly) {
                             const e = (0, a.mergeDeep)({}, this.dictionary.paths.operations.page_edit.cancel);
                             S.actions.set(e.name, e)
                         }
@@ -4382,15 +4382,15 @@
                     }
                     for (const [t, n] of e)
                         for (const e of n) e.reject(new s(t, this.queryset))
                 }
             }
             var r = n(59198),
                 o = n(97348),
-                l = n(38527),
+                l = n(50118),
                 u = n(38191),
                 d = n(88251);
 
             function c(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 if (0 === e.length) return Promise.resolve();
                 const n = e[0].constructor;
@@ -4716,18 +4716,18 @@
                 M = (n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(33948), n(50887)),
                 I = n(38191),
                 R = n(76274),
                 O = n(53259),
                 B = n(2907),
                 N = n(64765),
                 D = n(39487),
-                L = n(14175),
-                j = n(86767),
+                j = n(14175),
+                L = n(86767),
                 q = {};
-            q.styleTagTransform = x(), q.setAttributes = _(), q.insert = v().bind(null, "head"), q.domAPI = h(), q.insertStyleElement = y(), p()(j.Z, q), j.Z && j.Z.locals && j.Z.locals;
+            q.styleTagTransform = x(), q.setAttributes = _(), q.insert = v().bind(null, "head"), q.domAPI = h(), q.insertStyleElement = y(), p()(L.Z, q), L.Z && L.Z.locals && L.Z.locals;
             const $ = (0, i.defineComponent)({
                     name: "StringArrayFieldEdit",
                     props: {
                         field: {
                             type: Object,
                             required: !0
                         },
@@ -4758,15 +4758,15 @@
                                 validator: this.itemsValidator
                             },
                             on: {
                                 change: e => this.$emit("set-value", e)
                             },
                             class: "tags-selector"
                         })];
-                        return this.hideable && e.push((0, i.h)(L.eX, {
+                        return this.hideable && e.push((0, i.h)(j.eX, {
                             nativeOn: {
                                 click: e => this.$emit("hide-field", e)
                             }
                         })), (0, i.h)("div", {
                             class: "input-group"
                         }, e)
                     }
@@ -5092,15 +5092,15 @@
                                         [t]: i
                                     },
                                     o = s.value.slice();
                                 o[e] = a, n("set-value", o)
                             },
                             Card: te.Z,
                             ModelFields: ne.Z,
-                            HideButton: L.eX
+                            HideButton: j.eX
                         }
                     }
                 }),
                 se = (0, Z.Z)(ie, ee, [], !1, null, null, null).exports;
             const ae = (0, i.defineComponent)({
                 components: {
                     field_content_edit: se
@@ -5915,15 +5915,15 @@
                             i = this.translateValue(n);
                         t.text = e ? "⬇ ".concat(i) : "⬆ ".concat(i)
                     }
                     return t
                 }
             }
         },
-        38527: function(e, t, n) {
+        50118: function(e, t, n) {
             n.r(t), n.d(t, {
                 DependFromFkField: function() {
                     return v
                 },
                 DynamicField: function() {
                     return p
                 },
@@ -6138,33 +6138,26 @@
                     props: r.FieldPropsDef,
                     emits: ["set-value"],
                     setup(e, t) {
                         let {
                             emit: n
                         } = t;
                         const i = e,
-                            r = (0, a.getApp)(),
-                            o = (0, s.ref)(r.fieldsResolver.resolveField({
-                                type: "string",
-                                name: i.field.name
-                            }));
+                            a = (0, s.ref)(i.field.getRealField(i.data));
                         return (0, s.watch)((() => i.data[i.field.dependField]), (() => {
-                            o.value = i.field.getRealField(i.data), "edit" === i.type && n("set-value", {
+                            a.value = i.field.getRealField(i.data), "edit" === i.type && n("set-value", {
                                 field: i.field.name,
-                                value: o.value.getInitialValue(),
+                                value: a.value.getInitialValue(),
                                 markChanged: !1
                             })
-                        }), {
-                            immediate: !0
-                        }), {
+                        })), {
                             __sfc: !0,
                             props: i,
                             emit: n,
-                            app: r,
-                            realField: o
+                            realField: a
                         }
                     }
                 }),
                 m = (0, l.Z)(h, f, [], !1, null, null, null).exports;
             class v extends r.BaseField {
                 constructor(e) {
                     super(e), (0, d.Z)(this, "dependField", void 0), (0, d.Z)(this, "dependFieldAttribute", void 0), (0, d.Z)(this, "callback", void 0), this.dependField = this.props.field, this.dependFieldAttribute = this.props.field_attribute, this.callback = this.props.callback
@@ -6653,15 +6646,15 @@
                 FieldsResolver: function() {
                     return E
                 },
                 ModalWindowAndButtonMixin: function() {
                     return Xa.Z
                 },
                 TableRowMixin: function() {
-                    return js.Z
+                    return Ls.Z
                 },
                 addDefaultFields: function() {
                     return rr
                 },
                 array: function() {
                     return V
                 },
@@ -6779,15 +6772,15 @@
                 DateField: function() {
                     return qe
                 },
                 DateFieldContent: function() {
                     return De
                 },
                 DateFieldMixin: function() {
-                    return Le
+                    return je
                 },
                 DateTimeField: function() {
                     return We
                 },
                 DateTimeFieldContent: function() {
                     return He
                 },
@@ -6935,15 +6928,15 @@
             });
             var p = {};
             n.r(p), n.d(p, {
                 MultipleNamedBinaryImageField: function() {
                     return zi
                 },
                 MultipleNamedBinaryImageFieldContentEdit: function() {
-                    return Li
+                    return ji
                 },
                 MultipleNamedBinaryImageFieldContentReadonly: function() {
                     return Bi
                 },
                 MultipleNamedBinaryImageFieldMixin: function() {
                     return Gi
                 }
@@ -7103,30 +7096,30 @@
                 PasswordFieldMixin: function() {
                     return Ra
                 }
             });
             var C = {};
             n.r(C), n.d(C, {
                 ColorField: function() {
-                    return La
+                    return ja
                 },
                 ColorFieldContentMixin: function() {
                     return Na
                 },
                 ColorFieldMixin: function() {
                     return Da
                 }
             });
             var S = {};
             n.r(S), n.d(S, {
                 EmailField: function() {
                     return qa
                 },
                 EmailFieldMixin: function() {
-                    return ja
+                    return La
                 }
             });
             var k = {};
             n.r(k), n.d(k, {
                 HiddenField: function() {
                     return Ua
                 },
@@ -7327,17 +7320,17 @@
                             this.field.options.default && !i.includes(this.field.options.default) && n.push(this.field.options.default), n = n.concat(i), t(n.filter((t => -1 != t.indexOf(e))))
                         },
                         setValueByHandsInStore(e) {
                             this.$emit("set-value", e)
                         }
                     }
                 },
-                L = D,
-                j = n(51900),
-                q = (0, j.Z)(L, I, [], !1, null, null, null).exports,
+                j = D,
+                L = n(51900),
+                q = (0, L.Z)(j, I, [], !1, null, null, null).exports,
                 $ = {
                     mixins: [A.BaseFieldMixin],
                     components: {
                         field_content_edit: q
                     }
                 };
             class U extends M.StringField {
@@ -7435,15 +7428,15 @@
                 ae = n(19216),
                 re = n.n(ae),
                 oe = n(44589),
                 le = n.n(oe),
                 ue = n(70261),
                 de = {};
             de.styleTagTransform = le(), de.setAttributes = se(), de.insert = ne().bind(null, "head"), de.domAPI = ee(), de.insertStyleElement = re(), J()(ue.Z, de), ue.Z && ue.Z.locals && ue.Z.locals;
-            var ce = (0, j.Z)(Y, W, [], !1, null, "eafa3df0", null).exports,
+            var ce = (0, L.Z)(Y, W, [], !1, null, "eafa3df0", null).exports,
                 pe = function() {
                     var e = this,
                         t = e._self._c;
                     return t("div", {
                         class: e.classes,
                         attrs: {
                             onselectstart: "return false",
@@ -7465,15 +7458,15 @@
                             return ["boolean-select_disabled"]
                         }
                     }
                 },
                 he = n(3377),
                 me = {};
             me.styleTagTransform = le(), me.setAttributes = se(), me.insert = ne().bind(null, "head"), me.domAPI = ee(), me.insertStyleElement = re(), J()(he.Z, me), he.Z && he.Z.locals && he.Z.locals;
-            var ve = (0, j.Z)(fe, pe, [], !1, null, "b4f7c9d8", null).exports,
+            var ve = (0, L.Z)(fe, pe, [], !1, null, "b4f7c9d8", null).exports,
                 ge = function() {
                     var e = this;
                     return (0, e._self._c)("i", {
                         class: e.classes,
                         style: e.styles
                     })
                 };
@@ -7482,15 +7475,15 @@
                     mixins: [A.BaseFieldListView],
                     computed: {
                         classes() {
                             return this.value ? "boolean-true fa fa-check" : "boolean-false fa fa-times"
                         }
                     }
                 },
-                be = (0, j.Z)(_e, ge, [], !1, null, null, null).exports,
+                be = (0, L.Z)(_e, ge, [], !1, null, null, null).exports,
                 ye = {
                     mixins: [n(30636).Z],
                     methods: {
                         toggleValue() {
                             this.setValue(!this.value)
                         }
                     },
@@ -7697,15 +7690,15 @@
                         },
                         getLabel(e, t) {
                             return e.labels && e.labels[t.number] ? e.labels[t.number] : t.number
                         }
                     }
                 },
                 Ze = Fe,
-                Ae = (0, j.Z)(Ze, ke, [], !1, null, null, null).exports,
+                Ae = (0, L.Z)(Ze, ke, [], !1, null, null, null).exports,
                 Te = n(14175),
                 Pe = {
                     mixins: [Te.Di],
                     data() {
                         return {
                             iconClasses: ["fas", "fa-pencil-alt"],
                             helpText: "Crontab form"
@@ -8002,15 +7995,15 @@
                                 a = "";
                             for (let e in i) i[e].length < s && (s = i[e].length, a = i[e]);
                             return a
                         }
                     }
                 },
                 Ve = Ee,
-                Me = (0, j.Z)(Ve, Se, [], !1, null, null, null).exports,
+                Me = (0, L.Z)(Ve, Se, [], !1, null, null, null).exports,
                 Ie = {
                     components: {
                         field_content_edit: {
                             mixins: [A.BaseFieldContentEdit, Me]
                         }
                     }
                 };
@@ -8036,42 +8029,42 @@
                 De = {
                     data() {
                         return {
                             inputType: "date"
                         }
                     }
                 },
-                Le = {
+                je = {
                     components: {
                         field_content_readonly: {
                             mixins: [A.BaseFieldContentReadonlyMixin, De]
                         },
                         field_content_edit: {
                             mixins: [A.BaseFieldContentEdit, De]
                         }
                     }
                 };
-            class je extends A.BaseField {
+            class Le extends A.BaseField {
                 constructor(e) {
                     super(e), this.dateInnerFormat = "YYYY-MM-DD", this.dateRepresentFormat = this.props.format || this.dateInnerFormat
                 }
                 _getValue(e, t) {
                     if (e) return Ne()(e).format(t)
                 }
                 toInner(e) {
                     return this._getValue(super.toInner(e), this.dateInnerFormat)
                 }
                 toRepresent(e) {
                     return this._getValue(super.toInner(e), this.dateRepresentFormat)
                 }
                 static get mixins() {
-                    return super.mixins.concat(Le)
+                    return super.mixins.concat(je)
                 }
             }
-            var qe = je,
+            var qe = Le,
                 $e = n(94611),
                 Ue = n.n($e),
                 He = {
                     data() {
                         return {
                             inputType: "datetime-local"
                         }
@@ -8249,15 +8242,15 @@
             it._withStripped = !0;
             var st = {
                     mixins: [Te.Di]
                 },
                 at = n(8947),
                 rt = {};
             rt.styleTagTransform = le(), rt.setAttributes = se(), rt.insert = ne().bind(null, "head"), rt.domAPI = ee(), rt.insertStyleElement = re(), J()(at.Z, rt), at.Z && at.Z.locals && at.Z.locals;
-            var ot = (0, j.Z)(st, it, [], !1, null, "0567e189", null).exports,
+            var ot = (0, L.Z)(st, it, [], !1, null, "0567e189", null).exports,
                 lt = {
                     components: {
                         DownButton: {
                             mixins: [ot],
                             data() {
                                 return {
                                     iconClasses: ["fa", "fa-chevron-left"],
@@ -8278,15 +8271,15 @@
                     mixins: [A.BaseFieldContentEdit],
                     data() {
                         return {
                             class_list: ["form-control", "uptime-input"]
                         }
                     }
                 },
-                ut = (0, j.Z)(lt, nt, [], !1, null, null, null).exports;
+                ut = (0, L.Z)(lt, nt, [], !1, null, null, null).exports;
             const dt = {
                     mask: tt.ZP.MaskedRange,
                     from: 0,
                     to: 99
                 },
                 ct = {
                     mask: tt.ZP.MaskedRange,
@@ -8441,15 +8434,15 @@
                     return (0, T.getTimeInUptimeFormat)(super.toRepresent(e))
                 }
                 static get mixins() {
                     return super.mixins.concat(vt)
                 }
             }
             var _t = gt,
-                bt = n(38527),
+                bt = n(50118),
                 yt = {
                     extends: Te.Di,
                     data() {
                         return {
                             wrapperClasses: [],
                             wrapperStyles: {},
                             spanClasses: ["btn", "btn-default", "btn-right", "textfile"],
@@ -8561,15 +8554,15 @@
                     },
                     methods: {
                         onChange(e) {
                             this.$emit("read-file", e)
                         }
                     }
                 }),
-                St = (0, j.Z)(Ct, xt, [], !1, null, null, null).exports,
+                St = (0, L.Z)(Ct, xt, [], !1, null, null, null).exports,
                 kt = (0, G.defineComponent)({
                     components: {
                         ReadFileButton: St
                     },
                     extends: A.BaseFieldContentEdit,
                     emits: ["set-value", "hide-field"],
                     data() {
@@ -8589,15 +8582,15 @@
                             this.$emit("set-value", e.target.value)
                         }
                     }
                 }),
                 Ft = n(26560),
                 Zt = {};
             Zt.styleTagTransform = le(), Zt.setAttributes = se(), Zt.insert = ne().bind(null, "head"), Zt.domAPI = ee(), Zt.insertStyleElement = re(), J()(Ft.Z, Zt), Ft.Z && Ft.Z.locals && Ft.Z.locals;
-            var At = (0, j.Z)(kt, wt, [], !1, null, "d92651d4", null).exports,
+            var At = (0, L.Z)(kt, wt, [], !1, null, "d92651d4", null).exports,
                 Tt = (0, G.defineComponent)({
                     components: {
                         field_content_edit: At
                     },
                     extends: A.BaseFieldMixin,
                     props: A.FieldPropsDef,
                     data() {
@@ -8765,20 +8758,20 @@
             };
             Nt._withStripped = !0;
             const Dt = function() {
                 const e = document.createElement("div");
                 return ("draggable" in e || "ondragstart" in e && "ondrop" in e) && "FormData" in window && "FileReader" in window
             }();
 
-            function Lt(e) {
+            function jt(e) {
                 e.preventDefault(), e.stopPropagation()
             }
-            const jt = ["dragover", "dragenter"],
+            const Lt = ["dragover", "dragenter"],
                 qt = ["dragleave", "dragend", "drop"],
-                $t = ["drag", "dragstart", ...jt, ...qt];
+                $t = ["drag", "dragstart", ...Lt, ...qt];
             var Ut = (0, G.defineComponent)({
                     __name: "FileInput",
                     props: {
                         multiple: {
                             type: Boolean
                         },
                         text: null,
@@ -8807,17 +8800,17 @@
                                 onDragLeave: i,
                                 onDragFinished: s
                             } = e;
                             if (!Dt) return;
 
                             function a(e) {
                                 const a = t.value;
-                                for (const t of $t) a[e](t, Lt);
+                                for (const t of $t) a[e](t, jt);
                                 if (n)
-                                    for (const t of jt) a[e](t, n);
+                                    for (const t of Lt) a[e](t, n);
                                 if (i)
                                     for (const t of qt) a[e](t, i);
                                 s && a[e]("drop", s)
                             }(0, G.onBeforeUnmount)((() => {
                                 t.value && a("removeEventListener")
                             }));
                             const r = (0, G.watch)(t, (() => {
@@ -8843,15 +8836,15 @@
                             }
                         }
                     }
                 }),
                 Ht = n(79721),
                 Gt = {};
             Gt.styleTagTransform = le(), Gt.setAttributes = se(), Gt.insert = ne().bind(null, "head"), Gt.domAPI = ee(), Gt.insertStyleElement = re(), J()(Ht.Z, Gt), Ht.Z && Ht.Z.locals && Ht.Z.locals;
-            var zt = (0, j.Z)(Ut, Nt, [], !1, null, "47a537a6", null).exports,
+            var zt = (0, L.Z)(Ut, Nt, [], !1, null, "47a537a6", null).exports,
                 Wt = (0, G.defineComponent)({
                     __name: "FileFieldSelector",
                     props: {
                         field: null,
                         text: null,
                         multiple: {
                             type: Boolean
@@ -8872,30 +8865,30 @@
                         return {
                             __sfc: !0,
                             emit: n,
                             FileInput: zt
                         }
                     }
                 }),
-                Qt = (0, j.Z)(Wt, Bt, [], !1, null, null, null).exports,
+                Qt = (0, L.Z)(Wt, Bt, [], !1, null, null, null).exports,
                 Yt = (0, G.defineComponent)({
                     components: {
                         FileFieldSelector: Qt
                     },
                     extends: At,
                     methods: {
                         readFile(e) {
                             const t = e[0];
                             if (!t) return;
                             const n = new FileReader;
                             n.onload = () => this.$emit("set-value", (0, T.arrayBufferToBase64)(n.result)), n.readAsArrayBuffer(t)
                         }
                     }
                 }),
-                Kt = (0, j.Z)(Yt, Ot, [], !1, null, null, null).exports,
+                Kt = (0, L.Z)(Yt, Ot, [], !1, null, null, null).exports,
                 Jt = function() {
                     var e = this,
                         t = e._self._c;
                     return e.value ? t("a", {
                         staticClass: "btn btn-secondary",
                         attrs: {
                             href: "data:application/octet-stream;base64,".concat(e.value),
@@ -8905,15 +8898,15 @@
                         staticClass: "fas fa-download"
                     })]) : e._e()
                 };
             Jt._withStripped = !0;
             var Xt = {
                     mixins: [A.BaseFieldContentReadonlyMixin]
                 },
-                en = (0, j.Z)(Xt, Jt, [], !1, null, null, null).exports,
+                en = (0, L.Z)(Xt, Jt, [], !1, null, null, null).exports,
                 tn = (0, G.defineComponent)({
                     components: {
                         field_content_edit: Kt,
                         field_content_readonly: en
                     },
                     extends: Tt
                 }),
@@ -9179,15 +9172,15 @@
                             Card: hn.Z
                         }
                     }
                 }),
                 vn = n(11435),
                 gn = {};
             gn.styleTagTransform = le(), gn.setAttributes = se(), gn.insert = ne().bind(null, "head"), gn.domAPI = ee(), gn.insertStyleElement = re(), J()(vn.Z, gn), vn.Z && vn.Z.locals && vn.Z.locals;
-            var _n = (0, j.Z)(mn, fn, [], !1, null, "2efa8755", null).exports,
+            var _n = (0, L.Z)(mn, fn, [], !1, null, "2efa8755", null).exports,
                 bn = (0, G.defineComponent)({
                     __name: "MultipleFilesInput",
                     props: {
                         field: null,
                         text: null,
                         multiple: {
                             type: Boolean
@@ -9221,15 +9214,15 @@
                                 o.value = [], e.some((e => !s(e))) ? o.value = e : n("input", e)
                             },
                             FileNamesEditor: _n,
                             FileFieldSelector: Qt
                         }
                     }
                 }),
-                yn = (0, j.Z)(bn, on, [], !1, null, null, null).exports,
+                yn = (0, L.Z)(bn, on, [], !1, null, null, null).exports,
                 wn = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("ul", e._l(e.files, (function(i, s) {
                         return t("li", {
                             key: s
@@ -9285,15 +9278,15 @@
                             }
                         }
                     }
                 }),
                 Cn = n(34498),
                 Sn = {};
             Sn.styleTagTransform = le(), Sn.setAttributes = se(), Sn.insert = ne().bind(null, "head"), Sn.domAPI = ee(), Sn.insertStyleElement = re(), J()(Cn.Z, Sn), Cn.Z && Cn.Z.locals && Cn.Z.locals;
-            var kn = (0, j.Z)(xn, wn, [], !1, null, "4fdbf401", null).exports,
+            var kn = (0, L.Z)(xn, wn, [], !1, null, "4fdbf401", null).exports,
                 Fn = (0, G.defineComponent)({
                     __name: "MultipleNamedBinaryFileFieldContentEdit",
                     props: A.FieldEditPropsDef,
                     emits: ["set-value", "hide-field", "clear"],
                     setup(e, t) {
                         let {
                             emit: n
@@ -9319,15 +9312,15 @@
                                 n("set-value", [...null !== (t = i.value) && void 0 !== t ? t : [], ...s])
                             },
                             MultipleFilesInput: yn,
                             FilesList: kn
                         }
                     }
                 }),
-                Zn = (0, j.Z)(Fn, rn, [], !1, null, null, null).exports,
+                Zn = (0, L.Z)(Fn, rn, [], !1, null, null, null).exports,
                 An = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return e.value && e.value.length > 0 ? t(n.BootstrapModal, {
                         attrs: {
                             styles: "width: 90vw; max-width: 1000px",
@@ -9380,15 +9373,15 @@
                             props: t,
                             title: n,
                             BootstrapModal: Tn.Z,
                             FilesList: kn
                         }
                     }
                 }),
-                En = (0, j.Z)(Pn, An, [], !1, null, null, null).exports,
+                En = (0, L.Z)(Pn, An, [], !1, null, null, null).exports,
                 Vn = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("div", [t("div", [e._v("\n        " + e._s(n.text) + "\n    ")]), e._v(" "), e.value && e.value.length > 0 ? t(n.FilesList, {
                         attrs: {
                             files: e.value,
@@ -9412,15 +9405,15 @@
                             __sfc: !0,
                             props: t,
                             text: n,
                             FilesList: kn
                         }
                     }
                 }),
-                In = (0, j.Z)(Mn, Vn, [], !1, null, null, null).exports,
+                In = (0, L.Z)(Mn, Vn, [], !1, null, null, null).exports,
                 Rn = (0, G.defineComponent)({
                     components: {
                         field_content_readonly: In,
                         field_content_edit: Zn,
                         field_list_view: En
                     },
                     extends: A.BaseFieldMixin
@@ -9567,16 +9560,16 @@
                                 r.value || n("done", new File([i.file], s.value, {
                                     type: i.file.type
                                 }))
                             }
                         }
                     }
                 }),
-                Ln = (0, j.Z)(Dn, Nn, [], !1, null, null, null).exports,
-                jn = (0, G.defineComponent)({
+                jn = (0, L.Z)(Dn, Nn, [], !1, null, null, null).exports,
+                Ln = (0, G.defineComponent)({
                     __name: "SingleFileInput",
                     props: {
                         field: null,
                         text: null,
                         multiple: {
                             type: Boolean
                         },
@@ -9606,20 +9599,20 @@
                             maxNameLength: r,
                             minNameLength: o,
                             readFile: async function(e) {
                                 s.value = void 0;
                                 const t = e[0];
                                 t && (a(t) ? n("input", t) : s.value = t)
                             },
-                            FileRenameInput: Ln,
+                            FileRenameInput: jn,
                             FileFieldSelector: Qt
                         }
                     }
                 }),
-                qn = (0, j.Z)(jn, Bn, [], !1, null, null, null).exports,
+                qn = (0, L.Z)(Ln, Bn, [], !1, null, null, null).exports,
                 $n = (0, G.defineComponent)({
                     __name: "NamedBinaryFileFieldContentEdit",
                     props: A.FieldEditPropsDef,
                     emits: ["set-value", "hide-field", "clear"],
                     setup(e, t) {
                         let {
                             emit: n
@@ -9635,15 +9628,15 @@
                                 const t = await (0, T.readFileAsObject)(e);
                                 cn(i.field, [t]) && n("set-value", t)
                             },
                             SingleFileInput: qn
                         }
                     }
                 }),
-                Un = (0, j.Z)($n, On, [], !1, null, null, null).exports,
+                Un = (0, L.Z)($n, On, [], !1, null, null, null).exports,
                 Hn = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return n.link ? t("a", {
                         attrs: {
                             href: n.link,
@@ -9674,15 +9667,15 @@
                             props: t,
                             link: n,
                             fileName: i,
                             text: s
                         }
                     }
                 }),
-                zn = (0, j.Z)(Gn, Hn, [], !1, null, null, null).exports,
+                zn = (0, L.Z)(Gn, Hn, [], !1, null, null, null).exports,
                 Wn = (0, G.defineComponent)({
                     components: {
                         field_content_readonly: zn,
                         field_content_edit: Un,
                         field_list_view: zn
                     },
                     extends: A.BaseFieldMixin
@@ -9807,15 +9800,15 @@
                             BootstrapModal: Tn.Z
                         }
                     }
                 }),
                 ti = n(70545),
                 ni = {};
             ni.styleTagTransform = le(), ni.setAttributes = se(), ni.insert = ne().bind(null, "head"), ni.domAPI = ee(), ni.insertStyleElement = re(), J()(ti.Z, ni), ti.Z && ti.Z.locals && ti.Z.locals;
-            var ii = (0, j.Z)(ei, Xn, [], !1, null, "1fe7c439", null).exports,
+            var ii = (0, L.Z)(ei, Xn, [], !1, null, "1fe7c439", null).exports,
                 si = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("div", [n.showPreview ? t(n.ImageBlock, {
                         attrs: {
                             field: e.field,
@@ -10235,15 +10228,15 @@
                             }
                         }
                     }
                 }),
                 fi = n(61186),
                 hi = {};
             hi.styleTagTransform = le(), hi.setAttributes = se(), hi.insert = ne().bind(null, "head"), hi.domAPI = ee(), hi.insertStyleElement = re(), J()(fi.Z, hi), fi.Z && fi.Z.locals && fi.Z.locals;
-            var mi = (0, j.Z)(pi, oi, [], !1, null, "0ec81725", null).exports,
+            var mi = (0, L.Z)(pi, oi, [], !1, null, "0ec81725", null).exports,
                 vi = (0, G.defineComponent)({
                     __name: "ResolutionValidatorModal",
                     props: {
                         field: null,
                         images: null
                     },
                     emits: ["cancel", "validated"],
@@ -10281,15 +10274,15 @@
                             ResolutionValidatorImage: mi
                         }
                     }
                 }),
                 gi = n(85135),
                 _i = {};
             _i.styleTagTransform = le(), _i.setAttributes = se(), _i.insert = ne().bind(null, "head"), _i.domAPI = ee(), _i.insertStyleElement = re(), J()(gi.Z, _i), gi.Z && gi.Z.locals && gi.Z.locals;
-            var bi = (0, j.Z)(vi, ri, [], !1, null, "96c3182c", null).exports,
+            var bi = (0, L.Z)(vi, ri, [], !1, null, "96c3182c", null).exports,
                 yi = (0, G.defineComponent)({
                     __name: "NamedBinaryImageFieldContentEdit",
                     props: A.FieldEditPropsDef,
                     emits: ["set-value", "hide-field", "clear"],
                     setup(e, t) {
                         let {
                             emit: n
@@ -10321,15 +10314,15 @@
                             readFiles: u,
                             ImageBlock: ii,
                             ResolutionValidatorModal: bi,
                             SingleFileInput: qn
                         }
                     }
                 }),
-                wi = (0, j.Z)(yi, si, [], !1, null, null, null).exports,
+                wi = (0, L.Z)(yi, si, [], !1, null, null, null).exports,
                 xi = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return e.value && e.value.content ? t(n.ImageBlock, {
                         attrs: {
                             field: e.field,
@@ -10352,15 +10345,15 @@
                     setup(e) {
                         return {
                             __sfc: !0,
                             ImageBlock: ii
                         }
                     }
                 }),
-                Si = (0, j.Z)(Ci, xi, [], !1, null, null, null).exports,
+                Si = (0, L.Z)(Ci, xi, [], !1, null, null, null).exports,
                 ki = (0, G.defineComponent)({
                     components: {
                         field_content_readonly: Si,
                         field_content_edit: wi,
                         field_list_view: Si
                     },
                     extends: A.BaseFieldMixin
@@ -10558,15 +10551,15 @@
                         }
                     }
                 })),
                 Vi = Ei,
                 Mi = n(20649),
                 Ii = {};
             Ii.styleTagTransform = le(), Ii.setAttributes = se(), Ii.insert = ne().bind(null, "head"), Ii.domAPI = ee(), Ii.insertStyleElement = re(), J()(Mi.Z, Ii), Mi.Z && Mi.Z.locals && Mi.Z.locals;
-            var Ri = (0, j.Z)(Vi, Ti, [], !1, null, "0ad7db6c", null).exports,
+            var Ri = (0, L.Z)(Vi, Ti, [], !1, null, "0ad7db6c", null).exports,
                 Oi = (0, G.defineComponent)({
                     __name: "MultipleNamedBinaryImageFieldContentReadonly",
                     props: {
                         field: null,
                         value: null
                     },
                     setup(e) {
@@ -10579,15 +10572,15 @@
                             __sfc: !0,
                             props: t,
                             text: n,
                             Carousel: Ri
                         }
                     }
                 }),
-                Bi = (0, j.Z)(Oi, Ai, [], !1, null, null, null).exports,
+                Bi = (0, L.Z)(Oi, Ai, [], !1, null, null, null).exports,
                 Ni = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("div", [n.imagesForValidation ? t(n.ResolutionValidatorModal, {
                         attrs: {
                             field: e.field,
@@ -10662,16 +10655,16 @@
                             readFiles: l,
                             ResolutionValidatorModal: bi,
                             MultipleFilesInput: yn,
                             Carousel: Ri
                         }
                     }
                 }),
-                Li = (0, j.Z)(Di, Ni, [], !1, null, null, null).exports,
-                ji = function() {
+                ji = (0, L.Z)(Di, Ni, [], !1, null, null, null).exports,
+                Li = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return e.value && e.value.length > 0 ? t(n.BootstrapModal, {
                         attrs: {
                             classes: "modal-lg",
                             title: e.$ts(e.field.title)
@@ -10724,15 +10717,15 @@
                                 }, [t("i", {
                                     staticClass: "fas fa-eye"
                                 })])]
                             }
                         }], null, !1, 2374029067)
                     }) : e._e()
                 };
-            ji._withStripped = !0;
+            Li._withStripped = !0;
             var qi = (0, G.defineComponent)({
                     __name: "MultipleNamedBinaryImageFieldListView",
                     props: {
                         field: null,
                         value: null
                     },
                     setup(e) {
@@ -10762,19 +10755,19 @@
                             BootstrapModal: Tn.Z
                         }
                     }
                 }),
                 $i = n(22985),
                 Ui = {};
             Ui.styleTagTransform = le(), Ui.setAttributes = se(), Ui.insert = ne().bind(null, "head"), Ui.domAPI = ee(), Ui.insertStyleElement = re(), J()($i.Z, Ui), $i.Z && $i.Z.locals && $i.Z.locals;
-            var Hi = (0, j.Z)(qi, ji, [], !1, null, "710d8c99", null).exports,
+            var Hi = (0, L.Z)(qi, Li, [], !1, null, "710d8c99", null).exports,
                 Gi = (0, G.defineComponent)({
                     components: {
                         field_content_readonly: Bi,
-                        field_content_edit: Li,
+                        field_content_edit: ji,
                         field_list_view: Hi
                     },
                     extends: A.BaseFieldMixin
                 }),
                 zi = class extends Jn {
                     constructor(e) {
                         var t;
@@ -11033,15 +11026,15 @@
                             BootstrapModal: Tn.Z
                         }
                     }
                 }),
                 rs = n(21805),
                 os = {};
             os.styleTagTransform = le(), os.setAttributes = se(), os.insert = ne().bind(null, "head"), os.domAPI = ee(), os.insertStyleElement = re(), J()(rs.Z, os), rs.Z && rs.Z.locals && rs.Z.locals;
-            var ls = (0, j.Z)(as, es, [], !1, null, "37a0f1ac", null).exports,
+            var ls = (0, L.Z)(as, es, [], !1, null, "37a0f1ac", null).exports,
                 us = (0, G.defineComponent)({
                     __name: "CSVFileFieldEdit",
                     props: A.FieldEditPropsDef,
                     emits: ["set-value", "hide-field", "clear"],
                     setup(e, t) {
                         let {
                             emit: n
@@ -11081,15 +11074,15 @@
                             FileFieldSelector: Qt
                         }
                     }
                 }),
                 ds = n(56296),
                 cs = {};
             cs.styleTagTransform = le(), cs.setAttributes = se(), cs.insert = ne().bind(null, "head"), cs.domAPI = ee(), cs.insertStyleElement = re(), J()(ds.Z, cs), ds.Z && ds.Z.locals && ds.Z.locals;
-            var ps = (0, j.Z)(us, Ji, [], !1, null, "6d3fcb4a", null).exports,
+            var ps = (0, L.Z)(us, Ji, [], !1, null, "6d3fcb4a", null).exports,
                 fs = function() {
                     var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return n.rows.length > 0 ? t("div", {
                         staticStyle: {
                             margin: "0"
@@ -11184,15 +11177,15 @@
                 }),
                 ms = n(52456),
                 vs = {};
             vs.styleTagTransform = le(), vs.setAttributes = se(), vs.insert = ne().bind(null, "head"), vs.domAPI = ee(), vs.insertStyleElement = re(), J()(ms.Z, vs), ms.Z && ms.Z.locals && ms.Z.locals;
             var gs = n(30518),
                 _s = {};
             _s.styleTagTransform = le(), _s.setAttributes = se(), _s.insert = ne().bind(null, "head"), _s.domAPI = ee(), _s.insertStyleElement = re(), J()(gs.Z, _s), gs.Z && gs.Z.locals && gs.Z.locals;
-            var bs = (0, j.Z)(hs, fs, [], !1, null, "63e30122", null).exports,
+            var bs = (0, L.Z)(hs, fs, [], !1, null, "63e30122", null).exports,
                 ys = n(12075);
             const ws = (0, G.defineComponent)({
                 components: {
                     field_content_edit: ps,
                     field_content_readonly: bs
                 },
                 extends: A.BaseFieldMixin
@@ -11361,15 +11354,15 @@
                             inputRef: a,
                             handleBlur: function(e) {
                                 n("set-value", e.target ? e.target.value : void 0)
                             }
                         }
                     }
                 }),
-                Fs = (0, j.Z)(ks, Ss, [], !1, null, null, null).exports,
+                Fs = (0, L.Z)(ks, Ss, [], !1, null, null, null).exports,
                 Zs = (0, G.defineComponent)({
                     components: {
                         field_content_edit: Fs
                     },
                     mixins: [Cs.FKFieldMixin]
                 });
             class As extends Cs.FKField {
@@ -11582,15 +11575,15 @@
                             void 0 === e.value && void 0 === e.prefetch_value && (e = void 0), this.$emit("set-value", e)
                         },
                         updateQuerySet(e) {
                             this.queryset = e
                         }
                     }
                 },
-                Ms = (0, j.Z)(Vs, Ps, [], !1, null, null, null).exports,
+                Ms = (0, L.Z)(Vs, Ps, [], !1, null, null, null).exports,
                 Is = {
                     components: {
                         field_content_edit: Ms
                     }
                 },
                 Rs = class extends Ts {
                     static get mixins() {
@@ -11643,15 +11636,15 @@
                             this.$emit("filter", this.$refs.input.value)
                         },
                         cleanFilterValue() {
                             this.$refs.input.value = "", this.applyFilter()
                         }
                     }
                 },
-                Ns = (0, j.Z)(Bs, Os, [function() {
+                Ns = (0, L.Z)(Bs, Os, [function() {
                     var e = this._self._c;
                     return e("span", {
                         staticClass: "input-group-text"
                     }, [e("i", {
                         staticClass: "fa fa-search",
                         attrs: {
                             "aria-hidden": "true"
@@ -11694,15 +11687,15 @@
                             on: {
                                 "change-value": e.changeValue
                             }
                         })
                     })), 1)])
                 };
             Ds._withStripped = !0;
-            var Ls = function() {
+            var js = function() {
                 var e = this,
                     t = e._self._c;
                 return t("tr", {
                     staticClass: "item-row item-row-id highlight-tr",
                     class: e.is_selected,
                     attrs: {
                         "data-id": e.instance.getPkValue(),
@@ -11734,18 +11727,18 @@
                                 list_view: !0,
                                 use_prop_data: !0
                             }
                         }
                     })], 1)
                 }))], 2)
             };
-            Ls._withStripped = !0;
-            var js = n(88225),
+            js._withStripped = !0;
+            var Ls = n(88225),
                 qs = {
-                    mixins: [js.Z],
+                    mixins: [Ls.Z],
                     props: {
                         qs: {
                             type: Object,
                             required: !0
                         },
                         instance: {
                             type: Object,
@@ -11788,15 +11781,15 @@
                             this.$emit("change-value", {
                                 view_val: e,
                                 value_val: t
                             })
                         }
                     }
                 },
-                $s = (0, j.Z)(qs, Ls, [], !1, null, null, null).exports,
+                $s = (0, L.Z)(qs, js, [], !1, null, null, null).exports,
                 Us = {
                     components: {
                         fma_table_row: $s
                     },
                     props: {
                         instances: {
                             type: Object,
@@ -11822,15 +11815,15 @@
                     },
                     methods: {
                         changeValue(e) {
                             this.$emit("change-value", e)
                         }
                     }
                 },
-                Hs = (0, j.Z)(Us, Ds, [], !1, null, null, null).exports;
+                Hs = (0, L.Z)(Us, Ds, [], !1, null, null, null).exports;
             class Gs extends Cs.FKField {
                 constructor(e) {
                     super(e), this.onlyLastChild = this.props.only_last_child, this.parentFieldName = this.props.parent_field_name, this.limit = 1e5
                 }
                 makeRequest() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 0,
                         t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
@@ -11991,15 +11984,15 @@
                             this.setValue(this.field.getEmptyValue()), this.selectedNode.unselect(), this.selectedNode = null, this.selectedText = ""
                         }
                     }
                 },
                 Ys = n(80306),
                 Ks = {};
             Ks.styleTagTransform = le(), Ks.setAttributes = se(), Ks.insert = ne().bind(null, "head"), Ks.domAPI = ee(), Ks.insertStyleElement = re(), J()(Ys.Z, Ks), Ys.Z && Ys.Z.locals && Ys.Z.locals;
-            var Js = (0, j.Z)(Qs, Ws, [], !1, null, "6009ed91", null).exports,
+            var Js = (0, L.Z)(Qs, Ws, [], !1, null, "6009ed91", null).exports,
                 Xs = n(32900),
                 ea = {
                     mixins: [A.BaseFieldMixin],
                     components: {
                         field_content_edit: Js,
                         field_content_readonly: Xs.Z,
                         field_list_view: Xs.Z
@@ -12029,15 +12022,15 @@
                             return this.value && "string" == typeof this.value ? JSON.parse(this.value) : this.value
                         }
                     }
                 },
                 sa = n(92469),
                 aa = {};
             aa.styleTagTransform = le(), aa.setAttributes = se(), aa.insert = ne().bind(null, "head"), aa.domAPI = ee(), aa.insertStyleElement = re(), J()(sa.Z, aa), sa.Z && sa.Z.locals && sa.Z.locals;
-            var ra = (0, j.Z)(ia, na, [], !1, null, "e3f84444", null).exports,
+            var ra = (0, L.Z)(ia, na, [], !1, null, "e3f84444", null).exports,
                 oa = {
                     provide() {
                         return {
                             jsonMapper: this.field.jsonMapper
                         }
                     },
                     components: {
@@ -12067,15 +12060,15 @@
                 isStringArray(e) {
                     return (e.length > 0 || e.size > 0) && e.every((e => "string" == typeof e || "symbol" == typeof e))
                 }
             }
             class da extends A.BaseField {
                 constructor() {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0;
-                    super(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {}), this.jsonMapper = e || new ua
+                    super(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {}), (0, Z.Z)(this, "allowedMediaTypes", ["application/json"]), this.jsonMapper = e || new ua
                 }
                 getEmptyValue() {
                     return null
                 }
                 static get mixins() {
                     return super.mixins.concat(oa)
                 }
@@ -12114,15 +12107,15 @@
                     name: "JsonArray",
                     components: {
                         Card: hn.Z
                     },
                     mixins: [fa],
                     inject: ["jsonMapper"]
                 },
-                ma = (0, j.Z)(ha, pa, [], !1, null, null, null).exports,
+                ma = (0, L.Z)(ha, pa, [], !1, null, null, null).exports,
                 va = function() {
                     var e = this,
                         t = e._self._c;
                     return e.isEmpty ? t("div") : t("Card", {
                         attrs: {
                             title: e.title,
                             collapsable: ""
@@ -12152,15 +12145,15 @@
                             return !this.valueAsObj || 0 === Object.keys(this.valueAsObj).length
                         },
                         valueAsObj() {
                             return this.value instanceof Map ? Object.fromEntries(this.value.entries()) : this.value
                         }
                     }
                 },
-                _a = (0, j.Z)(ga, va, [], !1, null, null, null).exports,
+                _a = (0, L.Z)(ga, va, [], !1, null, null, null).exports,
                 ba = function() {
                     var e = this,
                         t = e._self._c;
                     return t("div", {
                         staticClass: "json-string"
                     }, [t("b", [e._v(e._s(e.title))]), e._v("\n    : " + e._s(e.valueAsStr) + "\n")])
                 };
@@ -12173,15 +12166,15 @@
                             return "symbol" == typeof this.value ? this.value.description : this.value
                         }
                     }
                 },
                 wa = n(46934),
                 xa = {};
             xa.styleTagTransform = le(), xa.setAttributes = se(), xa.insert = ne().bind(null, "head"), xa.domAPI = ee(), xa.insertStyleElement = re(), J()(wa.Z, xa), wa.Z && wa.Z.locals && wa.Z.locals;
-            var Ca = (0, j.Z)(ya, ba, [], !1, null, "6e2d9c49", null).exports,
+            var Ca = (0, L.Z)(ya, ba, [], !1, null, "6e2d9c49", null).exports,
                 Sa = function() {
                     var e = this,
                         t = e._self._c;
                     return t("div", {
                         staticClass: "string-json-array"
                     }, [t("label", [e._v(e._s(e.title))]), e._v(" "), e._l(e.strings, (function(n, i) {
                         return t("p", {
@@ -12201,15 +12194,15 @@
                             return this.value.map((e => e ? "symbol" == typeof e ? e.description : e : ""))
                         }
                     }
                 },
                 Fa = n(86716),
                 Za = {};
             Za.styleTagTransform = le(), Za.setAttributes = se(), Za.insert = ne().bind(null, "head"), Za.domAPI = ee(), Za.insertStyleElement = re(), J()(Fa.Z, Za), Fa.Z && Fa.Z.locals && Fa.Z.locals;
-            var Aa = (0, j.Z)(ka, Sa, [], !1, null, "432de31e", null).exports;
+            var Aa = (0, L.Z)(ka, Sa, [], !1, null, "432de31e", null).exports;
             ta.b.add(_a), ta.b.add(ma), ta.b.add(Aa), ta.b.add(Ca);
             var Ta = n(76274),
                 Pa = {
                     data() {
                         return {
                             inputType: "password"
                         }
@@ -12293,15 +12286,15 @@
                             this.inputType = "password" === this.inputType ? "text" : "password"
                         },
                         copy() {
                             (0, T.copyToClipboard)(this.value)
                         }
                     }
                 },
-                Ia = (0, j.Z)(Ma, Ea, [], !1, null, null, null).exports,
+                Ia = (0, L.Z)(Ma, Ea, [], !1, null, null, null).exports,
                 Ra = {
                     components: {
                         field_content_readonly: {
                             mixins: [A.BaseFieldContentReadonlyMixin, Pa]
                         },
                         field_content_edit: Ia
                     }
@@ -12325,15 +12318,15 @@
                             mixins: [A.BaseFieldContentReadonlyMixin, Na]
                         },
                         field_content_edit: {
                             mixins: [A.BaseFieldContentEdit, Na]
                         }
                     }
                 };
-            class La extends A.BaseField {
+            class ja extends A.BaseField {
                 static get mixins() {
                     return super.mixins.concat(Da)
                 }
                 getEmptyValue() {
                     return null
                 }
                 _getValue() {
@@ -12344,29 +12337,29 @@
                     return this._getValue(e)
                 }
                 toRepresent() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this._getValue(e)
                 }
             }
-            const ja = {
+            const La = {
                 components: {
                     field_content_edit: {
                         mixins: [A.BaseFieldContentEdit],
                         data() {
                             return {
                                 inputType: "email"
                             }
                         }
                     }
                 }
             };
             class qa extends M.StringField {
                 static get mixins() {
-                    return super.mixins.concat(ja)
+                    return super.mixins.concat(La)
                 }
                 static get validation_reg_exp() {
                     return /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
                 }
                 validateValue() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         t = super.validateValue(e);
@@ -12492,15 +12485,15 @@
 
             function rr(e) {
                 for (const [t, n] of [
                         [E.DEFAULT_FIELD_KEY, M.StringField],
                         ["autocomplete", H],
                         ["binfile", nn],
                         ["choices", Ce.ChoicesField],
-                        ["color", La],
+                        ["color", ja],
                         ["crontab", Oe],
                         ["csvfile", xs],
                         ["date", qe],
                         ["date-time", We],
                         ["deep_fk", zs],
                         ["decimal", Je.DecimalField],
                         ["email", qa],
@@ -12858,23 +12851,23 @@
                         attrs: {
                             value: e.value,
                             model: e.field.itemsModel
                         }
                     })
                 };
             D._withStripped = !0;
-            var L = {
+            var j = {
                     name: "RelatedListFieldReadonlyView",
                     mixins: [s.BaseFieldContentReadonlyMixin, V]
                 },
-                j = (0, k.Z)(L, D, [], !1, null, null, null).exports;
+                L = (0, k.Z)(j, D, [], !1, null, null, null).exports;
             const q = {
                 components: {
-                    field_content_readonly: j,
-                    field_content_edit: j,
+                    field_content_readonly: L,
+                    field_content_edit: L,
                     field_list_view: N
                 },
                 mixins: [s.BaseFieldMixin]
             };
             class $ extends s.BaseField {
                 constructor(e) {
                     var t;
@@ -12906,15 +12899,15 @@
                 },
                 i: function() {
                     return o
                 }
             });
             var i = n(70538),
                 s = n(87444),
-                a = n(24389),
+                a = n(83943),
                 r = n(82509);
             const o = (0, i.defineComponent)({
                 components: {
                     field_content_edit: a.Z,
                     field_content_readonly: r.Z
                 },
                 extends: s.BaseFieldMixin
@@ -12924,18 +12917,18 @@
                     return [o]
                 }
             }
         },
         48058: function(e, t, n) {
             n.r(t), n.d(t, {
                 WYSIWYGField: function() {
-                    return c
+                    return p
                 },
                 WYSIWYGFieldMixin: function() {
-                    return d
+                    return c
                 }
             });
             var i = n(70538),
                 s = (n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(33948), n(56716)),
                 a = n(59198);
             const r = new Map([
                     ["ru", {
@@ -12951,15 +12944,30 @@
                         load: () => Promise.resolve()
                     }],
                     ["vi", {
                         code: "vi",
                         load: e => n.e(454).then(n.bind(n, 10860)).then((t => t.default(e)))
                     }]
                 ]),
-                o = (0, i.defineComponent)({
+                o = e => (e.eventEmitter.addEventType("select-file"), {
+                    toolbarItems: [{
+                        groupIndex: 0,
+                        itemIndex: 0,
+                        item: {
+                            name: "select-file",
+                            tooltip: s.a.ts("Select file"),
+                            command: "select-file",
+                            className: "btn fas fa-file-alt"
+                        }
+                    }],
+                    wysiwygCommands: {
+                        "select-file": () => (e.eventEmitter.emit("select-file"), !0)
+                    }
+                }),
+                l = (0, i.defineComponent)({
                     name: "WYSIWYGEditor",
                     props: {
                         readOnly: {
                             type: Boolean,
                             default: !1
                         },
                         initialValue: {
@@ -12967,107 +12975,122 @@
                             default: null
                         }
                     },
                     emits: {
                         change: e => !0
                     },
                     setup(e, t) {
-                        var o;
+                        var l;
                         let {
-                            emit: l
-                        } = t, u = null;
-                        const d = {
+                            emit: u
+                        } = t, d = null;
+                        const c = {
                                 minHeight: "200px",
-                                language: null === (o = r.get(s.a.locale)) || void 0 === o ? void 0 : o.code,
+                                language: null === (l = r.get(s.a.locale)) || void 0 === l ? void 0 : l.code,
                                 useCommandShortcut: !0,
                                 usageStatistics: !1,
                                 hideModeSwitch: !0,
                                 toolbarItems: [
                                     ["heading", "bold", "italic", "strike"],
                                     ["hr", "quote"],
                                     ["ul", "ol", "task", "indent", "outdent"],
                                     ["table", "link"]
                                 ],
-                                theme: (0, a.getApp)().darkModeEnabled ? "dark" : "light"
+                                theme: (0, a.getApp)().darkModeEnabled ? "dark" : "light",
+                                plugins: [o],
+                                hooks: {
+                                    "select-file": async () => {
+                                        var e;
+                                        const t = await new Promise(((e, t) => {
+                                            const n = document.createElement("input");
+                                            n.accept = ".md,text/markdown", n.type = "file", n.addEventListener("change", (() => {
+                                                var i;
+                                                const s = null === (i = n.files) || void 0 === i ? void 0 : i[0];
+                                                s && s.text().then((t => e(t))).catch((e => t(e)))
+                                            })), n.click()
+                                        }));
+                                        u("change", t), null === (e = d) || void 0 === e || e.invoke("setMarkdown", t)
+                                    }
+                                }
                             },
-                            c = (0, i.computed)((() => {
+                            p = (0, i.computed)((() => {
                                 return t = e.readOnly, o = r.get(s.a.locale), (0, i.defineAsyncComponent)((async () => {
                                     const [e, i] = await Promise.all([n.e(742).then(n.bind(n, 49742)), Promise.all([n.e(742), n.e(826)]).then(n.bind(n, 3826)), n.e(345).then(n.bind(n, 3345)), (0, a.getApp)().darkModeEnabled ? n.e(368).then(n.bind(n, 85368)) : Promise.resolve()]);
                                     return o && await o.load(e.default), t ? i.Viewer : i.Editor
                                 }));
                                 var t, o
                             }));
 
-                        function p() {
-                            l("change", u.invoke("getMarkdown"))
+                        function f() {
+                            u("change", d.invoke("getMarkdown"))
                         }
-                        return () => (0, i.h)(c.value, {
-                            ref: e => u = e,
+                        return () => (0, i.h)(p.value, {
+                            ref: e => d = e,
                             props: {
                                 initialValue: e.initialValue,
                                 initialEditType: "wysiwyg",
-                                options: d
+                                options: c
                             },
                             on: {
-                                blur: p
+                                blur: f
                             }
                         })
                     }
                 });
-            var l = n(87444),
-                u = n(78357);
-            const d = (0, l.defineFieldComponent)({
-                readonly: e => () => (0, i.h)(o, {
+            var u = n(87444),
+                d = n(78357);
+            const c = (0, u.defineFieldComponent)({
+                readonly: e => () => (0, i.h)(l, {
                     props: {
                         readOnly: !0,
                         initialValue: e.value
                     }
                 }),
                 edit: (e, t) => {
                     let {
                         emit: n
                     } = t;
-                    return () => (0, i.h)(o, {
+                    return () => (0, i.h)(l, {
                         props: {
                             readOnly: !1,
                             initialValue: e.value
                         },
                         on: {
                             change: t => {
                                 t !== e.value && n("set-value", t)
                             }
                         }
                     })
                 }
             });
-            class c extends u.N {
+            class p extends d.N {
                 static get mixins() {
-                    return [d]
+                    return [c]
                 }
             }
         },
         2907: function(e, t, n) {
             n.r(t), n.d(t, {
                 HTMLField: function() {
-                    return $
+                    return U
                 },
                 HTMLFieldContentReadonly: function() {
                     return x
                 },
                 HTMLFieldMixin: function() {
-                    return q
+                    return $
                 },
                 PlainTextField: function() {
                     return R
                 },
                 PlainTextFieldContentReadonly: function() {
                     return k
                 },
                 StringArrayField: function() {
-                    return L
+                    return j
                 },
                 StringField: function() {
                     return F.Z
                 },
                 TextAreaField: function() {
                     return M.N
                 },
@@ -13077,39 +13100,39 @@
                 TextAreaFieldContentReadonly: function() {
                     return A.Z
                 },
                 TextAreaFieldMixin: function() {
                     return M.i
                 },
                 TextParagraphField: function() {
-                    return H
+                    return G
                 },
                 TextParagraphFieldContentReadonly: function() {
                     return E
                 },
                 masked: function() {
-                    return G
+                    return z
                 },
                 phone: function() {
                     return i
                 },
                 replaceHashLinks: function() {
-                    return j
+                    return q
                 },
                 wysiwyg: function() {
-                    return ae
+                    return re
                 }
             });
             var i = {};
             n.r(i), n.d(i, {
                 PhoneField: function() {
-                    return se
+                    return ae
                 },
                 PhoneFieldMixin: function() {
-                    return ne
+                    return ie
                 }
             });
             var s = function() {
                 var e = this;
                 return (0, e._self._c)("div", {
                     staticClass: "scroll html_content",
                     domProps: {
@@ -13163,15 +13186,15 @@
                                 whiteSpace: "pre-wrap"
                             }
                         }
                     }
                 },
                 k = (0, w.Z)(S, C, [], !1, null, null, null).exports,
                 F = n(29073),
-                Z = n(24389),
+                Z = n(83943),
                 A = n(82509),
                 T = function() {
                     var e = this,
                         t = e._self._c;
                     return t("div", {
                         class: e.classes,
                         style: e.styles
@@ -13226,21 +13249,22 @@
                 N = (0, w.Z)(B, O, [], !1, null, null, null).exports;
             const D = (0, V.defineComponent)({
                 components: {
                     field_list_view: N
                 },
                 extends: M.i
             });
-            class L extends M.N {
+            class j extends M.N {
                 static get mixins() {
                     return [D]
                 }
             }
+            var L = n(4942);
 
-            function j(e, t) {
+            function q(e, t) {
                 const n = e.querySelectorAll("a"),
                     i = document.location.href,
                     s = document.location.origin;
                 for (const e of n)
                     if (e.href && -1 !== e.href.search(s)) {
                         if (!e.href.includes(i)) {
                             const n = e.href.match(/#([A-z0-9,-]+)$/),
@@ -13254,55 +13278,58 @@
                                 continue
                             }
                             e.href = i + t + e.href.split(s)[1]
                         }
                     } else e.setAttribute("target", "_blank"), e.setAttribute("rel", "noreferrer")
             }
             n(33948);
-            const q = (0, V.defineComponent)({
+            const $ = (0, V.defineComponent)({
                 components: {
                     field_content_readonly: x
                 },
                 extends: M.i,
                 data() {
                     return {
                         link_path: ""
                     }
                 },
                 mounted() {
                     this.setLinksInsideField()
                 },
                 methods: {
                     setLinksInsideField() {
-                        j(this.$el, this.link_path)
+                        q(this.$el, this.link_path)
                     }
                 }
             });
-            class $ extends M.N {
+            class U extends M.N {
+                constructor() {
+                    super(...arguments), (0, L.Z)(this, "allowedMediaTypes", ["text/html"])
+                }
                 static get mixins() {
-                    return [q]
+                    return [$]
                 }
             }
-            const U = (0, V.defineComponent)({
+            const H = (0, V.defineComponent)({
                 components: {
                     field_content_readonly: E,
                     field_content_edit: Z.Z
                 }
             });
-            class H extends a.BaseField {
+            class G extends a.BaseField {
                 toRepresent(e) {
                     let t = this.getValue(e);
                     return void 0 === t && (t = this.options.default), "object" == typeof t ? Array.isArray(t) ? t.join(" ") : JSON.stringify(t) : t
                 }
                 static get mixins() {
-                    return [U]
+                    return [H]
                 }
             }
-            var G = n(33364),
-                z = (n(31672), n(2490), n(59461), function() {
+            var z = n(33364),
+                W = (n(31672), n(2490), n(59461), function() {
                     var e = this,
                         t = e._self._c;
                     return t("div", {
                         staticClass: "input-group"
                     }, [e._m(0), e._v(" "), t(e.countryCodeField.component, {
                         tag: "component",
                         staticClass: "code-selector",
@@ -13348,18 +13375,18 @@
                         nativeOn: {
                             click: function(t) {
                                 return e.clearValue.apply(null, arguments)
                             }
                         }
                     })], 1)
                 });
-            z._withStripped = !0;
-            var W = {
+            W._withStripped = !0;
+            var Q = {
                     name: "PhoneFieldContentEdit",
-                    mixins: [G.MaskedFieldEdit],
+                    mixins: [z.MaskedFieldEdit],
                     data() {
                         const e = this.$app.fieldsResolver.resolveField({
                             name: "countryCode",
                             type: "string",
                             enum: this.field.codes.slice().reverse(),
                             required: !0
                         });
@@ -13385,28 +13412,28 @@
                     },
                     methods: {
                         beforeSet(e) {
                             return e ? this.countryCode + e : null
                         }
                     }
                 },
-                Q = n(84821),
-                Y = {};
-            Y.styleTagTransform = _(), Y.setAttributes = h(), Y.insert = p().bind(null, "head"), Y.domAPI = d(), Y.insertStyleElement = v(), l()(Q.Z, Y), Q.Z && Q.Z.locals && Q.Z.locals;
-            var K = (0, w.Z)(W, z, [function() {
+                Y = n(84821),
+                K = {};
+            K.styleTagTransform = _(), K.setAttributes = h(), K.insert = p().bind(null, "head"), K.domAPI = d(), K.insertStyleElement = v(), l()(Y.Z, K), Y.Z && Y.Z.locals && Y.Z.locals;
+            var J = (0, w.Z)(Q, W, [function() {
                     var e = this._self._c;
                     return e("div", {
                         staticClass: "input-group-prepend"
                     }, [e("div", {
                         staticClass: "input-group-text"
                     }, [e("span", [this._v("+")])])])
                 }], !1, null, "ab1545bc", null).exports,
-                J = n(53973),
-                X = n(59198);
-            const ee = {
+                X = n(53973),
+                ee = n(59198);
+            const te = {
                     data() {
                         return {
                             justNumber: "",
                             countryCode: "1"
                         }
                     },
                     mounted() {
@@ -13420,61 +13447,61 @@
                                 if (!t) return this.setValue(null), "";
                                 this.countryCode = t
                             }
                             return e.slice(this.countryCode.length)
                         }
                     }
                 },
-                te = {
-                    mixins: [ee],
+                ne = {
+                    mixins: [te],
                     computed: {
                         preparedValue() {
-                            return this.justNumber ? "+".concat(this.countryCode, " ").concat(J.ZP.pipe(this.justNumber, this.field.mask)) : ""
+                            return this.justNumber ? "+".concat(this.countryCode, " ").concat(X.ZP.pipe(this.justNumber, this.field.mask)) : ""
                         }
                     }
                 },
-                ne = {
-                    mixins: [G.MaskedFieldMixin],
+                ie = {
+                    mixins: [z.MaskedFieldMixin],
                     components: {
                         field_content_edit: {
-                            mixins: [K, ee]
+                            mixins: [J, te]
                         },
                         field_content_readonly: {
-                            mixins: [a.BaseFieldContentReadonlyMixin, te]
+                            mixins: [a.BaseFieldContentReadonlyMixin, ne]
                         },
                         field_list_view: {
-                            mixins: [a.BaseFieldListView, te]
+                            mixins: [a.BaseFieldListView, ne]
                         }
                     }
                 },
-                ie = ["5999", "4779", "1939", "1876", "1869", "1868", "1849", "1829", "1809", "1787", "1784", "1767", "1758", "1721", "1684", "1671", "1670", "1664", "1649", "1473", "1441", "1345", "1340", "1284", "1268", "1264", "1246", "1242", "998", "996", "995", "994", "993", "992", "977", "976", "975", "974", "973", "972", "971", "970", "968", "967", "966", "965", "964", "963", "962", "961", "960", "886", "880", "856", "855", "853", "852", "850", "692", "691", "690", "689", "688", "687", "686", "685", "683", "682", "681", "680", "679", "678", "677", "676", "675", "674", "673", "672", "670", "598", "597", "596", "595", "594", "593", "592", "591", "590", "509", "508", "507", "506", "505", "504", "503", "502", "501", "500", "423", "421", "420", "389", "387", "386", "385", "383", "382", "381", "380", "379", "378", "377", "376", "375", "374", "373", "372", "371", "370", "359", "358", "357", "356", "355", "354", "353", "352", "351", "350", "299", "298", "297", "291", "269", "268", "267", "266", "265", "264", "263", "262", "261", "260", "258", "257", "256", "255", "254", "253", "252", "251", "250", "249", "248", "246", "245", "244", "243", "242", "241", "240", "239", "238", "237", "236", "235", "234", "233", "232", "231", "230", "229", "228", "227", "226", "225", "224", "223", "222", "221", "220", "218", "216", "213", "212", "211", "98", "95", "94", "93", "92", "91", "90", "86", "84", "82", "81", "77", "76", "66", "65", "64", "63", "62", "61", "60", "58", "57", "56", "55", "54", "53", "52", "51", "49", "48", "47", "46", "45", "44", "43", "41", "40", "39", "36", "34", "33", "32", "31", "30", "27", "20", "7", "1"];
-            class se extends G.MaskedField {
+                se = ["5999", "4779", "1939", "1876", "1869", "1868", "1849", "1829", "1809", "1787", "1784", "1767", "1758", "1721", "1684", "1671", "1670", "1664", "1649", "1473", "1441", "1345", "1340", "1284", "1268", "1264", "1246", "1242", "998", "996", "995", "994", "993", "992", "977", "976", "975", "974", "973", "972", "971", "970", "968", "967", "966", "965", "964", "963", "962", "961", "960", "886", "880", "856", "855", "853", "852", "850", "692", "691", "690", "689", "688", "687", "686", "685", "683", "682", "681", "680", "679", "678", "677", "676", "675", "674", "673", "672", "670", "598", "597", "596", "595", "594", "593", "592", "591", "590", "509", "508", "507", "506", "505", "504", "503", "502", "501", "500", "423", "421", "420", "389", "387", "386", "385", "383", "382", "381", "380", "379", "378", "377", "376", "375", "374", "373", "372", "371", "370", "359", "358", "357", "356", "355", "354", "353", "352", "351", "350", "299", "298", "297", "291", "269", "268", "267", "266", "265", "264", "263", "262", "261", "260", "258", "257", "256", "255", "254", "253", "252", "251", "250", "249", "248", "246", "245", "244", "243", "242", "241", "240", "239", "238", "237", "236", "235", "234", "233", "232", "231", "230", "229", "228", "227", "226", "225", "224", "223", "222", "221", "220", "218", "216", "213", "212", "211", "98", "95", "94", "93", "92", "91", "90", "86", "84", "82", "81", "77", "76", "66", "65", "64", "63", "62", "61", "60", "58", "57", "56", "55", "54", "53", "52", "51", "49", "48", "47", "46", "45", "44", "43", "41", "40", "39", "36", "34", "33", "32", "31", "30", "27", "20", "7", "1"];
+            class ae extends z.MaskedField {
                 constructor(e) {
-                    e[X.X_OPTIONS] = {
+                    e[ee.X_OPTIONS] = {
                         mask: {
                             mask: [{
                                 mask: "(000) 000-000"
                             }, {
                                 mask: "(000) 000-00-00"
                             }, {
                                 mask: "(000) 000-000-00"
                             }, {
                                 mask: "(000) 000-000-000"
                             }]
                         }
-                    }, super(e), this.codes = ie
+                    }, super(e), this.codes = se
                 }
                 static get mixins() {
-                    return [ne]
+                    return [ie]
                 }
                 getEmptyValue() {
                     return null
                 }
             }
-            var ae = n(48058)
+            var re = n(48058)
         },
         71829: function(e, t, n) {
             n.d(t, {
                 D: function() {
                     return o
                 }
             });
@@ -13816,16 +13843,16 @@
                 }
                 static shouldUseBulk(e) {
                     return !this.nonBulkMethods || !this.nonBulkMethods.includes(e)
                 }
                 shouldUseBulk(e) {
                     return this._c.shouldUseBulk(e)
                 }
-                async update(e, t) {
-                    return (await this._queryset.update(this, [this], e, t))[0]
+                async update(e, t, n) {
+                    return (await this._queryset.update(this, [this], e, t, n))[0]
                 }
                 async delete() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
                     return (await this._queryset.delete([this], e))[0]
                 }
                 async create() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "post";
@@ -13942,19 +13969,19 @@
                 guiQuerySets: function() {
                     return _
                 }
             }), n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(33948);
             var i = n(4942),
                 s = (n(21703), n(15306), n(88449), n(2490), n(59849), n(57640), n(9924), n(99244), n(74326), n(82499), n(19755)),
                 a = n.n(s),
-                r = n(29526),
-                o = n(8366),
-                l = n(59198),
-                u = n(40151),
-                d = n(70538);
+                r = n(70538),
+                o = n(29526),
+                l = n(8366),
+                u = n(59198),
+                d = n(40151);
             class c extends Error {
                 constructor(e, t) {
                     super("Wrong model used. Expected: ".concat(e.name, ". Actual: ").concat(t._name, "."))
                 }
                 static checkModel(e, t) {
                     if (!(t instanceof e)) throw new c(e, t)
                 }
@@ -13983,21 +14010,21 @@
                     })
                 }
                 getModelClass(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 1;
                     const n = this.models[e];
                     if (n) return Array.isArray(n) ? n[t] : n;
                     switch (e) {
-                        case l.RequestTypes.PARTIAL_UPDATE:
-                        case l.RequestTypes.UPDATE:
-                            return this.getModelClass(l.RequestTypes.CREATE, t);
-                        case l.RequestTypes.CREATE:
-                            return this.getModelClass(l.RequestTypes.RETRIEVE, t);
-                        case l.RequestTypes.RETRIEVE:
-                            return this.getModelClass(l.RequestTypes.LIST, t)
+                        case u.RequestTypes.PARTIAL_UPDATE:
+                        case u.RequestTypes.UPDATE:
+                            return this.getModelClass(u.RequestTypes.CREATE, t);
+                        case u.RequestTypes.CREATE:
+                            return this.getModelClass(u.RequestTypes.RETRIEVE, t);
+                        case u.RequestTypes.RETRIEVE:
+                            return this.getModelClass(u.RequestTypes.LIST, t)
                     }
                     return null
                 }
                 getRequestModelClass(e) {
                     const t = this.getModelClass(e, 0);
                     if (!t) throw new Error("No request model for operation ".concat(e, " on path ").concat(this.url));
                     return t
@@ -14010,15 +14037,15 @@
                 getDataType() {
                     return this.url.replace(/^\/|\/$/g, "").split("/")
                 }
                 clone() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                     const n = Object.create(Object.getPrototypeOf(this));
-                    return a().extend(!0, n, this), Object.assign(n, e), t || n.clearCache(), Object.freeze((0, d.readonly)(n))
+                    return a().extend(!0, n, this), Object.assign(n, e), t || n.clearCache(), Object.freeze((0, r.readonly)(n))
                 }
                 copy() {
                     let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.clone(e, !0)
                 }
                 all() {
                     return this.clone()
@@ -14039,164 +14066,169 @@
                     return [...this.getDataType(), e]
                 }
                 async get(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                     if (t) return this.clone({
                         pathParamsValues: t
                     }).get(e);
-                    const n = this.getResponseModelClass(l.RequestTypes.RETRIEVE);
+                    const n = this.getResponseModelClass(u.RequestTypes.RETRIEVE);
                     let i;
                     if (void 0 === e) i = await this.getOne();
                     else {
                         const t = await this.execute({
-                            method: l.HttpMethods.GET,
+                            method: u.HttpMethods.GET,
                             path: this._getDetailPath(e),
                             query: this.query,
-                            useBulk: n.shouldUseBulk(l.HttpMethods.GET)
+                            useBulk: n.shouldUseBulk(u.HttpMethods.GET)
                         });
                         i = new n(t.data, this), i._response = t
                     }
-                    return this.prefetchEnabled && await (0, u.Z)([i], {
+                    return this.prefetchEnabled && await (0, d.Z)([i], {
                         isPrefetch: !0
                     }), i
                 }
                 async getOne(e) {
                     if (e) return this.clone({
                         pathParamsValues: e
                     }).getOne();
-                    const t = this.getResponseModelClass(l.RequestTypes.RETRIEVE),
-                        n = t === this.getResponseModelClass(l.RequestTypes.LIST);
-                    if (t.shouldUseBulk(l.HttpMethods.GET) && !n) {
+                    const t = this.getResponseModelClass(u.RequestTypes.RETRIEVE),
+                        n = t === this.getResponseModelClass(u.RequestTypes.LIST);
+                    if (t.shouldUseBulk(u.HttpMethods.GET) && !n) {
                         const e = t.pkField.name,
                             n = this.getDataType(),
-                            i = await r.apiConnector.sendBulk([{
-                                method: l.HttpMethods.GET,
+                            i = await o.apiConnector.sendBulk([{
+                                method: u.HttpMethods.GET,
                                 path: n,
-                                query: (0, l.makeQueryString)({
+                                query: (0, u.makeQueryString)({
                                     ...this.query,
                                     limit: 1
                                 }, !0)
                             }, {
-                                method: l.HttpMethods.GET,
+                                method: u.HttpMethods.GET,
                                 path: [...n, "<<0[data][results][0][".concat(e, "]>>")]
                             }]);
                         if (i[0].data.count > 1) throw new Error("More then one entity found");
-                        0 === i[0].data.count && r.APIResponse.throwStatusError(404, {
+                        0 === i[0].data.count && o.APIResponse.throwStatusError(404, {
                             detail: "No ".concat(t.name, " matches the given query.")
                         });
                         const s = new t(i[1].data, this);
-                        return this.prefetchEnabled && await (0, u.Z)([s], {
+                        return this.prefetchEnabled && await (0, d.Z)([s], {
                             isPrefetch: !0
                         }), s
                     } {
                         var i;
                         const e = await this.filter({
                             limit: 1
                         }).items();
                         if (null !== (i = e.extra) && void 0 !== i && i.count && e.extra.count > 1) throw new Error("More then one entity found");
-                        if (!e.length) throw new r.StatusError(404, "Not Found");
+                        if (!e.length) throw new o.StatusError(404, "Not Found");
                         return n ? e[0] : this.get(e[0].getPkValue())
                     }
                 }
                 async items() {
                     let e = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0],
                         t = arguments.length > 1 ? arguments[1] : void 0;
                     if (t) return this.clone({
                         pathParamsValues: t
                     }).items(e);
                     if (!e && this.cache) return this.cache;
-                    const n = this.getResponseModelClass(l.RequestTypes.LIST),
+                    const n = this.getResponseModelClass(u.RequestTypes.LIST),
                         i = await this.execute({
-                            method: l.HttpMethods.GET,
+                            method: u.HttpMethods.GET,
                             path: this.getDataType(),
                             query: this.query,
-                            useBulk: n.shouldUseBulk(l.HttpMethods.GET)
+                            useBulk: n.shouldUseBulk(u.HttpMethods.GET)
                         }),
-                        s = (0, o.createInstancesList)(i.data.results.map((e => new n(e, this.clone()))));
+                        s = (0, l.createInstancesList)(i.data.results.map((e => new n(e, this.clone()))));
                     for (const e of Object.keys(i.data)) p.includes(e) || (s.extra[e] = i.data[e]);
-                    return s.total = s.extra.count, this.prefetchEnabled && await (0, u.Z)(s, {
+                    return s.total = s.extra.count, this.prefetchEnabled && await (0, d.Z)(s, {
                         isPrefetch: !0
                     }), s
                 }
                 _getCreateBulkPath(e) {
                     return [...this.getDataType(), "<<0[data][".concat(e, "]>>")]
                 }
                 async create(e) {
-                    let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : l.HttpMethods.POST;
-                    const n = this.getRequestModelClass(l.RequestTypes.CREATE);
+                    let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : u.HttpMethods.POST;
+                    const n = this.getRequestModelClass(u.RequestTypes.CREATE);
                     c.checkModel(n, e);
-                    const i = this.getResponseModelClass(l.RequestTypes.RETRIEVE),
-                        s = n === this.getResponseModelClass(l.RequestTypes.RETRIEVE),
+                    const i = this.getResponseModelClass(u.RequestTypes.RETRIEVE),
+                        s = n === this.getResponseModelClass(u.RequestTypes.RETRIEVE),
                         a = this.getDataType();
-                    if (!s && n.shouldUseBulk(t) && i.shouldUseBulk(l.HttpMethods.GET)) {
+                    if (!s && n.shouldUseBulk(t) && i.shouldUseBulk(u.HttpMethods.GET)) {
                         const n = i.pkField.name,
-                            s = await r.apiConnector.sendBulk([{
+                            s = await o.apiConnector.sendBulk([{
                                 method: t,
                                 path: a,
                                 data: e._getInnerData()
                             }, {
-                                method: l.HttpMethods.GET,
+                                method: u.HttpMethods.GET,
                                 path: this._getCreateBulkPath(n)
                             }]);
-                        return r.APIResponse.checkStatus(s[0].status, s[0].data), new i(s[1].data, this)
+                        return o.APIResponse.checkStatus(s[0].status, s[0].data), new i(s[1].data, this)
                     } {
                         const i = await this.execute({
                                 method: t,
                                 data: e,
                                 path: a,
                                 query: this.query,
                                 useBulk: n.shouldUseBulk(t)
                             }),
                             r = new n(i.data, this);
                         return s ? r : this.get(r.getPkValue())
                     }
                 }
                 async update(e, t) {
-                    let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : l.HttpMethods.PATCH,
-                        i = arguments.length > 3 ? arguments[3] : void 0;
+                    let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : u.HttpMethods.PATCH,
+                        i = arguments.length > 3 ? arguments[3] : void 0,
+                        s = arguments.length > 4 ? arguments[4] : void 0;
                     void 0 === t && (t = await this.items());
-                    const s = n === l.HttpMethods.PATCH ? l.RequestTypes.PARTIAL_UPDATE : l.RequestTypes.UPDATE,
-                        a = this.getRequestModelClass(s),
-                        o = this.getResponseModelClass(l.RequestTypes.RETRIEVE);
-                    c.checkModel(a, e);
-                    const u = a === o,
-                        d = e._getInnerData(i);
-                    if (!u && a.shouldUseBulk(n) && o.shouldUseBulk(l.HttpMethods.GET)) {
+                    const a = n === u.HttpMethods.PATCH ? u.RequestTypes.PARTIAL_UPDATE : u.RequestTypes.UPDATE,
+                        r = this.getRequestModelClass(a),
+                        l = this.getResponseModelClass(u.RequestTypes.RETRIEVE);
+                    c.checkModel(r, e);
+                    const d = r === l,
+                        p = e._getInnerData(i);
+                    if (!d && r.shouldUseBulk(n) && l.shouldUseBulk(u.HttpMethods.GET)) {
                         const e = t.flatMap((e => {
                             const t = this._getDetailPath(e.getPkValue());
                             return [{
                                 method: n,
                                 path: t,
-                                data: d
+                                data: p
                             }, {
-                                method: l.HttpMethods.GET,
+                                method: u.HttpMethods.GET,
                                 path: t
                             }]
                         }));
-                        return (await r.apiConnector.sendBulk(e, l.BulkType.TRANSACTIONAL)).map((e => new r.APIResponse(e))).filter(((e, t) => t % 2 != 0)).map((e => new o(e.data, this)))
+                        return (await o.apiConnector.sendBulk(e, u.BulkType.TRANSACTIONAL)).map((e => new o.APIResponse(e))).filter(((e, t) => t % 2 != 0)).map((e => new l(e.data, this)))
                     }
                     return Promise.all(t.map((async e => {
-                        const t = await this.execute({
+                        var t;
+                        const i = {};
+                        !s && null !== (t = e._response) && void 0 !== t && t.headers.ETag && (i["If-Match"] = e._response.headers.ETag);
+                        const a = await this.execute({
                             method: n,
-                            data: d,
+                            data: p,
                             path: this._getDetailPath(e.getPkValue()),
                             query: this.query,
-                            useBulk: a.shouldUseBulk(n)
+                            useBulk: r.shouldUseBulk(n),
+                            headers: Object.keys(i).length > 0 ? i : void 0
                         });
-                        return new a(t.data, this)
+                        return new r(a.data, this)
                     })))
                 }
                 async delete(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1];
                     void 0 === e && (e = await this.items());
-                    const n = this.getModelClass(l.RequestTypes.RETRIEVE, 1),
-                        i = !n || n.shouldUseBulk(l.HttpMethods.DELETE),
+                    const n = this.getModelClass(u.RequestTypes.RETRIEVE, 1),
+                        i = !n || n.shouldUseBulk(u.HttpMethods.DELETE),
                         s = {};
                     return t && (s.HTTP_X_Purge_Nested = String(t)), Promise.all(e.map((e => this.execute({
-                        method: l.HttpMethods.DELETE,
+                        method: u.HttpMethods.DELETE,
                         path: this._getDetailPath(e.getPkValue()),
                         headers: s,
                         useBulk: i
                     }))))
                 }
                 _isModelInstance(e) {
                     return Boolean(e && "_getInnerData" in e && "function" == typeof e._getInnerData)
@@ -14211,25 +14243,25 @@
                             path: e.path,
                             query: e.query,
                             headers: e.headers,
                             version: e.version
                         };
                     if (void 0 !== n) {
                         const e = i ? n._getInnerData() : n;
-                        return s ? r.apiConnector.makeRequest({
+                        return s ? o.apiConnector.makeRequest({
                             ...a,
                             useBulk: s,
                             data: e
-                        }) : r.apiConnector.makeRequest({
+                        }) : o.apiConnector.makeRequest({
                             ...a,
                             useBulk: s,
-                            data: (0, l.objectToFormData)(e)
+                            data: (0, u.objectToFormData)(e)
                         })
                     }
-                    return r.apiConnector.makeRequest({
+                    return o.apiConnector.makeRequest({
                         ...a,
                         useBulk: s
                     })
                 }
                 clearCache() {
                     this.cache = void 0
                 }
@@ -14255,42 +14287,42 @@
                 }
             }
             class v {
                 constructor(e) {
                     this.viewsTree = e
                 }
                 findQuerySetForNested(e, t) {
-                    const n = this.viewsTree.root.get((0, l.pathToArray)(t)),
+                    const n = this.viewsTree.root.get((0, u.pathToArray)(t)),
                         i = this.viewsTree.findInParentsDeep(n, this._getMatcher(e));
                     if (i) return i;
                     throw new Error("Cannot find model ".concat(e, " for path ").concat(t))
                 }
                 findQuerySet(e) {
                     let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                     const n = this._getMatcher(e);
                     if (!t) return this.viewsTree.findInFirstLevel(n);
-                    const i = "/" === t ? this.viewsTree.root : this.viewsTree.root.get((0, l.pathToArray)(t));
+                    const i = "/" === t ? this.viewsTree.root : this.viewsTree.root.get((0, u.pathToArray)(t));
                     if (!i) throw new Error("View does not exists in tree: " + t);
                     const s = n(i.view) || this.viewsTree.findInChildren(i, n) || this.viewsTree.findInNeighbourPaths(i, n) || this.viewsTree.findInParentsDeep(i, n);
                     if (s) return s;
                     throw new Error("Cannot find model ".concat(e, " for path ").concat(t))
                 }
                 _getMatcher(e) {
                     return t => {
                         var n, i;
-                        if (t.type !== l.ViewTypes.LIST) return;
-                        const s = null === (n = t) || void 0 === n || null === (i = n.objects) || void 0 === i ? void 0 : i.getResponseModelClass(l.RequestTypes.LIST);
+                        if (t.type !== u.ViewTypes.LIST) return;
+                        const s = null === (n = t) || void 0 === n || null === (i = n.objects) || void 0 === i ? void 0 : i.getResponseModelClass(u.RequestTypes.LIST);
                         return s && s.name === e ? (t.deepNestedParentView && (t = t.deepNestedParentView), t.objects.clone()) : null
                     }
                 }
             }
             const g = new Map([
                     ["QuerySet", f]
                 ]),
-                _ = (0, l.mapToObjectProxy)(g)
+                _ = (0, u.mapToObjectProxy)(g)
         },
         79806: function(e, t, n) {
             n.r(t), n.d(t, {
                 RouterConstructor: function() {
                     return r
                 }
             });
@@ -14609,33 +14641,34 @@
                                     })
                                 }
                                 return t.at(-1).link = "", t.length > 4 ? [...t.slice(0, 2), {
                                     name: "..."
                                 }, ...t.slice(-2)] : t
                             }))
                         })(),
+                        u = (0, r.getApp)(),
                         {
-                            start: u,
-                            stop: d,
-                            setCallback: c,
-                            setPk: p
+                            start: d,
+                            stop: c,
+                            setCallback: p,
+                            setPk: f
                         } = (0, a.useAutoUpdate)({
                             callback: () => {
                                 var t, n, i;
                                 return null !== (t = null === (n = (i = (0, r.getApp)().store.page).updateData) || void 0 === n ? void 0 : n.call(i)) && void 0 !== t ? t : Promise.reject("Please provide auto update callback or disable auto update for view ".concat(e.path))
                             },
                             pk: () => {
                                 var e, t;
                                 return null === (e = (t = (0, r.getApp)().store.page).getAutoUpdatePk) || void 0 === e ? void 0 : e.call(t)
                             },
                             labels: e.subscriptionLabels || void 0,
                             startOnMount: e.autoupdate
                         });
 
-                    function f() {
+                    function h() {
                         t.value = !1, i.value = !0
                     }
                     return {
                         ...m({
                             view: e,
                             isListItem: !1
                         }),
@@ -14644,25 +14677,34 @@
                         error: n,
                         response: i,
                         title: o,
                         breadcrumbs: l,
                         initLoading: function() {
                             n.value = null, i.value = null, t.value = !0
                         },
-                        setLoadingSuccessful: f,
+                        setLoadingSuccessful: h,
                         setLoadingError: function(e) {
                             t.value = !1, n.value = e
                         },
                         fetchData: function() {
-                            return f(), Promise.resolve()
+                            return h(), Promise.resolve()
                         },
-                        startAutoUpdate: u,
-                        stopAutoUpdate: d,
-                        setAutoUpdateCallback: c,
-                        setAutoUpdatePk: p
+                        startAutoUpdate: d,
+                        stopAutoUpdate: c,
+                        setAutoUpdateCallback: p,
+                        setAutoUpdatePk: f,
+                        executeMainAction: function() {
+                            if (e.mainAction) {
+                                const t = e.actions.get(e.mainAction);
+                                t && u.actions.execute({
+                                    action: t,
+                                    instance: u.store.page.instance
+                                })
+                            }
+                        }
                     }
                 },
                 g = e => {
                     const t = (0, s.ref)([]),
                         n = (0, s.computed)((() => e.value.every((e => t.value.includes(e.getPkValue())))));
 
                     function i(e) {
@@ -15460,36 +15502,41 @@
                     });
                     const n = (0, p.getApp)();
                     return {
                         ...t,
                         setInstance: function(e) {
                             e instanceof t.model.value || (e = new t.model.value(void 0, null, e)), t.setInstance(e)
                         },
-                        save: async function() {
+                        save: async function i(s) {
                             try {
                                 t.validateAndSetInstanceData()
                             } catch (e) {
                                 return n.error_handler.defineErrorAndShow(e), void(e instanceof m.ModelValidationError && (t.fieldsErrors.value = e.toFieldsErrors()))
                             }
-                            const i = t.instance.value;
-                            if (!i) return;
+                            const a = t.instance.value;
+                            if (!a) return;
                             t.loading.value = !0;
-                            const s = i.getViewFieldString() || i.getPkValue() || "";
+                            const r = a.getViewFieldString() || a.getPkValue() || "";
                             try {
                                 const n = e.params.method,
-                                    a = await i.update(n, e.isPartial ? Array.from(t.instance.value.sandbox.changedFields) : void 0);
-                                return i.sandbox.markUnchanged(), t.fieldsErrors.value = {}, v.guiPopUp.success(g.a.t(v.pop_up_msg.instance.success.save, [s, e.name])), e.isDeepNested ? (0, p.openPage)((0, l.B8)()) : (0, p.openPage)({
+                                    i = await a.update(n, !e.isPartial || null != s && s.allFields ? void 0 : Array.from(t.instance.value.sandbox.changedFields), null == s ? void 0 : s.ignoreEtag);
+                                return a.sandbox.markUnchanged(), t.fieldsErrors.value = {}, v.guiPopUp.success(g.a.t(v.pop_up_msg.instance.success.save, [r, e.name])), e.isDeepNested ? (0, p.openPage)((0, l.B8)()) : (0, p.openPage)({
                                     path: (0, l.B8)(),
                                     params: {
-                                        providedInstance: a
+                                        providedInstance: i
                                     }
                                 })
                             } catch (e) {
-                                const s = i.parseModelError(e.data);
-                                s && (t.fieldsErrors.value = s.toFieldsErrors()), n.error_handler.showError(g.a.t(v.pop_up_msg.instance.error.save, [n.error_handler.errorToString(s || e)]))
+                                const s = a.parseModelError(e.data);
+                                if (s) t.fieldsErrors.value = s.toFieldsErrors();
+                                else if (e && "object" == typeof e && "status" in e && 412 === e.status) return confirm(g.a.ts("The data has been changed on the server. Do you want to overwrite it?")) ? i({
+                                    ignoreEtag: !0,
+                                    allFields: !0
+                                }) : void 0;
+                                n.error_handler.showError(g.a.t(v.pop_up_msg.instance.error.save, [n.error_handler.errorToString(s || e)]))
                             } finally {
                                 t.loading.value = !1
                             }
                         },
                         reload: function() {
                             return t.fetchData({
                                 forceSet: !0
@@ -15649,15 +15696,15 @@
                 createUniqueIdGenerator: function() {
                     return Z
                 },
                 deepEqual: function() {
                     return a.vZ
                 },
                 defaultDownloadResponseHandler: function() {
-                    return j
+                    return L
                 },
                 deferredPromise: function() {
                     return w
                 },
                 downloadBase64File: function() {
                     return a.lS
                 },
@@ -15820,15 +15867,15 @@
                 saveAllSettings: function() {
                     return P
                 },
                 saveHideMenuSettings: function() {
                     return a.Wu
                 },
                 setFileDownloadHandler: function() {
-                    return L
+                    return j
                 },
                 sleep: function() {
                     return a._v
                 },
                 sliceLongString: function() {
                     return a.TB
                 },
@@ -16075,20 +16122,20 @@
 
             function N(e) {
                 const t = e.headers.get("Content-Disposition");
                 if (!t) return "";
                 const n = /filename="(.+)"/.exec(t);
                 return n ? n[1] : ""
             }
-            let D = j;
+            let D = L;
 
-            function L(e) {
+            function j(e) {
                 D = e
             }
-            async function j(e) {
+            async function L(e) {
                 const t = await e.blob(),
                     n = URL.createObjectURL(t),
                     i = N(e),
                     s = document.createElement("a");
                 s.href = n, i && (s.download = i), document.body.appendChild(s), s.click(), document.body.removeChild(s), setTimeout((() => URL.revokeObjectURL(n)), 100)
             }
 
@@ -16127,15 +16174,15 @@
                 }
             });
             var i = n(4942),
                 s = (n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(33948), n(15306), n(57658), n(67476)),
                 a = n(70538),
                 r = n(59198),
                 o = n(51916),
-                l = n(89045),
+                l = n(68217),
                 u = n(56039),
                 d = n(56716);
             const c = (0, r.createUniqueIdGenerator)();
             class p {
                 constructor(e, t) {
                     var n, s, a, r, o;
                     let l = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [];
@@ -16295,30 +16342,30 @@
                     }
                     return super.getTitle(e)
                 }
             }(0, i.Z)(v, "viewType", "PAGE");
             class g extends m {
                 constructor(e, t) {
                     var n;
-                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "nestedAllowAppend", void 0), (0, i.Z)(this, "multiActions", new Map), (0, i.Z)(this, "listView", null), (0, i.Z)(this, "hideReadonlyFields", !0), this.nestedAllowAppend = null !== (n = e["x-allow-append"]) && void 0 !== n && n
+                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "nestedAllowAppend", void 0), (0, i.Z)(this, "multiActions", new Map), (0, i.Z)(this, "listView", null), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "mainAction", "save"), this.nestedAllowAppend = null !== (n = e["x-allow-append"]) && void 0 !== n && n
                 }
                 _createStore() {
                     return this._createStoreWithHook((0, u.createNewViewStore)(this))
                 }
                 getRoutePath() {
                     var e;
                     return (0, r.joinPaths)(null === (e = this.parent) || void 0 === e ? void 0 : e.getRoutePath(), (0, r.pathToArray)(this.path).last)
                 }
                 getModel() {
                     return this.objects.getResponseModelClass(r.RequestTypes.CREATE)
                 }
             }(0, i.Z)(g, "viewType", "PAGE_NEW");
             class _ extends m {
                 constructor(e, t) {
-                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "parent", null), (0, i.Z)(this, "isEditStyleOnly", !1), (0, i.Z)(this, "isPartial", void 0), (0, i.Z)(this, "hideReadonlyFields", !0), this.isPartial = e.method === r.HttpMethods.PATCH
+                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "parent", null), (0, i.Z)(this, "isEditStyleOnly", !1), (0, i.Z)(this, "isPartial", void 0), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "mainAction", "save"), this.isPartial = e.method === r.HttpMethods.PATCH
                 }
                 _createStore() {
                     return this._createStoreWithHook((0, u.createEditViewStore)(this))
                 }
                 getRoutePath() {
                     var e;
                     return this.isDeepNested ? (0, r.joinPaths)(null === (e = this.parent) || void 0 === e ? void 0 : e.getRoutePath(), (0, r.pathToArray)(this.path).last) : super.getRoutePath()
@@ -16326,15 +16373,15 @@
                 getModel() {
                     return this.objects.getRequestModelClass(this.isPartial ? r.RequestTypes.PARTIAL_UPDATE : r.RequestTypes.UPDATE)
                 }
             }(0, i.Z)(_, "viewType", "PAGE_EDIT");
             class b extends m {
                 constructor(e, t) {
                     var n;
-                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "method", void 0), (0, i.Z)(this, "action", void 0), (0, i.Z)(this, "isFileResponse", void 0), this.method = e.method, this.action = e.action, this.isFileResponse = null !== (n = e.isFileResponse) && void 0 !== n && n
+                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "method", void 0), (0, i.Z)(this, "action", void 0), (0, i.Z)(this, "isFileResponse", void 0), (0, i.Z)(this, "mainAction", "execute"), this.method = e.method, this.action = e.action, this.isFileResponse = null !== (n = e.isFileResponse) && void 0 !== n && n
                 }
                 _createStore() {
                     return this._createStoreWithHook((0, u.createActionViewStore)(this))
                 }
                 getRoutePath() {
                     var e;
                     return (0, r.joinPaths)(null === (e = this.parent) || void 0 === e ? void 0 : e.getRoutePath(), (0, r.pathToArray)(this.path).last)
@@ -16552,14 +16599,21 @@
         65977: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".status[data-v-721f3f24]{font-size:70px;font-weight:200;color:#ffc107 !important;margin-right:10px;margin-bottom:0}.margin-0[data-v-721f3f24]{margin:0}", ""]), t.Z = r
         },
+        26571: function(e, t, n) {
+            var i = n(8081),
+                s = n.n(i),
+                a = n(23645),
+                r = n.n(a)()(s());
+            r.push([e.id, ".file-input-btn[data-v-a9fc330c]{position:relative;cursor:pointer}.file-input-btn .hidden-input[data-v-a9fc330c]{position:absolute;top:0px;left:0px;height:0;width:0;opacity:0;overflow:hidden}", ""]), t.Z = r
+        },
         14279: function(e, t, n) {
             var i = n(8081),
                 s = n.n(i),
                 a = n(23645),
                 r = n.n(a)()(s());
             r.push([e.id, ".popover-symbol[data-v-c9bddf36]{color:var(--info);display:inline-block;width:1em;text-align:center;cursor:pointer;outline:none}", ""]), t.Z = r
         },
@@ -20680,15 +20734,15 @@
                 C = n(44589),
                 S = n.n(C),
                 k = n(15853),
                 F = {};
             F.styleTagTransform = S(), F.setAttributes = y(), F.insert = _().bind(null, "head"), F.domAPI = v(), F.insertStyleElement = x(), h()(k.Z, F), k.Z && k.Z.locals && k.Z.locals;
             var Z = (0, d.Z)(p, i, [], !1, null, null, null).exports
         },
-        89045: function(e, t, n) {
+        68217: function(e, t, n) {
             n.d(t, {
                 Z: function() {
                     return p
                 }
             });
             var i = function() {
                 var e = this,
@@ -20697,30 +20751,40 @@
                 return t("div", {
                     staticClass: "row"
                 }, [n.beforeFieldsGroups ? t(n.beforeFieldsGroups, {
                     tag: "component",
                     attrs: {
                         page: n.self
                     }
-                }) : e._e(), e._v(" "), t("div", {
-                    class: e.view.wrapperClasses
+                }) : e._e(), e._v(" "), t("form", {
+                    class: e.view.wrapperClasses,
+                    on: {
+                        submit: function(e) {
+                            return e.preventDefault(), n.store.executeMainAction.apply(null, arguments)
+                        }
+                    }
                 }, [n.response ? t(n.ModelFields, {
                     attrs: {
                         data: n.sandbox,
                         model: n.model,
                         editable: !n.readOnly,
                         "fields-errors": n.fieldsErrors,
                         "hide-read-only": n.hideReadOnly,
                         "require-value-on-clear": n.requireValueOnClear,
                         "fields-groups": n.fieldsGroups
                     },
                     on: {
                         "set-value": n.store.setFieldValue
                     }
-                }) : e._e()], 1), e._v(" "), n.afterFieldsGroups ? t(n.afterFieldsGroups, {
+                }) : e._e(), e._v(" "), t("input", {
+                    attrs: {
+                        type: "submit",
+                        hidden: ""
+                    }
+                })], 1), e._v(" "), n.afterFieldsGroups ? t(n.afterFieldsGroups, {
                     tag: "component",
                     attrs: {
                         page: n.self
                     }
                 }) : e._e()], 1)
             };
             i._withStripped = !0;
@@ -21345,40 +21409,105 @@
                 b = n(44589),
                 y = n.n(b),
                 w = n(70779),
                 x = {};
             x.styleTagTransform = y(), x.setAttributes = v(), x.insert = h().bind(null, "head"), x.domAPI = p(), x.insertStyleElement = _(), d()(w.Z, x), w.Z && w.Z.locals && w.Z.locals;
             var C = (0, n(51900).Z)(l, i, [], !1, null, "ee46bd7e", null).exports
         },
-        24389: function(e, t, n) {
+        83943: function(e, t, n) {
             n.d(t, {
                 Z: function() {
-                    return c
+                    return A
                 }
             });
             var i = function() {
                 var e = this,
                     t = e._self._c;
-                return e._self._setupProxy, t("FieldTextarea", {
+                return e._self._setupProxy, t("div", [t("FileInputButton", {
+                    staticStyle: {
+                        "margin-bottom": "0.5rem"
+                    },
+                    attrs: {
+                        accept: e.accept
+                    },
+                    nativeOn: {
+                        input: function(t) {
+                            return e.handleFileInput.apply(null, arguments)
+                        }
+                    }
+                }), e._v(" "), t("FieldTextarea", {
                     attrs: {
                         value: e.value || "",
                         field: e.field
                     },
                     on: {
                         input: function(t) {
                             return e.$emit("set-value", t)
                         }
                     }
-                })
+                })], 1)
             };
             i._withStripped = !0;
             var s = n(70538),
                 a = n(87444),
                 r = function() {
                     var e = this,
+                        t = e._self._c;
+                    return e._self._setupProxy, t("label", {
+                        staticClass: "btn btn-default file-input-btn"
+                    }, [t("input", {
+                        staticClass: "hidden-input",
+                        attrs: {
+                            type: "file",
+                            multiple: e.multiple,
+                            accept: e.accept
+                        }
+                    }), e._v(" "), t("i", {
+                        class: e.iconClass
+                    }), e._v(" "), t("span", {
+                        staticClass: "sr-only"
+                    }, [e._v(e._s(e.$t("Select file")))])])
+                };
+            r._withStripped = !0;
+            var o = (0, s.defineComponent)({
+                    __name: "FileInputButton",
+                    props: {
+                        multiple: {
+                            type: Boolean
+                        },
+                        accept: null,
+                        iconClass: {
+                            default: "fas fa-file-alt"
+                        }
+                    },
+                    setup(e) {
+                        return {
+                            __sfc: !0
+                        }
+                    }
+                }),
+                l = n(93379),
+                u = n.n(l),
+                d = n(7795),
+                c = n.n(d),
+                p = n(90569),
+                f = n.n(p),
+                h = n(3565),
+                m = n.n(h),
+                v = n(19216),
+                g = n.n(v),
+                _ = n(44589),
+                b = n.n(_),
+                y = n(26571),
+                w = {};
+            w.styleTagTransform = b(), w.setAttributes = m(), w.insert = f().bind(null, "head"), w.domAPI = c(), w.insertStyleElement = g(), u()(y.Z, w), y.Z && y.Z.locals && y.Z.locals;
+            var x = n(51900),
+                C = (0, x.Z)(o, r, [], !1, null, "a9fc330c", null).exports,
+                S = function() {
+                    var e = this,
                         t = e._self._c,
                         n = e._self._setupProxy;
                     return t("div", {
                         staticClass: "input-group"
                     }, [t("textarea", e._b({
                         staticClass: "form-control",
                         staticStyle: {
@@ -21392,16 +21521,16 @@
                             value: e.value || ""
                         },
                         on: {
                             input: n.handleInput
                         }
                     }, "textarea", n.attrs, !1))])
                 };
-            r._withStripped = !0;
-            var o = (0, s.defineComponent)({
+            S._withStripped = !0;
+            var k = (0, s.defineComponent)({
                     __name: "FieldTextarea",
                     props: {
                         field: null,
                         value: null,
                         rows: {
                             default: 3
                         },
@@ -21423,24 +21552,44 @@
                             attrs: r,
                             handleInput: function(e) {
                                 n("input", e.target.value)
                             }
                         }
                     }
                 }),
-                l = n(51900),
-                u = (0, l.Z)(o, r, [], !1, null, null, null).exports,
-                d = (0, s.defineComponent)({
+                F = (0, x.Z)(k, S, [], !1, null, null, null).exports,
+                Z = (0, s.defineComponent)({
                     components: {
-                        FieldTextarea: u
+                        FieldTextarea: F,
+                        FileInputButton: C
                     },
                     props: a.FieldEditPropsDef,
-                    emits: a.FieldEditEmitsDef
+                    emits: a.FieldEditEmitsDef,
+                    setup(e, t) {
+                        let {
+                            emit: n
+                        } = t;
+                        return {
+                            accept: (0, s.computed)((() => {
+                                var t;
+                                if ("allowedMediaTypes" in e.field) return null === (t = e.field.allowedMediaTypes) || void 0 === t ? void 0 : t.join(",")
+                            })),
+                            handleFileInput: async function(e) {
+                                var t;
+                                const i = e.target,
+                                    s = (null !== (t = i.files) && void 0 !== t ? t : [])[0];
+                                if (s) {
+                                    const e = await s.text();
+                                    n("set-value", e), i.value = ""
+                                }
+                            }
+                        }
+                    }
                 }),
-                c = (0, l.Z)(d, i, [], !1, null, null, null).exports
+                A = (0, x.Z)(Z, i, [], !1, null, null, null).exports
         },
         82509: function(e, t, n) {
             n.d(t, {
                 Z: function() {
                     return a
                 }
             });
```

### Comparing `vstutils-5.5.9/vstutils/static/img/anonymous.png` & `vstutils-5.6.0a1/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/static_files.py` & `vstutils-5.6.0a1/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/tasks.py` & `vstutils-5.6.0a1/vstutils/tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.apps import apps
 
 from .utils import import_class, send_template_email_handler, Lock, translate as _
 
 celery_app: Celery = import_class(
     settings.WORKER_OPTIONS['app'].replace(':', '.')  # type: ignore
 )
+notificator = apps.get_app_config('vstutils_api').module.notificator_class([])
 
 
 class TaskMeta(type):
     def __new__(mcs, name, bases, attrs, uniq=None):
         task_class = super(TaskMeta, mcs).__new__(mcs, name, bases, attrs)
         task_class.run = mcs.get_notificator_decorator(task_class.run)
 
@@ -32,20 +33,16 @@
     @staticmethod
     def get_notificator_decorator(func):
         if getattr(func, '__notify_wrapped__', False):
             return func
 
         @wraps(func, assigned=WRAPPER_ASSIGNMENTS+('__notify_wrapped__',))
         def wrapper(self, *args, **kwargs):
-            notifier = (
-                getattr(self, '__notifier__', None) or
-                apps.get_app_config('vstutils_api').module.notificator_class([])
-            )
-            with notifier:
-                self.__notifier__ = notifier
+            with notificator:
+                self.__notifier__ = notificator
                 result = func(self, *args, **kwargs)
             self.__notifier__ = None
             return result
 
         wrapper.__notify_wrapped__ = True
         return wrapper
```

### Comparing `vstutils-5.5.9/vstutils/templates/auth/base.html` & `vstutils-5.6.0a1/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/auth/language_selector.html` & `vstutils-5.6.0a1/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/auth/tfa.html` & `vstutils-5.6.0a1/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/base.html` & `vstutils-5.6.0a1/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/gui/base.html` & `vstutils-5.6.0a1/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/gui/offline.html` & `vstutils-5.6.0a1/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/gui/service-worker.js` & `vstutils-5.6.0a1/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/package.json.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/setup.py.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/test.py.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.6.0a1/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/registration/confirm_email.html` & `vstutils-5.6.0a1/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.6.0a1/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.6.0a1/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/registration/user_registration.html` & `vstutils-5.6.0a1/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/rest_framework/admin.html` & `vstutils-5.6.0a1/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.6.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.6.0a1/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templatetags/request_static.py` & `vstutils-5.6.0a1/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templatetags/translation.py` & `vstutils-5.6.0a1/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.6.0a1/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.6.0a1/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/templatetags/vstconfigs.py` & `vstutils-5.6.0a1/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/tests.py` & `vstutils-5.6.0a1/vstutils/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,18 +350,21 @@
         if relogin:
             client = self._login()
         else:
             client = self.client
 
         request_handler = getattr(client, rtype)
 
-        if kwargs.get("data", False):
-            if isinstance(kwargs["data"], str):
+        if data := kwargs.get("data", False):
+            if isinstance(data, str):
                 kwargs["content_type"] = "application/json"
-            elif isinstance(kwargs["data"], (bytes, bytearray)):
+            elif isinstance(data, (dict, list, tuple, set)):
+                kwargs["content_type"] = "application/json"
+                kwargs['data'] = json.dumps(data)
+            elif isinstance(data, (bytes, bytearray)):
                 kwargs["content_type"] = "application/msgpack"
 
         if 'content_type' in kwargs and kwargs["content_type"].startswith('application/'):
             kwargs['HTTP_ACCEPT'] = kwargs["content_type"]
 
         kwargs['code'] = code or self.std_codes.get(rtype, 200)
```

### Comparing `vstutils-5.5.9/vstutils/tools.py` & `vstutils-5.6.0a1/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/translations/cn.py` & `vstutils-5.6.0a1/vstutils/translations/cn.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,14 +247,15 @@
     'Link': '链接',
 
     # csv
     'Actions': '行動',
     'Index': '指數',
     'Download with headers': '帶標題下載',
     'Changes you made may not be saved.': '您所做的更改可能不会保存。',
+    'The data has been changed on the server. Do you want to overwrite it?': '服务器上的数据已更改。 您想覆盖它们吗？',
 }
 
 SERVER_TRANSLATION = {
     # field's validation
     "value is not a valid list": "值不是有效列表",
     "value is not a valid JSON": "值不是有效的 JSON",
     "key {missing_key} is missing": "缺少密钥 {missing_key}",
```

### Comparing `vstutils-5.5.9/vstutils/translations/ru.py` & `vstutils-5.6.0a1/vstutils/translations/ru.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     'An error occurred during <b>{0}</b>. Error details:<br>{1}': 'Во время запуска действия <b>{0}</b> произошла ошибка. Подробнее:<br>{1}',
     'Link': 'Ссылка',
     # csv
     'Actions': 'Действия',
     'Index': 'Индекс',
     'Download with headers': 'Скачать с заголовками столбцов',
     'Changes you made may not be saved.': 'Внесенные изменения могут быть не сохранены.',
+    'The data has been changed on the server. Do you want to overwrite it?': 'Данные были изменены на сервере. Вы хотите их перезаписать?',
 }
 
 SERVER_TRANSLATION = {
     # field's validation
     "value is not a valid list": "значение не является допустимым списком",
     "value is not a valid JSON": "значение не является допустимым JSON",
     "key {missing_key} is missing": "ключ {missing_key} отсутствует",
```

### Comparing `vstutils-5.5.9/vstutils/translations/vi.py` & `vstutils-5.6.0a1/vstutils/translations/vi.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,15 @@
     'Link': 'Liên kết',
 
     # csv
     'Actions': 'Hành động',
     'Index': 'Mục lục',
     'Download with headers': 'Tải xuống với tiêu đề',
     'Changes you made may not be saved.': 'Những thay đổi bạn đã thực hiện có thể không được lưu.',
+    'The data has been changed on the server. Do you want to overwrite it?': 'Dữ liệu đã được thay đổi trên máy chủ. Bạn có muốn ghi đè lên chúng?',
 }
 
 SERVER_TRANSLATION = {
     # field's validation
     "value is not a valid list": "giá trị không phải là một danh sách hợp lệ",
     "value is not a valid JSON": "giá trị không phải là JSON hợp lệ",
     "key {missing_key} is missing": "khóa {missing_key} bị thiếu",
```

### Comparing `vstutils-5.5.9/vstutils/urls.py` & `vstutils-5.6.0a1/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/utils.py` & `vstutils-5.6.0a1/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/web.ini` & `vstutils-5.6.0a1/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils/wsgi.py` & `vstutils-5.6.0a1/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.9/vstutils.egg-info/PKG-INFO` & `vstutils-5.6.0a1/vstutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.9
+Version: 5.6.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.9/vstutils.egg-info/SOURCES.txt` & `vstutils-5.6.0a1/vstutils.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
 vstutils/management/__init__.py
 vstutils/management/commands/__init__.py
 vstutils/management/commands/_base.py
 vstutils/management/commands/celery_inspect.py
 vstutils/management/commands/dockermigrate.py
 vstutils/management/commands/dockerrun.py
 vstutils/management/commands/newproject.py
+vstutils/management/commands/rpc_worker.py
 vstutils/management/commands/run_task.py
 vstutils/management/commands/runrpc.py
 vstutils/management/commands/runserver.py
 vstutils/management/commands/web.py
 vstutils/models/__init__.py
 vstutils/models/base.py
 vstutils/models/cent_notify.py
```

### Comparing `vstutils-5.5.9/vstutils.egg-info/requires.txt` & `vstutils-5.6.0a1/vstutils.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,84 +1,84 @@
 django~=4.2.2
 configparser~=5.3.0
-configparserc~=1.4.1
-Markdown==3.4.1
+configparserc~=1.4.2
+Markdown~=3.4.3
 django-environ~=0.10.0
 djangorestframework~=3.14.0
 drf-yasg==1.21.6
 django-filter==23.2
 django-crispy-forms~=1.14.0
 drf_orjson_renderer~=1.7.1
 ormsgpack==1.2.6
-pyyaml~=5.4.1
+pyyaml~=6.0.0
 uvicorn~=0.22.0
 pyuwsgi==2.0.21
-fastapi~=0.98.0
+fastapi==0.100.0
 aiofiles~=23.1.0
 cent~=4.1.0
 PyJWT~=2.7.0
 jsmin~=3.0.1
 django-htmlmin~=0.11.0
 pyotp~=2.8.0
 django-storages[libcloud]==1.13.2
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
-sphinxcontrib-httpdomain~=1.8.0
+sphinxcontrib-httpdomain~=1.8.1
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.23.0
-sphinx-rtd-theme~=1.2.1
+sphinx-rtd-theme~=1.2.2
 
 [all]
 coverage~=7.2.7
 fakeldap==0.6.1
 tblib~=1.7.0
 beautifulsoup4~=4.12.2
 httpx~=0.24.1
-celery[redis]==5.3.0
+celery[redis]==5.3.1
 django-celery-beat~=2.5.0
 python-ldap==3.4.0
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
-sphinxcontrib-httpdomain~=1.8.0
+sphinxcontrib-httpdomain~=1.8.1
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.23.0
-sphinx-rtd-theme~=1.2.1
-redis[hiredis]~=4.5.5
+sphinx-rtd-theme~=1.2.2
+redis[hiredis]~=4.6.0
 Pillow~=9.4.0
 django-storages[boto3,libcloud]==1.13.2
 
 [boto3]
 django-storages[boto3,libcloud]==1.13.2
 
 [doc]
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
-sphinxcontrib-httpdomain~=1.8.0
+sphinxcontrib-httpdomain~=1.8.1
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.23.0
-sphinx-rtd-theme~=1.2.1
+sphinx-rtd-theme~=1.2.2
 
 [ldap]
 python-ldap==3.4.0
 
 [pil]
 Pillow~=9.4.0
 
 [prod]
-redis[hiredis]~=4.5.5
+redis[hiredis]~=4.6.0
 
 [rpc]
-celery[redis]==5.3.0
+celery[redis]==5.3.1
 django-celery-beat~=2.5.0
 
 [sqs]
-celery[redis]==5.3.0
+celery[redis]==5.3.1
 django-celery-beat~=2.5.0
 pycurl~=7.45.2
 
 [stubs]
 django-stubs[compatible-mypy]~=4.2.1
 djangorestframework-stubs[compatible-mypy]~=3.14.1
 celery-stubs~=0.1.3
```

