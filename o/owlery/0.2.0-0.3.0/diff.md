# Comparing `tmp/owlery-0.2.0.tar.gz` & `tmp/owlery-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlery-0.2.0.tar", last modified: Wed Jun  7 07:08:32 2023, max compression
+gzip compressed data, was "owlery-0.3.0.tar", last modified: Sat Jul 15 19:43:35 2023, max compression
```

## Comparing `owlery-0.2.0.tar` & `owlery-0.3.0.tar`

### file list

```diff
@@ -1,111 +1,116 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      143 2023-05-07 18:40:41.000000 owlery-0.2.0/.dockerignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/FUNDING.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)      762 2023-05-11 17:05:09.000000 owlery-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      431 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/release.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.github/workflows/scripts/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1289 2023-05-07 18:40:41.000000 owlery-0.2.0/.github/workflows/scripts/release.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2750 2023-06-07 07:00:18.000000 owlery-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2821 2023-05-07 18:40:41.000000 owlery-0.2.0/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)     1139 2023-05-07 18:40:41.000000 owlery-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      352 2023-05-07 18:40:41.000000 owlery-0.2.0/.readthedocs.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/.vscode/
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-05-07 18:40:41.000000 owlery-0.2.0/.vscode/settings.json
--rw-r--r--   0 michael   (1000) michael   (1000)      996 2023-06-07 07:05:35.000000 owlery-0.2.0/CHANGELOG.md
--rw-r--r--   0 michael   (1000) michael   (1000)     4718 2023-05-07 18:40:41.000000 owlery-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)     2179 2023-05-07 18:40:41.000000 owlery-0.2.0/Dockerfile
--rw-r--r--   0 michael   (1000) michael   (1000)     1084 2023-05-07 18:40:41.000000 owlery-0.2.0/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-07 18:40:41.000000 owlery-0.2.0/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-06-07 07:08:32.166276 owlery-0.2.0/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      697 2023-06-06 22:32:50.000000 owlery-0.2.0/README.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/changelog.d/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/changelog.d/.gitkeep
--rw-r--r--   0 michael   (1000) michael   (1000)      309 2023-05-07 18:40:41.000000 owlery-0.2.0/changelog.d/template.md
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.156276 owlery-0.2.0/dev/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-07 18:40:41.000000 owlery-0.2.0/dev/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      726 2023-06-07 07:07:49.000000 owlery-0.2.0/docker-compose.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-06-07 07:07:49.000000 owlery-0.2.0/docs/api.rst
--rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/changelog.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     4252 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/contributing.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     4247 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/getting-started.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      929 2023-06-07 07:07:49.000000 owlery-0.2.0/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/installation.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/integrations/
--rw-r--r--   0 michael   (1000) michael   (1000)     3591 2023-05-13 13:03:59.000000 owlery-0.2.0/docs/integrations/flask.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-07 19:55:42.000000 owlery-0.2.0/docs/license.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/make.bat
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/recipes/
--rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-05-13 07:31:46.000000 owlery-0.2.0/docs/recipes/celery.rst
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-13 12:58:30.000000 owlery-0.2.0/docs/recipes/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-06 21:59:54.000000 owlery-0.2.0/docs/recipes/rq.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/services/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/docs/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/imap.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3288 2023-05-07 20:01:11.000000 owlery-0.2.0/docs/services/email/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/pop3.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      195 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/email/smtp.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/services/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3624 2023-06-06 22:32:50.000000 owlery-0.2.0/docs/signals.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      170 2023-05-07 18:40:41.000000 owlery-0.2.0/docs/spelling-wordlist.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-06-07 06:25:49.000000 owlery-0.2.0/dovecot.conf
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/
--rw-r--r--   0 michael   (1000) michael   (1000)      398 2023-05-07 18:40:41.000000 owlery-0.2.0/owlery/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      160 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery/_version.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2962 2023-05-11 17:05:09.000000 owlery-0.2.0/owlery/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/owlery/py.typed
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/
--rw-r--r--   0 michael   (1000) michael   (1000)    20845 2023-06-07 06:48:04.000000 owlery-0.2.0/owlery/services/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)    16763 2023-06-07 06:56:34.000000 owlery-0.2.0/owlery/services/email/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2812 2023-06-07 06:41:44.000000 owlery-0.2.0/owlery/services/email/imap.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2673 2023-06-07 06:59:11.000000 owlery-0.2.0/owlery/services/email/pop3.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2644 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/email/smtp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1907 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/misc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/mms/
--rw-r--r--   0 michael   (1000) michael   (1000)     4341 2023-06-07 06:59:57.000000 owlery-0.2.0/owlery/services/mms/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3090 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/mms/twilio.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/sms/
--rw-r--r--   0 michael   (1000) michael   (1000)     3882 2023-06-07 06:48:04.000000 owlery-0.2.0/owlery/services/sms/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2551 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/sms/twilio.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1614 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/services/twilio.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery/services/whatsapp/
--rw-r--r--   0 michael   (1000) michael   (1000)     5366 2023-06-07 06:59:57.000000 owlery-0.2.0/owlery/services/whatsapp/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3955 2023-06-07 07:05:29.000000 owlery-0.2.0/owlery/services/whatsapp/twilio.py
--rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-06 22:32:50.000000 owlery-0.2.0/owlery/signals.py
--rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-05-13 12:55:55.000000 owlery-0.2.0/owlery/utils.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/owlery.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     2022 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       43 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      422 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-06-07 07:08:32.000000 owlery-0.2.0/owlery.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     4489 2023-05-07 19:41:49.000000 owlery-0.2.0/pyproject.toml
--rw-r--r--   0 michael   (1000) michael   (1000)       97 2023-06-06 22:32:50.000000 owlery-0.2.0/requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-06-07 07:08:32.166276 owlery-0.2.0/setup.cfg
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      576 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)       87 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/services/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/__init__.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/tests/services/email/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/email/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      123 2023-05-07 18:40:41.000000 owlery-0.2.0/tests/services/email/conftest.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3259 2023-06-07 06:47:46.000000 owlery-0.2.0/tests/services/email/test_imap.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3384 2023-06-07 06:47:54.000000 owlery-0.2.0/tests/services/email/test_pop3.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2413 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/email/test_smtp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9564 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_manager.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1191 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/services/test_service.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-06 22:32:50.000000 owlery-0.2.0/tests/test_signals.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1918 2023-05-07 18:40:41.000000 owlery-0.2.0/tox.ini
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-07 07:08:32.166276 owlery-0.2.0/typing/
--rw-r--r--   0 michael   (1000) michael   (1000)       62 2023-05-07 18:40:41.000000 owlery-0.2.0/typing/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      143 2023-05-07 18:40:41.000000 owlery-0.3.0/.dockerignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.3.0/.github/FUNDING.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)      431 2023-05-07 18:40:41.000000 owlery-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      319 2023-05-07 18:40:41.000000 owlery-0.3.0/.github/workflows/release.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/.github/workflows/scripts/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1289 2023-05-07 18:40:41.000000 owlery-0.3.0/.github/workflows/scripts/release.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3770 2023-06-12 17:03:02.000000 owlery-0.3.0/.github/workflows/tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2821 2023-05-07 18:40:41.000000 owlery-0.3.0/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)     1139 2023-05-07 18:40:41.000000 owlery-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      352 2023-05-07 18:40:41.000000 owlery-0.3.0/.readthedocs.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/.vscode/
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2023-05-07 18:40:41.000000 owlery-0.3.0/.vscode/settings.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2023-07-15 19:39:48.000000 owlery-0.3.0/CHANGELOG.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     4877 2023-06-09 18:35:37.000000 owlery-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     2179 2023-05-07 18:40:41.000000 owlery-0.3.0/Dockerfile
+-rw-r--r--   0 michael   (1000) michael   (1000)     1084 2023-05-07 18:40:41.000000 owlery-0.3.0/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      255 2023-05-07 18:40:41.000000 owlery-0.3.0/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-07-15 19:43:35.478534 owlery-0.3.0/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      697 2023-06-06 22:32:50.000000 owlery-0.3.0/README.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/changelog.d/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.3.0/changelog.d/.gitkeep
+-rw-r--r--   0 michael   (1000) michael   (1000)      309 2023-05-07 18:40:41.000000 owlery-0.3.0/changelog.d/template.md
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/dev/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2023-05-07 18:40:41.000000 owlery-0.3.0/dev/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)      291 2023-07-15 19:43:29.000000 owlery-0.3.0/docs/api.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)       31 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/changelog.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     4254 2023-06-12 17:03:02.000000 owlery-0.3.0/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/contributing.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     4247 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/getting-started.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      929 2023-07-15 19:43:29.000000 owlery-0.3.0/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     1131 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/installation.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/docs/integrations/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3591 2023-05-13 13:03:59.000000 owlery-0.3.0/docs/integrations/flask.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      401 2023-05-07 19:55:42.000000 owlery-0.3.0/docs/license.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      765 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/make.bat
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/docs/recipes/
+-rw-r--r--   0 michael   (1000) michael   (1000)      810 2023-05-13 07:31:46.000000 owlery-0.3.0/docs/recipes/celery.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-13 12:58:30.000000 owlery-0.3.0/docs/recipes/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2023-06-06 21:59:54.000000 owlery-0.3.0/docs/recipes/rq.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/docs/services/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.468534 owlery-0.3.0/docs/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/services/email/imap.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3288 2023-05-07 20:01:11.000000 owlery-0.3.0/docs/services/email/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/services/email/pop3.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      195 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/services/email/smtp.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2023-05-07 18:40:41.000000 owlery-0.3.0/docs/services/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3626 2023-06-09 18:35:37.000000 owlery-0.3.0/docs/signals.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      193 2023-06-09 18:35:37.000000 owlery-0.3.0/docs/spelling-wordlist.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/
+-rw-r--r--   0 michael   (1000) michael   (1000)      398 2023-05-07 18:40:41.000000 owlery-0.3.0/owlery/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      160 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery/_version.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2962 2023-05-11 17:05:09.000000 owlery-0.3.0/owlery/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.3.0/owlery/py.typed
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/
+-rw-r--r--   0 michael   (1000) michael   (1000)    20199 2023-06-12 17:03:02.000000 owlery-0.3.0/owlery/services/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)    17124 2023-06-12 17:03:02.000000 owlery-0.3.0/owlery/services/email/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4204 2023-06-11 14:09:07.000000 owlery-0.3.0/owlery/services/email/html.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2812 2023-06-07 06:41:44.000000 owlery-0.3.0/owlery/services/email/imap.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2673 2023-06-07 06:59:11.000000 owlery-0.3.0/owlery/services/email/pop3.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2644 2023-06-06 22:32:50.000000 owlery-0.3.0/owlery/services/email/smtp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1907 2023-06-06 22:32:50.000000 owlery-0.3.0/owlery/services/misc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/mms/
+-rw-r--r--   0 michael   (1000) michael   (1000)     4341 2023-06-07 06:59:57.000000 owlery-0.3.0/owlery/services/mms/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3092 2023-06-09 18:35:37.000000 owlery-0.3.0/owlery/services/mms/twilio.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1379 2023-06-10 13:20:22.000000 owlery-0.3.0/owlery/services/reddit.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/sms/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3882 2023-06-07 06:48:04.000000 owlery-0.3.0/owlery/services/sms/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3061 2023-06-08 22:14:11.000000 owlery-0.3.0/owlery/services/sms/gsmmodem.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2553 2023-06-09 18:35:37.000000 owlery-0.3.0/owlery/services/sms/twilio.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1614 2023-06-06 22:32:50.000000 owlery-0.3.0/owlery/services/twilio.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/voice/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2466 2023-06-09 21:56:03.000000 owlery-0.3.0/owlery/services/voice/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery/services/whatsapp/
+-rw-r--r--   0 michael   (1000) michael   (1000)     5366 2023-06-07 06:59:57.000000 owlery-0.3.0/owlery/services/whatsapp/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3955 2023-06-07 07:05:29.000000 owlery-0.3.0/owlery/services/whatsapp/twilio.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3668 2023-06-09 17:32:56.000000 owlery-0.3.0/owlery/services/whatsapp/wabp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      469 2023-06-06 22:32:50.000000 owlery-0.3.0/owlery/signals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      225 2023-05-13 12:55:55.000000 owlery-0.3.0/owlery/utils.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/owlery.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1840 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     2162 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       43 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      444 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2023-07-15 19:43:35.000000 owlery-0.3.0/owlery.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     4533 2023-06-09 18:35:37.000000 owlery-0.3.0/pyproject.toml
+-rw-r--r--   0 michael   (1000) michael   (1000)       97 2023-06-06 22:32:50.000000 owlery-0.3.0/requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-07-15 19:43:35.478534 owlery-0.3.0/setup.cfg
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.3.0/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      576 2023-05-07 18:40:41.000000 owlery-0.3.0/tests/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      526 2023-06-12 06:29:25.000000 owlery-0.3.0/tests/docker-compose.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      650 2023-06-07 19:18:34.000000 owlery-0.3.0/tests/dovecot.conf
+-rw-r--r--   0 michael   (1000) michael   (1000)      149 2023-06-12 06:29:47.000000 owlery-0.3.0/tests/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/tests/services/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.3.0/tests/services/__init__.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/tests/services/email/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-07 18:40:41.000000 owlery-0.3.0/tests/services/email/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1313 2023-06-12 17:03:02.000000 owlery-0.3.0/tests/services/email/conftest.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3930 2023-06-12 17:05:57.000000 owlery-0.3.0/tests/services/email/test_imap.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4274 2023-06-12 17:03:26.000000 owlery-0.3.0/tests/services/email/test_pop3.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3158 2023-06-12 06:29:47.000000 owlery-0.3.0/tests/services/email/test_smtp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9564 2023-06-06 22:32:50.000000 owlery-0.3.0/tests/services/test_manager.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1191 2023-06-06 22:32:50.000000 owlery-0.3.0/tests/services/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      793 2023-06-06 22:32:50.000000 owlery-0.3.0/tests/services/test_service.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2023-06-06 22:32:50.000000 owlery-0.3.0/tests/test_signals.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1939 2023-06-09 18:35:37.000000 owlery-0.3.0/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-07-15 19:43:35.478534 owlery-0.3.0/typing/
+-rw-r--r--   0 michael   (1000) michael   (1000)       62 2023-05-07 18:40:41.000000 owlery-0.3.0/typing/requirements.txt
```

### Comparing `owlery-0.2.0/.github/workflows/scripts/release.py` & `owlery-0.3.0/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/.github/workflows/tests.yml` & `owlery-0.3.0/.github/workflows/tests.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,39 @@
 name: Run tests
 on:
   pull_request:
+    branches:
+      - master
+      - features/**
+      - dependabot/**
   push:
+    branches:
+      - master
 
 jobs:
   docs:
     name: Run documentation tests
-    uses: ./.github/workflows/docs.yml
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+      - name: Setup Python 3.10
+        uses: actions/setup-python@v4
+        with:
+          python-version: '3.10'
+      - name: Install dependencies
+        run: |
+          sudo apt-get update
+          sudo apt-get install python3-enchant hunspell-en-gb
+          python -m pip install --upgrade pip setuptools wheel
+          python -m pip install -r docs/requirements.txt
+          python -m pip install tox tox-gh-actions
+      - name: Setup documentation build
+        run: tox r -e docs -vv --notest
+      - name: Run documentation build
+        run: tox r -e docs --skip-pkg-install
   style:
     name: Run linting and style checks
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python 3.11
         uses: actions/setup-python@v4
@@ -25,14 +48,15 @@
         run: tox r -e style -vv --notest
       - name: Run linting checks
         run: tox r -e style --skip-pkg-install
   tests:
     name: Run test suite - ${{ matrix.os }} - ${{ matrix.python }}
     strategy:
       fail-fast: false
+      max-parallel: 2
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python: [
           '3.8',
           '3.9',
           '3.10',
           '3.11',
@@ -58,16 +82,20 @@
           python -m pip install --upgrade pip setuptools wheel
           python -m pip install -r requirements.txt
           python -m pip install -r tests/requirements.txt
           python -m pip install .
           python -m pip install tox-gh-actions
       - name: Setup test suite
         run: tox r -e py${{ matrix.python }} -vv --notest
-      - name: Run test suite
-        run: tox r -e py${{ matrix.python }} --skip-pkg-install
+      - name: Run test suite (with integration tests)
+        if: ${{ matrix.os == 'ubuntu-latest' }}
+        run: tox r -e py${{ matrix.python }} --skip-pkg-install -- --integration --slow
+      - name: Run test suite (w/ointegration tests)
+        if: ${{ matrix.os != 'ubuntu-latest' }}
+        run: tox r -e py${{ matrix.python }} --skip-pkg-install -- --slow
       - name: Publish coveralls.io
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: tox r -e coveralls --skip-pkg-install
   typing:
     name: Run typing checks
     runs-on: ubuntu-latest
```

### Comparing `owlery-0.2.0/.gitignore` & `owlery-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/.pre-commit-config.yaml` & `owlery-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/.vscode/settings.json` & `owlery-0.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/CHANGELOG.md` & `owlery-0.3.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,20 @@
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 This project uses [towncrier](https://towncrier.readthedocs.io/) and the changes for the upcoming release can be found
 in the ``changelog.d/`` folder.
 
 <!-- towncrier release notes start -->
 
+## [0.3.0](https://github.com/COUR4G3/owlery/tree/0.2.0) - 2023-07-15
+
+
+- Refactored various APIs and methods.
+
+
 ## [0.2.0](https://github.com/COUR4G3/owlery/tree/0.2.0) - 2023-06-07
 
 
 ### Features
 
 - Set message status on send, and store exception on error.
 - Support for SMS text, MMS multimedia and WhatsApp messages.
```

### Comparing `owlery-0.2.0/CONTRIBUTING.md` & `owlery-0.3.0/CONTRIBUTING.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # Contributing
 
 Thank you for wanting to contribute to and improve this project!
 
 
+### Note!
+
+While this document outlines the ideal way to contribute to this project, **currently** the project is unstable and
+undergoing rapid development.
+
+
 ## Contents
 
 * [Getting Started](#getting-started)
   * [Issues](#issues)
   * [Pull Requests](#pull-requests)
 * [Running Tests](#running-tests)
 * [Linting and Formatting](#linting-and-formatting)
```

### Comparing `owlery-0.2.0/Dockerfile` & `owlery-0.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/LICENSE` & `owlery-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/PKG-INFO` & `owlery-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlery
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uniform messaging service for Python applications.
 Author-email: Michael de Villiers <michael@devilears.co.za>
 Maintainer-email: Michael de Villiers <michael@devilears.co.za>
 License: MIT
 Project-URL: Homepage, https://github.com/COUR4G3/owlery/
 Project-URL: Documentation, https://owlery-messaging.readthedocs.io/
 Project-URL: Changes, https://owlery-messaging.readthedocs.io/en/latest/changelog.html
```

### Comparing `owlery-0.2.0/README.md` & `owlery-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/Makefile` & `owlery-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/conf.py` & `owlery-0.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "m2r2",
     "sphinx.ext.autodoc",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.intersphinx",
-    "sphinx.ext.linkcode",
+    # "sphinx.ext.linkcode",
     "sphinx.ext.todo",
     "sphinx_click",
     "sphinx_copybutton",
     "sphinx_issues",
     "sphinx-prompt",
     "sphinxcontrib.spelling",
 ]
```

### Comparing `owlery-0.2.0/docs/getting-started.rst` & `owlery-0.3.0/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/index.rst` & `owlery-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/installation.rst` & `owlery-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/integrations/flask.rst` & `owlery-0.3.0/docs/integrations/flask.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/make.bat` & `owlery-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/recipes/celery.rst` & `owlery-0.3.0/docs/recipes/celery.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/recipes/rq.rst` & `owlery-0.3.0/docs/recipes/rq.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/services/email/index.rst` & `owlery-0.3.0/docs/services/email/index.rst`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/docs/signals.rst` & `owlery-0.3.0/docs/signals.rst`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,19 @@
 
     This signal is sent when a message status callback is received. The signal is invoked with the service as
     ``sender``, message identifier as ``message_id``, the status as ``status`` and the raw request data as ``raw``.
 
     Available statuses are:
 
     * ``'pending'`` - message has not yet been sent.
-    * ``'error'`` - an error occured sending the message.
+    * ``'error'`` - an error occurred sending the message.
     * ``'sent'`` - message has been sent.
     * ``'received'`` - message has been received.
     * ``'read'`` - message has been read.
-    * ``'unknown'`` - service returned an unknown state, interogate the ``raw`` data.
+    * ``'unknown'`` - service returned an unknown state, interrogate the ``raw`` data.
 
     Services may support none, some or all of these statuses.
 
     Example subscriber::
 
         from owlery.signals import on_receive_status_callback
```

### Comparing `owlery-0.2.0/dovecot.conf` & `owlery-0.3.0/tests/dovecot.conf`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/exceptions.py` & `owlery-0.3.0/owlery/exceptions.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/__init__.py` & `owlery-0.3.0/owlery/services/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import dataclasses
 import datetime as dt
+import enum
 import logging
-import platform
 import random
 import typing as t
 
 from collections import UserDict, UserList
 from contextlib import contextmanager
+from dataclasses import asdict, dataclass, field
 
-from .. import __version__
 from ..exceptions import (
     ServiceNotRegistered,
     ServiceReceiveCapabilityError,
     ServiceSendCapabilityError,
 )
 from ..signals import (
     on_after_send,
@@ -21,98 +20,100 @@
     on_open_session,
     on_receive_message,
     on_receive_status_callback,
     on_register_service,
     on_unregister_service,
 )
 
-USER_AGENT = (
-    f"owlery/{__version__} "
-    f"{platform.python_implementation()}/{platform.python_version()}"
-)
-
 
-@dataclasses.dataclass
+@dataclass
 class Attachment:
     """A representation of an attachment.
 
-    :param data: Bytes or file-like object contain attachment data.
-    :param mimetype: Mimetype of the attachment, defaults to
-                     ``'application/octet-stream'``.
+    :param data: The attachment data.
+    :param mimetype: The mimetype, default `'application/octet-stream'`.
 
     """
 
     data: t.Union[bytes, t.IO[bytes]]
     mimetype: str = "application/octet-stream"
 
+    def read(self, n: int = -1):
+        if isinstance(self.data, bytes):
+            return self.data
+        return self.data.read(n)
+
+
+class MessageState(enum.Enum):
+    DRAFT = "draft"
+    SENT = "sent"
+    DELIVERED = "delivered"
+    READ = "read"
+    RECEIVED = "received"
+    ERROR = "error"
 
-MessageStatus = t.Literal[
-    "draft",
-    "queued",
-    "sent",
-    "received",
-    "read",
-    "cancelled",
-    "error",
-]
 
-
-@dataclasses.dataclass
+@dataclass
 class Message:
-    """A representation for a received messages.
-
-    :param id: The message unique identifier.
-    :param reply_id: The message identifier this message is replied to.
-    :param date: The date the message was sent/received.
-    :param raw: The raw data response from service.
-    :param status: The message status.
-    :param exc: The exception object if an error occured.
-    :param service: Service to use for sending, replies and fowarding.
+    State = MessageState
 
-    """
+    id: t.Optional[t.Any] = None
+    date: dt.datetime = field(default_factory=dt.datetime.now)
+    raw: t.Optional[t.Any] = None
 
-    id: t.Optional[str] = None
-    reply_id: t.Optional[str] = None
-    date: t.Optional[dt.datetime] = None
-    raw: t.Any = None
-    status: MessageStatus = "draft"
-    exc: t.Optional[Exception] = None
+    state: MessageState = MessageState.DRAFT
     service: t.Optional["Service"] = None
 
     def as_dict(self):
-        return dataclasses.asdict(self)
+        return asdict(self)
+
+    def send(self, service: t.Optional["Service"] = None):
+        """Send the message.
 
-    def send(self, service=None):
+        :param service: The service to use, optional.
+
+        """
         if not service:
             service = self.service
         if not service:
-            raise ValueError("No service to send this message")
+            raise ValueError("No service associated with this message")
 
         return service.send_message(self)
 
 
 class MessageBuilder(UserDict):
-    def __init__(self, dict=None, service=None, **kwargs):
-        self.service = service
+    Message = Message
 
-        super().__init__(dict, **kwargs)
+    def as_message(self):
+        """Return the message as a message object."""
+        return self.Message(**self.data)
 
-    def _replace(self, **kwargs):
-        message = self.copy()
-        message.update(**kwargs)
+    def date(self, date: dt.datetime):
+        """Set a Date on the message."""
+        return self.__class__(**{**self.copy(), "date": date})
 
-        return message
+    def send(self, service: t.Optional["Service"] = None):
+        """Send the message.
 
-    def send(self):
-        service = self.service
+        :param service: The service to use, optional.
+
+        """
         if not service:
-            raise ValueError("No service to send this message")
+            service = self["service"]
+        if not service:
+            raise ValueError("No service associated with this message")
 
         return service.send(**self.data)
 
+    def _replace(self, **kwargs):
+        new = self.copy()
+        new.update(kwargs)
+
+        return new
+
 
 class Outbox(UserList):
     """Outbox containing captured messages.
 
     :param suppress: Do not send messages when released.
 
     """
@@ -173,156 +174,128 @@
         """Whether a connection or session has been started."""
 
         self.suppress = suppress
         """Suppress sending of messages."""
 
         self._media_helper = None
 
-        self._wrap_methods()
-
         self.logger = logging.getLogger(__name__)
 
     def _on_receive_message(self, message):
         message.status = "received"
 
         on_receive_message.send(self, message=message)
 
         self.logger.debug("Received message:\n%r", message)
 
-    def _wrap_close(self):
+    def _wrap_close(self, f):
         # wrap the close method:
         # - dispatch the `on_session_close` signals.
         # - unset the ``opened`` flag.
         # - log a message.
-        original_close = self.close
-
         def close(self):
-            original_close()
+            f()
 
             on_close_session.send(self)
 
             self.logger.debug("Closed session")
 
             self.opened = False
 
-        self.close = close.__get__(self, Service)
-        self._close = original_close
+        return close.__get__(self, Service)
 
-    def _wrap_methods(self):
-        # wrap all methods
-        self._wrap_close()
-        self._wrap_open()
-        self._wrap_receive()
-        self._wrap_receive_webhook()
-        self._wrap_send()
-        self._wrap_status_callback()
-
-    def _wrap_open(self):
+    def _wrap_open(self, f):
         # wrap the open method:
         # - dispatch `on_session_open` signals.
         # - set the ``opened`` flag.
         # - log a message.
 
-        original_open = self.open
-
         def open(self):
-            original_open()
+            f()
 
             on_open_session.send(self)
 
             self.logger.debug("Opened session")
 
             self.opened = True
 
-        self.open = open.__get__(self, Service)
-        self._open = original_open
+        return open.__get__(self, Service)
 
-    def _wrap_receive(self):
+    def _wrap_receive(self, f):
         # wrap the receive method:
         # - dispatch `on_receive_message` signals.
         # - open the connection or session if ``opened`` flag not set.
         # - log messages.
 
-        original_receive = self.receive
-
         def receive(self, **kwargs):
             if not self.opened:
                 self.open()
 
             count = 0
-            for message in original_receive(**kwargs):
+            for message in f(**kwargs):
                 self._on_receive_message(message)
 
                 yield message
                 count += 1
 
             self.logger.info("Received %d messages", count)
 
-        self.receive = receive.__get__(self, Service)
-        self._receive = original_receive
+        return receive.__get__(self, Service)
 
-    def _wrap_receive_webhook(self):
+    def _wrap_receive_webhook(self, f):
         # wrap the receive_webhook method:
         # - dispatch `on_receive_message` signals.
         # - log messages.
 
-        original_receive = self.receive_webhook
-
         def receive_webhook(self, request):
             count = 0
-            for message in original_receive(request):
+            for message in f(request):
                 self._on_receive_message(message)
 
                 yield message
                 count += 1
 
             self.logger.info("Received %d messages from webhook", count)
 
-        self.receive_webhook = receive_webhook.__get__(self, Service)
-        self._receive_webhook = original_receive
+        return receive_webhook.__get__(self, Service)
 
-    def _wrap_send(self):
+    def _wrap_send(self, f):
         # wrap the send method:
         # - dispatch ``on_before_send`` and ``on_after_send`` signals.
         # - open the connection or session if ``opened`` flag not set.
         # - silently discard the message if ``suppress`` flag is set.
         # - log messages.
 
-        original_send = self.send
-
         def send(self, **kwargs):
             on_before_send.send(self, message=kwargs)
 
             if self.suppress:
                 return
 
             if not self.opened:
                 self.open()
 
-            message = original_send(**kwargs)
+            message = f(**kwargs)
 
             on_after_send.send(self, message=message)
 
             # self.logger.info("Sent message %s", message.id)
             # self.logger.debug("%r", message)
 
             return message
 
-        self.send = send.__get__(self, Service)
-        self._send = original_send
+        return send.__get__(self, Service)
 
-    def _wrap_status_callback(self):
+    def _wrap_status_callback(self, f):
         # wrap the status_callback method:
         # - dispatch ``on_receive_status_callback`` signals.
         # - log messages.
 
-        original_status = self.status_callback
-
         def status_callback(self, request):
-            message_id, status, raw = original_status(request)
+            message_id, status, raw = f(request)
             on_receive_status_callback.send(
                 self,
                 message_id=message_id,
                 status=status,
                 raw=raw,
             )
 
@@ -330,26 +303,41 @@
                 "Received message status: %s, %s",
                 message_id,
                 status,
             )
 
             return message_id, status, raw
 
-        self.status_callback = status_callback.__get__(self, Service)
-        self._status_callback = original_status
+        return status_callback.__get__(self, Service)
 
     def __enter__(self):
         if not self.opened:
             self.open()
 
         return self
 
     def __exit__(self, exc_type, exc_value, exc_tb):
         self.close()
 
+    def __getattribute__(self, name):
+        attr = super().__getattribute__(name)
+
+        if name == "close":
+            return self._wrap_close(attr)
+        elif name == "open":
+            return self._wrap_open(attr)
+        elif name == "receive":
+            return self._wrap_receive(attr)
+        elif name == "send":
+            return self._wrap_send(attr)
+        elif name == "status_callback":
+            return self._wrap_status_callback(attr)
+
+        return attr
+
     def close(self):
         """Close a session or connection.
 
         Developers SHOULD implement this method if they need to cleanup or
         disconnect from a session.
 
         This is called at the end of a context manager, otherwise must be
@@ -477,17 +465,15 @@
 
     def send_message(self, message: Message):
         """Send a message from a message object.
 
         :param message: A :class:`Message` message object.
 
         """
-        data = message.as_dict()
-        data["service"] = self
-        return message.send(**data)
+        return self.send(**message.as_dict())
 
     def status_callback(self, request):
         """Receive sent message status callback from a webhook.
 
         Developers SHOULD implement this method.
 
         :param request: The request to parse.
@@ -511,34 +497,33 @@
 
 class ServiceManager(Service):
     """Base class for all service managers."""
 
     can_receive = True
     can_send = True
 
-    _wrap_close = property()
-    _wrap_open = property()
-
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         self.services = {}
         """Registered messaging services."""
 
         self._via = None
 
-        self._update_methods()
+    def __getattribute__(self, name):
+        attr = super(Service, self).__getattribute__(name)
 
-    def _update_methods(self):
-        # update methods for service managers
-        self._update_receive()
-        self._update_send()
+        if name == "receive":
+            return self._receive()
+        elif name == "send":
+            return self._send()
 
-    def _update_receive(self):
-        # update the send method:
+        return attr
+
+    def _receive(self):
         # - dispatch ``on_receive_message`` signal.
         # - select the correct service with ``via`` or receive on all services
 
         def receive(self, limit=100, via=None, **kwargs):
             services = []
             if via:
                 try:
@@ -563,18 +548,17 @@
                     # if service cannot send replies, set to manager
                     if not service.can_send:
                         message.service = self
                     on_receive_message.send(self, message=message)
                     yield message
                     limit -= 1
 
-        self.receive = receive.__get__(self, ServiceManager)
+        return receive.__get__(self, ServiceManager)
 
-    def _update_send(self):
-        # update the send method:: bool = False
+    def _send(self):
         # - dispatch ``on_before_send`` and ``on_after_send`` signals.
         # - silently discard the message if ``suppress`` flag is set.
         # - select the correct service, either default or ``via``.
 
         def send(self, via=None, **kwargs):
             service = None
 
@@ -602,18 +586,15 @@
 
             result = service.send(**kwargs)
 
             on_after_send.send(self, kwargs=kwargs)
 
             return result
 
-        self.send = send.__get__(self, ServiceManager)
-
-    def _wrap_methods(self):
-        return
+        return send.__get__(self, ServiceManager)
 
     def close(self):
         for service in self.services.values():
             if service.opened:
                 service.close()
 
     def ensure_service(
```

### Comparing `owlery-0.2.0/owlery/services/email/imap.py` & `owlery-0.3.0/owlery/services/email/imap.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/email/pop3.py` & `owlery-0.3.0/owlery/services/email/pop3.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/email/smtp.py` & `owlery-0.3.0/owlery/services/email/smtp.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/misc.py` & `owlery-0.3.0/owlery/services/misc.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/mms/__init__.py` & `owlery-0.3.0/owlery/services/mms/__init__.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/mms/twilio.py` & `owlery-0.3.0/owlery/services/mms/twilio.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.client = Client(account_sid, auth_token)
 
         super().__init__(**kwargs)
 
     def receive(self, limit: int = 100, **kwargs):
         messages = self.client.messages.stream(
             to=self.sender_id,
-            date_sent_after=date_sent_after,
+            # date_sent_after=date_sent_after,
             limit=limit,
         )
 
         for message in messages:
             to = message.to
             from_ = message.waid
```

### Comparing `owlery-0.2.0/owlery/services/sms/__init__.py` & `owlery-0.3.0/owlery/services/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/sms/twilio.py` & `owlery-0.3.0/owlery/services/sms/twilio.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         self.client = Client(account_sid, auth_token)
 
         super().__init__(**kwargs)
 
     def receive(self, limit: int = 100, **kwargs):
         messages = self.client.messages.stream(
             to=self.sender_id,
-            date_sent_after=date_sent_after,
+            # date_sent_after=date_sent_after,
             limit=limit,
         )
 
         for message in messages:
             to = message.to
             from_ = message.from_
```

### Comparing `owlery-0.2.0/owlery/services/twilio.py` & `owlery-0.3.0/owlery/services/twilio.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/whatsapp/__init__.py` & `owlery-0.3.0/owlery/services/whatsapp/__init__.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery/services/whatsapp/twilio.py` & `owlery-0.3.0/owlery/services/whatsapp/twilio.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/owlery.egg-info/PKG-INFO` & `owlery-0.3.0/owlery.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owlery
-Version: 0.2.0
+Version: 0.3.0
 Summary: Uniform messaging service for Python applications.
 Author-email: Michael de Villiers <michael@devilears.co.za>
 Maintainer-email: Michael de Villiers <michael@devilears.co.za>
 License: MIT
 Project-URL: Homepage, https://github.com/COUR4G3/owlery/
 Project-URL: Documentation, https://owlery-messaging.readthedocs.io/
 Project-URL: Changes, https://owlery-messaging.readthedocs.io/en/latest/changelog.html
```

### Comparing `owlery-0.2.0/owlery.egg-info/SOURCES.txt` & `owlery-0.3.0/owlery.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,18 @@
 .readthedocs.yml
 CHANGELOG.md
 CONTRIBUTING.md
 Dockerfile
 LICENSE
 MANIFEST.in
 README.md
-docker-compose.yml
-dovecot.conf
 pyproject.toml
 requirements.txt
 tox.ini
 .github/FUNDING.yml
-.github/workflows/docs.yml
 .github/workflows/publish.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 .github/workflows/scripts/release.py
 .vscode/settings.json
 changelog.d/.gitkeep
 changelog.d/template.md
@@ -55,27 +52,34 @@
 owlery.egg-info/SOURCES.txt
 owlery.egg-info/dependency_links.txt
 owlery.egg-info/entry_points.txt
 owlery.egg-info/requires.txt
 owlery.egg-info/top_level.txt
 owlery/services/__init__.py
 owlery/services/misc.py
+owlery/services/reddit.py
 owlery/services/twilio.py
 owlery/services/email/__init__.py
+owlery/services/email/html.py
 owlery/services/email/imap.py
 owlery/services/email/pop3.py
 owlery/services/email/smtp.py
 owlery/services/mms/__init__.py
 owlery/services/mms/twilio.py
 owlery/services/sms/__init__.py
+owlery/services/sms/gsmmodem.py
 owlery/services/sms/twilio.py
+owlery/services/voice/__init__.py
 owlery/services/whatsapp/__init__.py
 owlery/services/whatsapp/twilio.py
+owlery/services/whatsapp/wabp.py
 tests/__init__.py
 tests/conftest.py
+tests/docker-compose.yml
+tests/dovecot.conf
 tests/requirements.txt
 tests/test_signals.py
 tests/services/__init__.py
 tests/services/test_manager.py
 tests/services/test_misc.py
 tests/services/test_service.py
 tests/services/email/__init__.py
```

### Comparing `owlery-0.2.0/pyproject.toml` & `owlery-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     "m2r2 ~= 0.3.3",
     "setuptools_scm ~= 7.1.0",
     "sphinx ~= 6.1.3",
     "sphinx_issues ~= 3.0.1",
     "sphinx-prompt ~= 1.6.0",
 ]
 tests = [
+    "coverage[toml] ~= 6.5.0",
     "pytest ~= 7.2.0",
     "pytest-cov ~= 4.0.0",
     "pytest-mock ~= 3.10.0",
     "pytest-skip-slow == 0.0.3",
     "tox ~= 4.5.1",
 ]
 typing = [
@@ -126,22 +127,23 @@
 
 [[tool.mypy.overrides]]
 module = [
     "boto3",
     "click",
     "django",
     "django.*",
+    "envelope",
     "flask",
     "phonenumbers",
     "requests_toolbelt.sessions",
     "sendgrid",
     "sendgrid.*",
     "smpplib",
     "smpplib.*",
-    "twilio.rest",
+    "twilio.*",
 ]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
 addopts = "--cov=owlery/ --cov-report=term-missing:skip-covered"
 markers = [
     "slow: tests that are slow",
```

### Comparing `owlery-0.2.0/tests/conftest.py` & `owlery-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/tests/services/email/test_imap.py` & `owlery-0.3.0/tests/services/email/test_imap.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,102 +1,129 @@
 import imaplib
+import socket
 import time
 
-from email.utils import make_msgid
-
 import pytest
 
 from owlery.exceptions import ServiceAuthFailed
-from owlery.services.email import EmailMessage
 from owlery.services.email.imap import IMAP
 
 
-@pytest.fixture()
-def message():
-    message = EmailMessage(
-        to=["user"],
-        subject="Test message",
-        body="This is a test message.",
-        from_="test@example.com",
-        id=make_msgid(),
+def check_imap(host, port):
+    try:
+        sock = socket.create_connection((host, port), timeout=5.0)
+        sock.send(b"\0")
+        sock.recv(1)
+    except (OSError, socket.timeout):
+        return False
+    else:
+        sock.close()
+
+    return True
+
+
+@pytest.fixture(scope="session")
+def imap_service(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 143)
+
+    docker_services.wait_until_responsive(
+        timeout=30.0,
+        pause=0.1,
+        check=lambda: check_imap(docker_ip, port),
     )
 
-    with imaplib.IMAP4(host="localhost", port=143) as imap:
+    return docker_ip, port
+
+
+@pytest.fixture()
+def imap_message(imap_service, message):
+    host, port = imap_service
+
+    with imaplib.IMAP4(host=host, port=port) as imap:
         imap.login("user", "pass")
 
         imap.append(
             "INBOX",
             (),
             time.time(),
             message.as_bytes(),
         )
 
     return message
 
 
 @pytest.fixture(scope="session")
-def imap():
-    return IMAP(host="localhost", port=143, user="user", password="pass")
+def imap(imap_service):
+    host, port = imap_service
+    return IMAP(host=host, port=port, user="user", password="pass")
 
 
 @pytest.fixture
-def manager_with_imap(manager):
+def manager_with_imap(imap_service, manager):
+    host, port = imap_service
     return manager.register(
         IMAP,
-        host="localhost",
-        port=143,
+        host=host,
+        port=port,
         user="user",
         password="pass",
     )
 
 
 def test_init():
     IMAP(host="localhost", port=143, user="user", password="pass")
 
 
 @pytest.mark.integration
-def test_connect():
-    imap = IMAP(host="localhost", port=143, user="user", password="pass")
+@pytest.mark.xfail
+def test_connect(imap_service):
+    host, port = imap_service
+    imap = IMAP(host=host, port=port, user="user", password="pass")
 
     imap.open()
     imap.close()
 
 
 @pytest.mark.integration
-def test_connect_ssl():
+def test_connect_ssl(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 993)
+
     imap = IMAP(
-        host="localhost",
-        port=993,
+        host=docker_ip,
+        port=port,
         ssl=True,
         user="user",
         password="pass",
     )
 
     imap.open()
     imap.close()
 
 
 @pytest.mark.integration
-def test_connect_starttls():
+def test_connect_starttls(imap_service):
+    host, port = imap_service
+
     imap = IMAP(
-        host="localhost",
-        port=143,
+        host=host,
+        port=port,
         starttls=True,
         user="user",
         password="pass",
     )
 
     imap.open()
     imap.close()
 
 
 @pytest.mark.integration
 @pytest.mark.slow
-def test_connect_wrong_credentials():
-    imap = IMAP(host="localhost", port=143, user="user", password="wrong")
+def test_connect_wrong_credentials(imap_service):
+    host, port = imap_service
+    imap = IMAP(host=host, port=port, user="user", password="wrong")
 
     with pytest.raises(ServiceAuthFailed):
         imap.open()
 
     imap.close()
 
 
@@ -117,36 +144,36 @@
 
 def test_specified_port():
     imap = IMAP(port=144)
     assert imap.port == 144
 
 
 @pytest.mark.integration
-def test_receive(imap, message):
+def test_receive(imap, imap_message):
     for received_message in imap.receive(limit=10):
         received_message = received_message
     imap.close()
-    assert received_message.id == message.id
+    assert received_message.id == imap_message.id
 
 
 @pytest.mark.integration
-def test_receive_contextmanager(imap, message):
+def test_receive_contextmanager(imap, imap_message):
     with imap:
         for received_message in imap.receive(limit=10):
             received_message = received_message
-    assert received_message.id == message.id
+    assert received_message.id == imap_message.id
 
 
 @pytest.mark.integration
-def test_receive_with_manager(manager_with_imap, message):
+def test_receive_with_manager(manager_with_imap, imap_message):
     for received_message in manager_with_imap.receive(limit=10):
         received_message = received_message
     manager_with_imap.close()
-    assert received_message.id == message.id
+    assert received_message.id == imap_message.id
 
 
 @pytest.mark.integration
-def test_receive_with_manager_contextmanager(manager_with_imap, message):
+def test_receive_with_manager_contextmanager(manager_with_imap, imap_message):
     with manager_with_imap:
         for received_message in manager_with_imap.receive(limit=10):
             received_message = received_message
-    assert received_message.id == message.id
+    assert received_message.id == imap_message.id
```

### Comparing `owlery-0.2.0/tests/services/email/test_pop3.py` & `owlery-0.3.0/tests/services/email/test_smtp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,154 @@
-import imaplib
-import secrets
-import time
+import socket
 
 import pytest
 
 from owlery.exceptions import ServiceAuthFailed
-from owlery.services.email import EmailMessage
-from owlery.services.email.pop3 import POP3
+from owlery.services.email.smtp import SMTP
 
 
-@pytest.fixture()
-def message():
-    message = EmailMessage(
-        to=["user"],
-        subject=f"Test message {secrets.token_hex(8)}",
-        body="This is a test message.",
-        from_="test@example.com",
-    )
+def check_smtp(host, port):
+    try:
+        sock = socket.create_connection((host, port), timeout=5.0)
+        sock.recv(1)
+    except (OSError, socket.timeout):
+        return False
+    else:
+        sock.close()
+
+    return True
 
-    with imaplib.IMAP4(host="localhost", port=144) as imap:
-        imap.login("user", "pass")
 
-        imap.append(
-            "INBOX",
-            (),
-            time.time(),
-            message.as_bytes(),
-        )
+@pytest.fixture(scope="session")
+def smtp_service(docker_ip, docker_services):
+    port = docker_services.port_for("smtp", 1025)
+
+    docker_services.wait_until_responsive(
+        timeout=30.0,
+        pause=0.1,
+        check=lambda: check_smtp(docker_ip, port),
+    )
 
-    return message
+    return docker_ip, port
 
 
 @pytest.fixture(scope="session")
-def pop3():
-    return POP3(host="localhost", port=110, user="user", password="pass")
+def smtp(smtp_service):
+    host, port = smtp_service
+    return SMTP(host=host, port=port, user="test", password="test")
 
 
 @pytest.fixture
-def manager_with_pop3(manager):
+def manager_with_smtp(manager, smtp_service):
+    host, port = smtp_service
     return manager.register(
-        POP3,
-        host="localhost",
-        port=110,
-        user="user",
-        password="pass",
+        SMTP,
+        host=host,
+        port=port,
+        user="test",
+        password="test",
     )
 
 
 def test_init():
-    POP3(host="localhost", port=110, user="user", password="pass")
+    SMTP()
+
+
+def test_auto_port():
+    smtp = SMTP()
+    assert smtp.port == 25
+
+
+def test_auto_port_ssl():
+    smtp = SMTP(ssl=True)
+    assert smtp.port == 465
+
+
+def test_auto_port_starttls():
+    smtp = SMTP(starttls=True)
+    assert smtp.port == 587
+
+
+def test_specified_port():
+    smtp = SMTP(port=26)
+    assert smtp.port == 26
 
 
 @pytest.mark.integration
-def test_connect(pop3):
-    pop3.open()
-    pop3.close()
+def test_connect(smtp):
+    smtp.open()
+    smtp.close()
 
 
 @pytest.mark.integration
-def test_connect_ssl():
-    pop3 = POP3(
-        host="localhost",
-        port=995,
+def test_connect_ssl(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 465)
+
+    smtp = SMTP(
+        host=docker_ip,
+        port=port,
         ssl=True,
         user="user",
         password="pass",
     )
 
-    pop3.open()
-    pop3.close()
+    smtp.open()
+    smtp.close()
 
 
 @pytest.mark.integration
-def test_connect_starttls():
-    pop3 = POP3(
-        host="localhost",
-        port=110,
+def test_connect_starttls(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 587)
+
+    smtp = SMTP(
+        host=docker_ip,
+        port=port,
         starttls=True,
         user="user",
         password="pass",
     )
 
-    pop3.open()
-    pop3.close()
+    smtp.open()
+    smtp.close()
 
 
 @pytest.mark.integration
-@pytest.mark.slow
-def test_connect_wrong_credentials(pop3):
-    pop3 = POP3(
-        host="localhost",
-        port=110,
-        user="user",
-        password="wrong",
-        starttls=True,
-    )
-
-    with pytest.raises(ServiceAuthFailed):
-        pop3.open()
-
-    pop3.close()
-
-
-def test_auto_port():
-    pop3 = POP3()
-    assert pop3.port == 110
+def test_connect_auth(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 587)
+    smtp = SMTP(host=docker_ip, port=port, user="user", password="pass")
 
+    smtp.open()
+    smtp.close()
 
-def test_auto_port_ssl():
-    pop3 = POP3(ssl=True)
-    assert pop3.port == 995
-
-
-def test_auto_port_starttls():
-    pop3 = POP3(starttls=True)
-    assert pop3.port == 110
 
+@pytest.mark.integration
+def test_connect_wrong_credentials(docker_ip, docker_services):
+    port = docker_services.port_for("imap", 587)
+    smtp = SMTP(host=docker_ip, port=port, user="user", password="wrong")
 
-def test_specified_port():
-    pop3 = POP3(port=111)
-    assert pop3.port == 111
+    with pytest.raises(ServiceAuthFailed):
+        smtp.open()
+    smtp.close()
 
 
 @pytest.mark.integration
-def test_receive(pop3, message):
-    received_message = None
-    for received_message in pop3.receive(limit=10):
-        received_message = received_message
-    pop3.close()
-    assert received_message.subject == message.subject
+def test_send(smtp, message):
+    smtp.send_message(message)
+    smtp.close()
 
 
 @pytest.mark.integration
-def test_receive_contextmanager(pop3, message):
-    received_message = None
-    with pop3:
-        for received_message in pop3.receive(limit=10):
-            received_message = received_message
-    assert received_message.subject == message.subject
+def test_send_contextmanager(smtp, message):
+    with smtp:
+        smtp.send_message(message)
 
 
 @pytest.mark.integration
-def test_receive_with_manager(manager_with_pop3, message):
-    received_message = None
-    for received_message in manager_with_pop3.receive(limit=10):
-        received_message = received_message
-    manager_with_pop3.close()
-    assert received_message.subject == message.subject
+def test_send_with_manager(manager_with_smtp, message):
+    manager_with_smtp.send_message(message)
+    manager_with_smtp.close()
 
 
 @pytest.mark.integration
-def test_receive_with_manager_contextmanager(manager_with_pop3, message):
-    received_message = None
-    with manager_with_pop3:
-        for received_message in manager_with_pop3.receive(limit=10):
-            received_message = received_message
-    assert received_message.subject == message.subject
+def test_send_with_manager_contextmanager(manager_with_smtp, message):
+    with manager_with_smtp:
+        manager_with_smtp.send_message(message)
```

### Comparing `owlery-0.2.0/tests/services/test_manager.py` & `owlery-0.3.0/tests/services/test_manager.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/tests/services/test_misc.py` & `owlery-0.3.0/tests/services/test_misc.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/tests/services/test_service.py` & `owlery-0.3.0/tests/services/test_service.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/tests/test_signals.py` & `owlery-0.3.0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `owlery-0.2.0/tox.ini` & `owlery-0.3.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 deps = coverage[toml]
 skip_install = true
 commands = coverage erase
 
 [testenv:coveralls]
 description = check coverage with coveralls
 deps =
+    coverage[toml]<7
     coveralls
 commands =
     coveralls
 passenv = GITHUB_*
 
 [testenv:pkg]
 description = check packaging
```

