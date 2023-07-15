# Comparing `tmp/linsharecli-1.1.2.tar.gz` & `tmp/linsharecli-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linsharecli-1.1.2.tar", last modified: Fri Jul 29 17:14:37 2022, max compression
+gzip compressed data, was "linsharecli-1.1.3.tar", last modified: Sat Jul 15 10:27:34 2023, max compression
```

## Comparing `linsharecli-1.1.2.tar` & `linsharecli-1.1.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.645426 linsharecli-1.1.2/
--rw-r--r--   0 fred      (1000) fred      (1000)    35147 2022-04-30 15:18:02.000000 linsharecli-1.1.2/LICENSE.txt
--rw-r--r--   0 fred      (1000) fred      (1000)     2431 2022-07-29 17:14:37.645426 linsharecli-1.1.2/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)     1799 2022-04-30 15:18:02.000000 linsharecli-1.1.2/README.rst
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.638759 linsharecli-1.1.2/bin/
--rwxr-xr-x   0 fred      (1000) fred      (1000)      241 2022-01-15 02:09:40.000000 linsharecli-1.1.2/bin/debug.sh
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.638759 linsharecli-1.1.2/linsharecli/
--rw-r--r--   0 fred      (1000) fred      (1000)      861 2022-07-09 13:33:43.000000 linsharecli-1.1.2/linsharecli/__init__.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.642093 linsharecli-1.1.2/linsharecli/admin/
--rw-r--r--   0 fred      (1000) fred      (1000)    12258 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6419 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/authentication.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11384 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)    26343 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/domain.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8723 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/domainpolicies.py
--rw-r--r--   0 fred      (1000) fred      (1000)    12649 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/dpattern.py
--rw-r--r--   0 fred      (1000) fred      (1000)    47804 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/admin/func.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7796 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/iuser.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9123 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/admin/jwt.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8218 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/ldap.py
--rw-r--r--   0 fred      (1000) fred      (1000)    14180 2022-05-24 19:09:32.000000 linsharecli-1.1.2/linsharecli/admin/mail_activations.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9286 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/mail_attachments.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4020 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/mail_configs.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5444 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/public_keys.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8480 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/admin/shared_space_members.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6639 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/shared_spaces.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2344 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/threads.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2591 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/tmembers.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6260 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/upgrade_tasks.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3260 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/admin/user.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9029 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/admin/welcome_messages.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.642093 linsharecli-1.1.2/linsharecli/common/
--rw-r--r--   0 fred      (1000) fred      (1000)      838 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/common/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4334 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/common/actions.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2784 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/common/cell.py
--rw-r--r--   0 fred      (1000) fred      (1000)    30468 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/common/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)    13264 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/common/tables.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.642093 linsharecli-1.1.2/linsharecli/tests/
--rw-r--r--   0 fred      (1000) fred      (1000)        0 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/tests/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6131 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/tests/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)    14129 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/tests/documents.py
--rw-r--r--   0 fred      (1000) fred      (1000)    11040 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/tests/misc.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1333 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/tests/threads.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.645426 linsharecli-1.1.2/linsharecli/user/
--rw-r--r--   0 fred      (1000) fred      (1000)    13439 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7034 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/audit.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5846 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/contactslists.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7926 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/contactslistscontacts.py
--rw-r--r--   0 fred      (1000) fred      (1000)     8314 2022-07-09 12:19:31.000000 linsharecli-1.1.2/linsharecli/user/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)    17632 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/documents.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7621 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/guests.py
--rw-r--r--   0 fred      (1000) fred      (1000)    10677 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/jwt.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4135 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/rshares.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7635 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/shared_space_audit.py
--rw-r--r--   0 fred      (1000) fred      (1000)    10067 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/shared_space_members.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9332 2022-07-29 17:11:17.000000 linsharecli-1.1.2/linsharecli/user/shared_spaces.py
--rw-r--r--   0 fred      (1000) fred      (1000)    10200 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/shares.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2917 2022-04-30 15:18:02.000000 linsharecli-1.1.2/linsharecli/user/users.py
--rw-r--r--   0 fred      (1000) fred      (1000)    22265 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/wg_documents.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9964 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/wg_members.py
--rw-r--r--   0 fred      (1000) fred      (1000)     5019 2022-06-02 18:58:46.000000 linsharecli-1.1.2/linsharecli/user/workgroups.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2022-07-29 17:14:37.638759 linsharecli-1.1.2/linsharecli.egg-info/
--rwxr-xr-x   0 fred      (1000) fred      (1000)     2431 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/PKG-INFO
--rwxr-xr-x   0 fred      (1000) fred      (1000)     1761 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/SOURCES.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/dependency_links.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)      205 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/entry_points.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)      100 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/requires.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)       12 2022-07-29 17:14:37.000000 linsharecli-1.1.2/linsharecli.egg-info/top_level.txt
--rw-r--r--   0 fred      (1000) fred      (1000)       38 2022-07-29 17:14:37.645426 linsharecli-1.1.2/setup.cfg
--rwxr-xr-x   0 fred      (1000) fred      (1000)     3088 2022-07-09 13:33:43.000000 linsharecli-1.1.2/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.617428 linsharecli-1.1.3/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35147 2022-04-30 15:18:02.000000 linsharecli-1.1.3/LICENSE.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)     2411 2023-07-15 10:27:34.617428 linsharecli-1.1.3/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)     1799 2022-04-30 15:18:02.000000 linsharecli-1.1.3/README.rst
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.600762 linsharecli-1.1.3/bin/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      241 2022-01-15 02:09:40.000000 linsharecli-1.1.3/bin/debug.sh
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.600762 linsharecli-1.1.3/linsharecli/
+-rw-r--r--   0 fred      (1000) fred      (1000)      861 2022-07-29 17:14:37.000000 linsharecli-1.1.3/linsharecli/__init__.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.610762 linsharecli-1.1.3/linsharecli/admin/
+-rw-r--r--   0 fred      (1000) fred      (1000)    12316 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6419 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/admin/authentication.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11691 2023-03-17 18:04:12.000000 linsharecli-1.1.3/linsharecli/admin/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    25876 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/domain.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8783 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/domainpolicies.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12709 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/dpattern.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    47804 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/admin/func.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7856 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/iuser.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9183 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/jwt.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8278 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/ldap.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    14240 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/mail_activations.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9354 2023-07-15 10:20:11.000000 linsharecli-1.1.3/linsharecli/admin/mail_attachments.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4080 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/mail_configs.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5504 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/public_keys.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8480 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/admin/shared_space_members.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6639 2022-07-29 17:11:17.000000 linsharecli-1.1.3/linsharecli/admin/shared_spaces.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2404 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/threads.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2651 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/tmembers.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6268 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/upgrade_tasks.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3320 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/user.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9089 2022-08-01 15:40:50.000000 linsharecli-1.1.3/linsharecli/admin/welcome_messages.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.614095 linsharecli-1.1.3/linsharecli/common/
+-rw-r--r--   0 fred      (1000) fred      (1000)      838 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/common/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4334 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/common/actions.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2784 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/common/cell.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    30468 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/common/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    13264 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/common/tables.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.614095 linsharecli-1.1.3/linsharecli/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)        0 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/tests/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6131 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/tests/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    14129 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/tests/documents.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11040 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/tests/misc.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1333 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/tests/threads.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.617428 linsharecli-1.1.3/linsharecli/user/
+-rw-r--r--   0 fred      (1000) fred      (1000)    13439 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7034 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/audit.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5846 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/contactslists.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7926 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/contactslistscontacts.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     8314 2022-07-09 12:19:31.000000 linsharecli-1.1.3/linsharecli/user/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    17632 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/documents.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7621 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/guests.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10677 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/jwt.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4135 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/rshares.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7635 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/shared_space_audit.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10067 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/shared_space_members.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9332 2022-07-29 17:11:17.000000 linsharecli-1.1.3/linsharecli/user/shared_spaces.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10200 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/shares.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2917 2022-04-30 15:18:02.000000 linsharecli-1.1.3/linsharecli/user/users.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    22265 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/wg_documents.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9964 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/wg_members.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     5019 2022-06-02 18:58:46.000000 linsharecli-1.1.3/linsharecli/user/workgroups.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 10:27:34.600762 linsharecli-1.1.3/linsharecli.egg-info/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     2411 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/PKG-INFO
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     1761 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/SOURCES.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/dependency_links.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      204 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/entry_points.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      100 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/requires.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       12 2023-07-15 10:27:34.000000 linsharecli-1.1.3/linsharecli.egg-info/top_level.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-07-15 10:27:34.617428 linsharecli-1.1.3/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     3088 2023-07-15 10:20:45.000000 linsharecli-1.1.3/setup.py
```

### Comparing `linsharecli-1.1.2/LICENSE.txt` & `linsharecli-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/PKG-INFO` & `linsharecli-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: linsharecli
-Version: 1.1.2
+Version: 1.1.3
 Summary: LinShare command line interface.
 Home-page: https://github.com/fred49/linshare-cli
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -95,9 +94,7 @@
 ``$ linshareadmcli -s my-second-config domains list``
 
 You can also list all available configurations using:
 
 ``$ linshareadmcli list``
 
 
-
-
```

### Comparing `linsharecli-1.1.2/README.rst` & `linsharecli-1.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/__init__.py` & `linsharecli-1.1.3/linsharecli/common/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,9 +19,7 @@
 #
 # Copyright 2014 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
-
-__version__ = '1.1.2'
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/__init__.py` & `linsharecli-1.1.3/linsharecli/admin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 from .. import __version__
 
 # if you want to debug argcomplete completion,
 # you just need to export _ARC_DEBUG=True
 
 PARSERS = []
 
-def _add_parser(name=None, description=None, parsers=None):
+
+def _add_parser(name="", description=None, parsers=None):
     PARSERS.append(
         {
             'name': name,
             'description': description,
             'parsers': parsers
         }
     )
@@ -256,15 +257,16 @@
             **self.config.server.base_url.get_arg_parse_arguments())
 
         self.parser.add_argument('--debugger-names', action="append")
         self.parser.add_argument('--no-cell', action="store_true")
 
         # Adding all others parsers.
         subparsers = self.parser.add_subparsers()
-        for parser in PARSERS:
+        parsers = sorted(PARSERS, key=lambda d: d['name'])
+        for parser in parsers:
             name = parser.get('name')
             description = parser.get('description')
             func = parser.get('parsers')
             func(subparsers, name, description, self.config)
 
     def reload(self):
         """TODO"""
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/authentication.py` & `linsharecli-1.1.3/linsharecli/admin/authentication.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/admin/core.py` & `linsharecli-1.1.3/linsharecli/admin/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,15 +265,21 @@
 
 def add_parser(subparsers, name, desc, config):
     """Add test commands."""
     parser = subparsers.add_parser('test', add_help=False)
     parser.add_argument('files', nargs='*')
     parser.set_defaults(__func__=TestCommand(config))
 
-    parser = subparsers.add_parser('raw', add_help=True)
+    parser = subparsers.add_parser(
+        'raw',
+        help=(
+            "Retrieve json data from URL. Authentication is handled liek any"
+            " other commands."
+        )
+    )
     parser.add_argument('url')
     parser.add_argument(
             '-r', '--repeat', default=1,
             help="default=1", type=int)
     parser.add_argument(
         '-m', '--method',
         choices=["GET", "POST", "DELETE", "HEAD", "OPTIONS", "PUT"])
@@ -284,15 +290,21 @@
             '-s', '--silent', action="store_true",
             help="Do not display the payload")
     parser.add_argument(
             '--jq', action="store_true",
             help="pure json only")
     parser.set_defaults(__func__=RawCommand(config))
 
-    parser = subparsers.add_parser('auto')
+    parser = subparsers.add_parser(
+        'auto',
+        help=(
+            "Try to build dynamically a pretty table from data retieved from"
+            " the provide url as positional argument."
+        )
+    )
     parser.add_argument('url')
     parser.add_argument(
         '-x', '--complex-cells', action="append",
         default=[],
         help=(
             "Wil try to format these cells with default complex cell"
             " formatter: {name} ({uuid})"
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/domain.py` & `linsharecli-1.1.3/linsharecli/admin/domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,27 @@
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
-
 import json
 
+from argtoolbox import DefaultCompleter as Completer
+from vhatable.cell import ComplexCell
+from vhatable.cell import ComplexCellBuilder
+from vhatable.filters import PartialOr
 from linshareapi.cache import Time
 from linsharecli.admin.core import DefaultCommand
 from linsharecli.common.core import add_list_parser_options
 from linsharecli.common.core import add_delete_parser_options
 from linsharecli.common.actions import CreateOneAction
 from linsharecli.common.tables import DeleteAction
 from linsharecli.common.tables import TableBuilder
-from argtoolbox import DefaultCompleter as Completer
-from vhatable.cell import ComplexCell
-from vhatable.cell import ComplexCellBuilder
-from vhatable.filters import PartialOr
 
 
 class DomainsCommand(DefaultCommand):
     """For  api >= 1.9"""
     # pylint: disable=too-many-instance-attributes
     IDENTIFIER = "name"
     DEFAULT_SORT = "name"
@@ -51,74 +50,94 @@
 
     DEFAULT_TOTAL = "Domain found : %(count)s"
     MSG_RS_NOT_FOUND = "No domain could be found."
     MSG_RS_DELETED = (
         "%(position)s/%(count)s: "
         "The domain '%(name)s' (%(uuid)s) was deleted. (%(time)s s)"
     )
-    MSG_RS_CAN_NOT_BE_DELETED = "The domain '%(name)s'  '%(uuid)s' can not be deleted."
+    MSG_RS_CAN_NOT_BE_DELETED = (
+        "The domain '%(name)s'  '%(uuid)s' can not be deleted."
+    )
     MSG_RS_CAN_NOT_BE_DELETED_M = "%(count)s domain (s) can not be deleted."
-    MSG_RS_UPDATED = "The domain '%(name)s' (%(uuid)s) was successfully updated."
+    MSG_RS_UPDATED = (
+        "The domain '%(name)s' (%(uuid)s) was successfully updated."
+        )
     MSG_RS_CREATED = (
         "The domain '%(name)s' (%(uuid)s) "
         "was successfully created. (%(time)s s)"
     )
 
-    # pylint: disable=no-self-use
     def init_old_language_key_before_5(self):
+        """TODO"""
         DomainsCommand.IDENTIFIER = "label"
         DomainsCommand.DEFAULT_SORT = "label"
         DomainsCommand.RESOURCE_IDENTIFIER = "identifier"
 
         DomainsCommand.DEFAULT_TOTAL = "Domain found : %(count)s"
         DomainsCommand.MSG_RS_NOT_FOUND = "No domain could be found."
         DomainsCommand.MSG_RS_DELETED = (
             "%(position)s/%(count)s: "
             "The domain '%(label)s' (%(identifier)s) was deleted. (%(time)s s)"
         )
-        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED = "The domain '%(label)s'  '%(identifier)s' can not be deleted."
-        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED_M = "%(count)s domain (s) can not be deleted."
-        DomainsCommand.MSG_RS_UPDATED = "The domain '%(label)s' (%(identifier)s) was successfully updated."
+        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED = (
+            "The domain '%(label)s'  '%(identifier)s' can not be deleted."
+        )
+        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED_M = (
+            "%(count)s domain (s) can not be deleted."
+        )
+        DomainsCommand.MSG_RS_UPDATED = (
+            "The domain '%(label)s' (%(identifier)s) was successfully updated."
+        )
         DomainsCommand.MSG_RS_CREATED = (
             "The domain '%(label)s' (%(identifier)s) "
             "was successfully created. (%(time)s s)"
         )
 
-    # pylint: disable=no-self-use
     def init_old_language_key(self):
         """For  api >= 1.6 and api <= 1.8"""
         DomainsCommand.IDENTIFIER = "identifier"
         DomainsCommand.DEFAULT_SORT = "identifier"
         DomainsCommand.RESOURCE_IDENTIFIER = "identifier"
 
         DomainsCommand.DEFAULT_TOTAL = "Domain found : %(count)s"
         DomainsCommand.MSG_RS_NOT_FOUND = "No domain could be found."
-        DomainsCommand.MSG_RS_DELETED = "The domain '%(identifier)s' was deleted. (%(time)s s)"
+        DomainsCommand.MSG_RS_DELETED = (
+            "The domain '%(identifier)s' was deleted. (%(time)s s)"
+        )
         DomainsCommand.MSG_RS_DELETED = (
             "%(position)s/%(count)s: "
             "The domain '%(identifier)s' was deleted. (%(time)s s)"
         )
-        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED = "The domain '%(identifier)s' can not be deleted."
-        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED_M = "%(count)s domain (s) can not be deleted."
-        DomainsCommand.MSG_RS_UPDATED = "The domain '%(identifier)s' was successfully updated."
-        DomainsCommand.MSG_RS_CREATED = "The domain '%(identifier)s' was successfully created."
+        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED = (
+            "The domain '%(identifier)s' can not be deleted."
+        )
+        DomainsCommand.MSG_RS_CAN_NOT_BE_DELETED_M = (
+            "%(count)s domain (s) can not be deleted."
+        )
+        DomainsCommand.MSG_RS_UPDATED = (
+            "The domain '%(identifier)s' was successfully updated."
+        )
+        DomainsCommand.MSG_RS_CREATED = (
+            "The domain '%(identifier)s' was successfully created."
+        )
 
     def complete(self, args, prefix):
-        super(DomainsCommand, self).__call__(args)
+        super().__call__(args)
         if self.api_version == 0:
             self.init_old_language_key()
         elif self.api_version < 5:
             self.init_old_language_key_before_5()
         json_obj = self.ls.domains.list()
         return (v.get(self.RESOURCE_IDENTIFIER)
-                for v in json_obj if v.get(self.RESOURCE_IDENTIFIER).startswith(prefix))
+                for v in json_obj if v.get(
+                    self.RESOURCE_IDENTIFIER).startswith(prefix))
 
     def complete_welcome(self, args, prefix):
         """TODO"""
-        super(DomainsCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.welcome_messages.list(args.identifier)
         return (v.get('uuid')
                 for v in json_obj if v.get('uuid').startswith(prefix))
 
 
 class ProviderCell(ComplexCell):
     """TODO"""
@@ -141,30 +160,32 @@
 class DDeleteAction(DeleteAction):
     """TODO"""
 
     MSG_RS_DELETED = (
         "%(position)s/%(count)s: "
         "The domain '%(label)s' (%(identifier)s) was deleted. (%(time)s s)"
     )
-    MSG_RS_CAN_NOT_BE_DELETED = "The domain '%(identifier)s' can not be deleted."
+    MSG_RS_CAN_NOT_BE_DELETED = (
+        "The domain '%(identifier)s' can not be deleted."
+    )
 
     def __init__(self):
-        super(DDeleteAction, self).__init__(
+        super().__init__(
             mode=0,
             identifier="label",
             resource_identifier="identifier",
         )
 
 
 class DomainsListCommand(DomainsCommand):
     """ List all domains."""
 
     @Time('linsharecli.domains', label='Global time : %(time)s')
     def __call__(self, args):
-        super(DomainsListCommand, self).__call__(args)
+        super().__call__(args)
         if self.api_version == 0:
             self.init_old_language_key()
         elif self.api_version < 5:
             self.init_old_language_key_before_5()
         endpoint = self.ls.domains
         tbu = TableBuilder(self.ls, endpoint, self.DEFAULT_SORT)
         tbu.load_args(args)
@@ -193,102 +214,99 @@
         )
         if args.extended and self.api_version >= 5:
             table = tbu.build().load_v2(endpoint.list())
             domains = []
             for row in table.get_raw():
                 domains.append(endpoint.get(row['uuid']))
             return tbu.build().load_v2(domains).render()
-        else:
-            return tbu.build().load_v2(endpoint.list()).render()
+        return tbu.build().load_v2(endpoint.list()).render()
 
     def complete_fields(self, args, prefix):
         """TODO"""
         # pylint: disable=unused-argument
-        super(DomainsListCommand, self).__call__(args)
+        super().__call__(args)
         cli = self.ls.domains
         return cli.get_rbu().get_keys(True)
 
 
 class DomainsCreateCommand(DomainsCommand):
     """ List all domains."""
     # pylint: disable=unused-argument
 
     def __call__(self, args):
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         if self.api_version == 0:
             self.init_old_language_key()
         elif self.api_version < 5:
             if not args.description:
                 args.description = args.identifier
             self.init_old_language_key_before_5()
 
         act = CreateOneAction(self, self.ls.domains)
         if act.load(args).execute():
             if not args.domain_policy_auto:
                 return True
-            else:
-                domain_uuid = act.result.get('identifier')
-                policy = {
-                    "accessPolicy": {
-                        "rules": [
-                            {
-                                "domain": {
-                                    "identifier": domain_uuid,
-                                },
-                                "type": "ALLOW"
+            domain_uuid = act.result.get('identifier')
+            policy = {
+                "accessPolicy": {
+                    "rules": [
+                        {
+                            "domain": {
+                                "identifier": domain_uuid,
                             },
-                            {
-                                "type": "DENY_ALL"
-                            }
-                        ]
-                    },
-                    "label": args.identifier,
-                }
-                self.log.debug(json.dumps(policy, sort_keys=True, indent=2))
-                policy = self.ls.domain_policies.create(policy)
-                self.log.debug(json.dumps(policy, sort_keys=True, indent=2))
-                domain = self.ls.domains.get(domain_uuid)
-                domain['policy'] = policy
-                self.ls.domains.update(domain)
+                            "type": "ALLOW"
+                        },
+                        {
+                            "type": "DENY_ALL"
+                        }
+                    ]
+                },
+                "label": args.identifier,
+            }
+            self.log.debug(json.dumps(policy, sort_keys=True, indent=2))
+            policy = self.ls.domain_policies.create(policy)
+            self.log.debug(json.dumps(policy, sort_keys=True, indent=2))
+            domain = self.ls.domains.get(domain_uuid)
+            domain['policy'] = policy
+            self.ls.domains.update(domain)
             return True
-        else:
-            return False
+        return False
 
     def complete(self, args, prefix):
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_type(self, args, prefix):
         """ Complete with available domain type."""
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_type()
 
     def complete_role(self, args, prefix):
         """ Complete with available role."""
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_role()
 
     def complete_language(self, args, prefix):
         """ Complete with available language."""
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_language()
 
     def complete_mail_language(self, args, prefix):
         """ Complete with available external mail language."""
-        super(DomainsCreateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_mail_language()
 
 
 class DomainsUpdateCommand(DomainsCommand):
     """ Update a domain."""
 
     def __call__(self, args):
-        super(DomainsUpdateCommand, self).__call__(args)
+        super().__call__(args)
         resource = None
         for model in self.ls.domains.list():
             if model.get('identifier') == args.identifier:
                 resource = model
                 break
         if resource is None:
             raise ValueError("Domain idenfier not found")
@@ -304,37 +322,37 @@
         return self._run(
             self.ls.domains.update,
             "The following domain '%(identifier)s' was successfully updated",
             args.identifier,
             resource)
 
     def complete(self, args, prefix):
-        super(DomainsUpdateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_role(self, args, prefix):
         """ Complete with available role."""
         # pylint: disable=unused-argument
-        super(DomainsUpdateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_role()
 
     def complete_language(self, args, prefix):
         """ Complete with available language."""
         # pylint: disable=unused-argument
-        super(DomainsUpdateCommand, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_language()
 
 
 class DomainsUpdateV5Command(DomainsCommand):
     """ Update a domain."""
 
     def __call__(self, args):
-        super(DomainsUpdateV5Command, self).__call__(args)
+        super().__call__(args)
         domain_uuid = getattr(args, self.RESOURCE_IDENTIFIER)
         resource = self.ls.domains.get(domain_uuid)
         if resource is None:
             raise ValueError("Domain uuid not found")
         rbu = self.ls.domains.get_rbu()
         rbu.copy(resource)
         rbu.load_from_args(args)
@@ -342,54 +360,54 @@
         return self._run(
             self.ls.domains.update,
             "The following domain '%(uuid)s' was successfully updated",
             domain_uuid,
             resource)
 
     def complete(self, args, prefix):
-        super(DomainsUpdateV5Command, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_role(self, args, prefix):
         """ Complete with available role."""
         # pylint: disable=unused-argument
-        super(DomainsUpdateV5Command, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_role()
 
     def complete_language(self, args, prefix):
         """ Complete with available language."""
         # pylint: disable=unused-argument
-        super(DomainsUpdateV5Command, self).__call__(args)
+        super().__call__(args)
         return self.ls.domains.options_language()
 
 
 class DomainsDeleteCommand(DomainsCommand):
     """ List all domains."""
 
     def __call__(self, args):
-        super(DomainsDeleteCommand, self).__call__(args)
+        super().__call__(args)
         cli = self.ls.domains
         if self.api_version == 0:
             self.init_old_language_key()
             return self._delete(
                 args,
                 cli,
                 args.identifier)
-        elif self.api_version < 5:
+        if self.api_version < 5:
             self.init_old_language_key_before_5()
         return self._delete_all(args, cli, args.uuids)
 
 
 class DomainProvidersCreateCommand(DomainsCommand):
     """ Update a domain."""
 
     def __call__(self, args):
-        super(DomainProvidersCreateCommand, self).__call__(args)
+        super().__call__(args)
         resource = None
         for model in self.ls.domains.list():
             if model.get('identifier') == args.identifier:
                 resource = model
                 break
         if resource is None:
             raise ValueError("Domain idenfier not found")
@@ -412,39 +430,39 @@
             self.ls.domains.update,
             "The following user provider for domain '%(identifier)s' was \
 successfully created",
             args.identifier,
             rbu.to_resource())
 
     def complete(self, args, prefix):
-        super(DomainProvidersCreateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_ldap(self, args, prefix):
         """TODO"""
-        super(DomainProvidersCreateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.ldap_connections.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_dpattern(self, args, prefix):
         """TODO"""
-        super(DomainProvidersCreateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domain_patterns.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
 
 class DomainProvidersDeleteCommand(DomainsCommand):
     """ List all domains."""
 
     def __call__(self, args):
-        super(DomainProvidersDeleteCommand, self).__call__(args)
+        super().__call__(args)
         resource = None
         for model in self.ls.domains.list():
             if model.get('identifier') == args.identifier:
                 resource = model
                 break
         if resource is None:
             raise ValueError("Domain idenfier not found")
@@ -457,25 +475,25 @@
             self.ls.domains.update,
             "The following user provider '%(identifier)s' was successfully \
 deleted",
             args.identifier,
             rbu.to_resource())
 
     def complete(self, args, prefix):
-        super(DomainProvidersDeleteCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
 
 class DomainProvidersUpdateCommand(DomainsCommand):
     """ Update a user provider."""
 
     def __call__(self, args):
-        super(DomainProvidersUpdateCommand, self).__call__(args)
+        super().__call__(args)
         resource = None
         for model in self.ls.domains.list():
             if model.get('identifier') == args.identifier:
                 resource = model
                 break
         if resource is None:
             raise ValueError("Domain idenfier not found")
@@ -499,29 +517,29 @@
             self.ls.domains.update,
             "The following user provider '%(identifier)s' was successfully \
 updated",
             args.identifier,
             rbu.to_resource())
 
     def complete(self, args, prefix):
-        super(DomainProvidersUpdateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domains.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_ldap(self, args, prefix):
         """TODO"""
-        super(DomainProvidersUpdateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.ldap_connections.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
     def complete_dpattern(self, args, prefix):
         """TODO"""
-        super(DomainProvidersUpdateCommand, self).__call__(args)
+        super().__call__(args)
         json_obj = self.ls.domain_patterns.list()
         return (v.get('identifier')
                 for v in json_obj if v.get('identifier').startswith(prefix))
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all domain sub commands."""
@@ -533,85 +551,86 @@
     # command : list
     parser = subparsers2.add_parser(
         'list',
         help="list domains")
     parser.add_argument(
         'identifiers', nargs="*",
         help="Filter domains by their identifiers")
-    parser.add_argument('-n', '--label', action="store_true",
-                        help="sort by domain label")
     if api_version == 0:
         add_list_parser_options(parser, delete=True, cdate=False)
     else:
         add_list_parser_options(parser, delete=True, cdate=False)
     parser.set_defaults(__func__=DomainsListCommand(config))
 
     # command : create
-    parser_tmp2 = subparsers2.add_parser(
-        'create', help="create domain.")
-    if api_version < 5:
-        parser_tmp2.add_argument('--label', action="store", help="")
-        parser_tmp2.add_argument('identifier', action="store", help="")
-    else:
-        parser_tmp2.add_argument('name', action="store", help="")
-    parser_tmp2.add_argument(
-        '--type', dest="domain_type", action="store", help="",
-        required=True).completer = Completer("complete_type")
-    parser_tmp2.add_argument('--description', action="store", help="")
-    parser_tmp2.add_argument(
-        '--role', dest="role", action="store",
-        help="").completer = Completer("complete_role")
-    parser_tmp2.add_argument(
-        '--language', dest="language", action="store",
-        help="").completer = Completer("complete_language")
-    parser_tmp2.add_argument(
-        '--parent', dest="parent_id", action="store",
-        help="TODO").completer = Completer()
-    parser_tmp2.add_argument(
-        '--mime-policy', dest="mime_policy", action="store",
-        help="TODO").completer = Completer("complete_mime")
-    parser_tmp2.add_argument(
-        '--domain-policy', dest="domain_policy", action="store",
-        help="TODO").completer = Completer("complete_policy")
-    parser_tmp2.add_argument(
-        '--domain-policy-auto', dest="domain_policy_auto", action="store_true",
-        help="TODO")
-    parser_tmp2.add_argument(
-        '--mail-config', dest="mail_config", action="store",
-        help="TODO").completer = Completer("complete_mail")
-    parser_tmp2.add_argument('--cli-mode', action="store_true", help="")
-    parser_tmp2.set_defaults(__func__=DomainsCreateCommand(config))
+    def add_cmd_create_domain(subparsers2):
+        parser_tmp2 = subparsers2.add_parser(
+            'create', help="create domain.")
+        if api_version < 5:
+            parser_tmp2.add_argument('--label', action="store", help="")
+            parser_tmp2.add_argument('identifier', action="store", help="")
+        else:
+            parser_tmp2.add_argument('name', action="store", help="")
+        parser_tmp2.add_argument(
+            '--type', dest="domain_type", action="store", help="",
+            required=True).completer = Completer("complete_type")
+        parser_tmp2.add_argument('--description', action="store", help="")
+        parser_tmp2.add_argument(
+            '--role', dest="role", action="store",
+            help="").completer = Completer("complete_role")
+        parser_tmp2.add_argument(
+            '--language', dest="language", action="store",
+            help="").completer = Completer("complete_language")
+        parser_tmp2.add_argument(
+            '--parent', dest="parent_id", action="store",
+            help="TODO").completer = Completer()
+        parser_tmp2.add_argument(
+            '--mime-policy', dest="mime_policy", action="store",
+            help="TODO").completer = Completer("complete_mime")
+        parser_tmp2.add_argument(
+            '--domain-policy', dest="domain_policy", action="store",
+            help="TODO").completer = Completer("complete_policy")
+        parser_tmp2.add_argument(
+            '--domain-policy-auto', dest="domain_policy_auto",
+            action="store_true",
+            help="TODO")
+        parser_tmp2.add_argument(
+            '--mail-config', dest="mail_config", action="store",
+            help="TODO").completer = Completer("complete_mail")
+        parser_tmp2.add_argument('--cli-mode', action="store_true", help="")
+        parser_tmp2.set_defaults(__func__=DomainsCreateCommand(config))
 
     # command : update
-    parser_tmp2 = subparsers2.add_parser(
-        'update', help="update domain.")
-    parser_tmp2.add_argument('--label', action="store", help="")
-    parser_tmp2.add_argument('--description', action="store", help="")
-    parser_tmp2.add_argument(
-        '--role', dest="role", action="store",
-        help="").completer = Completer("complete_role")
-    parser_tmp2.add_argument(
-        '--language', dest="language", action="store",
-        help="").completer = Completer("complete_language")
-    if api_version >= 1:
-        parser_tmp2.add_argument(
-            '--mail-language', dest="external_mail_locale", action="store",
-            help="").completer = Completer("complete_mail_language")
-    parser_tmp2.add_argument(
-        '--welcome', dest="current_welcome_message", action="store",
-        help="welcome message identifier").completer = Completer(
-            "complete_welcome")
-    if api_version < 5:
+    def add_cmd_update_domain(subparsers2):
+        parser_tmp2 = subparsers2.add_parser(
+            'update', help="update domain.")
+        parser_tmp2.add_argument('--label', action="store", help="")
+        parser_tmp2.add_argument('--description', action="store", help="")
         parser_tmp2.add_argument(
-            'identifier', action="store", help="").completer = Completer()
-        parser_tmp2.set_defaults(__func__=DomainsUpdateCommand(config))
-    else:
+            '--role', dest="role", action="store",
+            help="").completer = Completer("complete_role")
         parser_tmp2.add_argument(
-            'uuid', action="store", help="").completer = Completer()
-        parser_tmp2.set_defaults(__func__=DomainsUpdateV5Command(config))
+            '--language', dest="language", action="store",
+            help="").completer = Completer("complete_language")
+        if api_version >= 1:
+            parser_tmp2.add_argument(
+                '--mail-language', dest="external_mail_locale", action="store",
+                help="").completer = Completer("complete_mail_language")
+        parser_tmp2.add_argument(
+            '--welcome', dest="current_welcome_message", action="store",
+            help="welcome message identifier").completer = Completer(
+                "complete_welcome")
+        if api_version < 5:
+            parser_tmp2.add_argument(
+                'identifier', action="store", help="").completer = Completer()
+            parser_tmp2.set_defaults(__func__=DomainsUpdateCommand(config))
+        else:
+            parser_tmp2.add_argument(
+                'uuid', action="store", help="").completer = Completer()
+            parser_tmp2.set_defaults(__func__=DomainsUpdateV5Command(config))
 
     # command : delete
     parser_tmp2 = subparsers2.add_parser(
         'delete', help="delete domain.")
     if api_version == 0:
         parser_tmp2.add_argument(
             'identifier',
@@ -662,10 +681,12 @@
             'cleanup', help="clean user provider.")
         parser_tmp2.add_argument(
             'identifier', action="store",
             help="domain identifier").completer = Completer()
         parser_tmp2.set_defaults(__func__=DomainProvidersDeleteCommand(config))
 
     if api_version < 5:
+        add_cmd_create_domain(subparsers2)
+        add_cmd_update_domain(subparsers2)
         add_cmd_set_provider(subparsers2)
         add_cmd_update_provider(subparsers2)
         add_cmd_delete_provider(subparsers2)
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/domainpolicies.py` & `linsharecli-1.1.3/linsharecli/admin/domainpolicies.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,16 @@
         act = DPDeleteAction()
         act.init(args, self.ls, self.ls.domain_policies)
         return act.delete(args.identifiers)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all domain policies sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list',
         help="list domain policies")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/dpattern.py` & `linsharecli-1.1.3/linsharecli/admin/dpattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,16 @@
             identifier = 'identifier'
         return (v.get(identifier)
                 for v in json_obj if v.get(identifier).startswith(prefix))
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all domain pattern sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     # pylint: disable=too-many-statements
     api_version = config.server.api_version.value
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/func.py` & `linsharecli-1.1.3/linsharecli/admin/func.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/admin/iuser.py` & `linsharecli-1.1.3/linsharecli/admin/iuser.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,16 @@
             self.MSG_RS_UPDATED,
             args.identifier,
             rbu.to_resource())
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all user sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
     # api_version = config.server.api_version.value
 
     # command : list
     parser = subparsers2.add_parser(
         'list',
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/jwt.py` & `linsharecli-1.1.3/linsharecli/admin/jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,16 @@
         super(JwtDeleteCommand, self).__call__(args)
         cli = self.ls.jwt
         return self._delete_all(args, cli, args.uuids)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all Jwt token sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser = subparsers.add_parser(name, help=desc)
     subparsers2 = parser.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list Jwt token.")
     parser.add_argument('identifiers', nargs="*", help="")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/ldap.py` & `linsharecli-1.1.3/linsharecli/admin/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,16 @@
                 cli,
                 args.identifier)
         return self._delete_all(args, cli, args.uuids)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all ldap connections sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     api_version = config.server.api_version.value
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list ldap connections.")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/mail_activations.py` & `linsharecli-1.1.3/linsharecli/admin/mail_activations.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,14 +357,16 @@
         const="ENABLE",
         dest="status")
     add_parser_options(actions_group, "Configuration Policy", "cp-")
 
 def add_parser(subparsers, name, desc, config):
     """Add all domain sub commands."""
     # pylint: disable=too-many-statements
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list mail_activations.")
     parser.add_argument('identifiers', nargs="*")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/mail_attachments.py` & `linsharecli-1.1.3/linsharecli/admin/mail_attachments.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,20 @@
 from linsharecli.admin.core import DefaultCommand
 
 
 class CreateOneAction(CCreateOneAction):
     """TODO"""
 
     def __init__(self, command, cli):
-        super(CreateAction, self).__init__(command, cli)
+        super(CCreateOneAction, self).__init__(command, cli)
         self.logo = None
         self.name = None
 
     def load(self, args):
-        super(CreateAction, self).load(args)
+        super(CCreateOneAction, self).load(args)
         self.logo = args.logo
         self.name = args.name
         return self
 
     def _execute(self, data):
         if data is None:
             data = self.rbu.to_resource()
@@ -166,14 +166,16 @@
         act.rbu = endpoint.get_rbu()
         act.rbu.copy(endpoint.get(args.uuid))
         return act.load(args).execute()
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all mail configs commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     parser_tmp.add_argument(
         'mail_config',
         help="Mail config uuid"
     ).completer = Completer("complete_configs")
 
     subparsers2 = parser_tmp.add_subparsers()
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/mail_configs.py` & `linsharecli-1.1.3/linsharecli/admin/mail_configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,14 +86,16 @@
         )
         json_obj = endpoint.list(args.domain, args.parent)
         return tbu.build().load_v2(json_obj).render()
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all mail configs commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list mail configs")
     parser.add_argument('identifiers', nargs="*", help="")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/public_keys.py` & `linsharecli-1.1.3/linsharecli/admin/public_keys.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         super(PublicKeyDeleteCommand, self).__call__(args)
         cli = self.ls.public_keys
         return self._delete_all(args, cli, args.uuids)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all public key sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list public key.")
     parser.add_argument('identifiers', nargs="*", help="")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/shared_space_members.py` & `linsharecli-1.1.3/linsharecli/admin/shared_space_members.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/admin/shared_spaces.py` & `linsharecli-1.1.3/linsharecli/admin/shared_spaces.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/admin/threads.py` & `linsharecli-1.1.3/linsharecli/admin/threads.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         super(ThreadsListCommand, self).__call__(args)
         cli = self.ls.threads
         return cli.get_rbu().get_keys(True)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all thread sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list',
         help="list threads from linshare")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/tmembers.py` & `linsharecli-1.1.3/linsharecli/admin/tmembers.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,16 @@
         super(ThreadMembersListCommand, self).__call__(args)
         cli = self.ls.thread_members
         return cli.get_rbu().get_keys(True)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all thread member sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
 
     subparsers2 = parser_tmp.add_subparsers()
     parser = subparsers2.add_parser(
         'list',
         help="list thread members.")
     parser.add_argument(
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/upgrade_tasks.py` & `linsharecli-1.1.3/linsharecli/admin/upgrade_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,16 @@
             self.log.debug("can trigger upgrade task : %s", args.identifier, exc_info=1)
             self.log.error(ex.args)
         return False
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all upgrade tasks sub commands."""
-    # api_version = config.server.api_version.value
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list all upgrade tasks.")
     parser.add_argument('identifier', nargs="?",
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/user.py` & `linsharecli-1.1.3/linsharecli/admin/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,14 +54,16 @@
         super(UsersListCommand, self).__call__(args)
         cli = self.ls.users
         return cli.get_rbu().get_keys(True)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all user sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
 
     subparsers2 = parser_tmp.add_subparsers()
     parser_tmp2 = subparsers2.add_parser('list',
                                          help="list users from linshare")
     parser_tmp2.add_argument('-f', '--firstname', action="store")
     parser_tmp2.add_argument('-l', '--lastname', action="store")
```

### Comparing `linsharecli-1.1.2/linsharecli/admin/welcome_messages.py` & `linsharecli-1.1.3/linsharecli/admin/welcome_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,16 @@
         super(WelcomeMessagesDeleteCommand, self).__call__(args)
         cli = self.ls.welcome_messages
         return self._delete_all(args, cli, args.uuids)
 
 
 def add_parser(subparsers, name, desc, config):
     """Add all welcome message sub commands."""
+    if config.server.api_version.value >= 5:
+        return
     parser_tmp = subparsers.add_parser(name, help=desc)
     subparsers2 = parser_tmp.add_subparsers()
 
     # command : list
     parser = subparsers2.add_parser(
         'list', help="list welcome message.")
     parser.add_argument('identifiers', nargs="*", help="")
```

### Comparing `linsharecli-1.1.2/linsharecli/common/__init__.py` & `linsharecli-1.1.3/linsharecli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 #
 # Copyright 2014 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
+
+__version__ = '1.1.3'
```

### Comparing `linsharecli-1.1.2/linsharecli/common/actions.py` & `linsharecli-1.1.3/linsharecli/common/actions.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/common/cell.py` & `linsharecli-1.1.3/linsharecli/common/cell.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/common/core.py` & `linsharecli-1.1.3/linsharecli/common/core.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/common/tables.py` & `linsharecli-1.1.3/linsharecli/common/tables.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/tests/core.py` & `linsharecli-1.1.3/linsharecli/tests/core.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/tests/documents.py` & `linsharecli-1.1.3/linsharecli/tests/documents.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/tests/misc.py` & `linsharecli-1.1.3/linsharecli/tests/misc.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/tests/threads.py` & `linsharecli-1.1.3/linsharecli/tests/threads.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/__init__.py` & `linsharecli-1.1.3/linsharecli/user/__init__.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/audit.py` & `linsharecli-1.1.3/linsharecli/user/audit.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/contactslists.py` & `linsharecli-1.1.3/linsharecli/user/contactslists.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/contactslistscontacts.py` & `linsharecli-1.1.3/linsharecli/user/contactslistscontacts.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/core.py` & `linsharecli-1.1.3/linsharecli/user/core.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/documents.py` & `linsharecli-1.1.3/linsharecli/user/documents.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/guests.py` & `linsharecli-1.1.3/linsharecli/user/guests.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/jwt.py` & `linsharecli-1.1.3/linsharecli/user/jwt.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/rshares.py` & `linsharecli-1.1.3/linsharecli/user/rshares.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/shared_space_audit.py` & `linsharecli-1.1.3/linsharecli/user/shared_space_audit.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/shared_space_members.py` & `linsharecli-1.1.3/linsharecli/user/shared_space_members.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/shared_spaces.py` & `linsharecli-1.1.3/linsharecli/user/shared_spaces.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/shares.py` & `linsharecli-1.1.3/linsharecli/user/shares.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/users.py` & `linsharecli-1.1.3/linsharecli/user/users.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/wg_documents.py` & `linsharecli-1.1.3/linsharecli/user/wg_documents.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/wg_members.py` & `linsharecli-1.1.3/linsharecli/user/wg_members.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli/user/workgroups.py` & `linsharecli-1.1.3/linsharecli/user/workgroups.py`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/linsharecli.egg-info/PKG-INFO` & `linsharecli-1.1.3/linsharecli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: linsharecli
-Version: 1.1.2
+Version: 1.1.3
 Summary: LinShare command line interface.
 Home-page: https://github.com/fred49/linshare-cli
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
@@ -95,9 +94,7 @@
 ``$ linshareadmcli -s my-second-config domains list``
 
 You can also list all available configurations using:
 
 ``$ linshareadmcli list``
 
 
-
-
```

### Comparing `linsharecli-1.1.2/linsharecli.egg-info/SOURCES.txt` & `linsharecli-1.1.3/linsharecli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linsharecli-1.1.2/setup.py` & `linsharecli-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,11 +87,11 @@
 
     # List run-time dependencies here.  These will be installed by pip when your
     # project is installed.
     install_requires=[
         'argtoolbox>=1.1.4,<1.2.0',
         'linshareapi>=1.0.10,<1.1.0',
         'progressbar2',
-        'vhatable>=1.0.0,<1.1.0',
+        'vhatable>=1.0.0,<1.2.0',
         'mock==2.0.0',
     ],
 )
```

