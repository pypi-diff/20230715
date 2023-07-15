# Comparing `tmp/netbox-cisco-support-plugin-0.0.60.tar.gz` & `tmp/netbox-cisco-support-plugin-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-cisco-support-plugin-0.0.60.tar", last modified: Mon Jul 10 12:54:51 2023, max compression
+gzip compressed data, was "netbox-cisco-support-plugin-0.0.61.tar", last modified: Sat Jul 15 15:29:06 2023, max compression
```

## Comparing `netbox-cisco-support-plugin-0.0.60.tar` & `netbox-cisco-support-plugin-0.0.61.tar`

### file list

```diff
@@ -1,61 +1,55 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/
--rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)    13503 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    12856 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.572923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1797 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/admin.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/serializers.py
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/views.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/filtersets.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/forms.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/commands/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/commands/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37347 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/
--rw-r--r--   0 vsts      (1001) docker     (123)     3497 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0001_initial.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)      400 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
--rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1102 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
--rw-r--r--   0 vsts      (1001) docker     (123)      480 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0006_alter_ciscodevicesupport_partner_coverage_end_date.py
--rw-r--r--   0 vsts      (1001) docker     (123)      487 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0007_alter_ciscodevicesupport_recommended_release.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    32243 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/models.py
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/navigation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3938 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3679 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/template_content.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.572923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
--rw-r--r--   0 vsts      (1001) docker     (123)     6716 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
--rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/
--rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_partner_contract_coverage_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)     1078 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eorfa_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)      888 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eos_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eoscr_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)     1030 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosm_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)      966 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvca_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)     1046 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvs_bar.html
--rw-r--r--   0 vsts      (1001) docker     (123)      950 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_last_day_support_bar.html
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templatetags/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templatetags/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2960 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templatetags/filters.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/urls.py
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/version.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1709 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/views.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-10 12:54:51.572923 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)    13503 2023-07-10 12:54:51.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2945 2023-07-10 12:54:51.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-10 12:54:51.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-10 12:54:51.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-07-10 12:54:51.000000 netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-10 12:54:51.576923 netbox-cisco-support-plugin-0.0.60/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-07-10 12:54:29.000000 netbox-cisco-support-plugin-0.0.60/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1068 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (123)       62 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)    13503 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    12856 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)      686 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1797 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/admin.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2424 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/serializers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      695 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/views.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4395 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/filtersets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10150 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/forms.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/commands/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/commands/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    37347 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/migrations/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5190 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/migrations/0001_initial.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/migrations/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    32243 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/models.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/navigation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3938 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3679 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/template_content.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6716 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/
+-rw-r--r--   0 vsts      (1001) docker     (123)      832 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_partner_contract_coverage_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     1078 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eorfa_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      888 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eos_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     1038 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eoscr_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     1030 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosm_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      966 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvca_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)     1046 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvs_bar.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      950 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_last_day_support_bar.html
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templatetags/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templatetags/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2960 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templatetags/filters.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1105 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/urls.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1709 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/views.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-07-15 15:29:06.468660 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)    13503 2023-07-15 15:29:06.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2388 2023-07-15 15:29:06.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 15:29:06.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-07-15 15:29:06.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       28 2023-07-15 15:29:06.000000 netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-07-15 15:29:06.472660 netbox-cisco-support-plugin-0.0.61/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1568 2023-07-15 15:28:48.000000 netbox-cisco-support-plugin-0.0.61/setup.py
```

### Comparing `netbox-cisco-support-plugin-0.0.60/LICENSE` & `netbox-cisco-support-plugin-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/PKG-INFO` & `netbox-cisco-support-plugin-0.0.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.60
+Version: 0.0.61
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.60/README.md` & `netbox-cisco-support-plugin-0.0.61/README.md`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/__init__.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/admin.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/admin.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/serializers.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/api/views.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/filtersets.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/forms.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/migrations/0001_initial.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,83 @@
-# Generated by Django 4.1.9 on 2023-06-06 12:19
+# Generated by Django 4.1.9 on 2023-07-15 15:14
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
-        ("dcim", "0171_cabletermination_change_logging"),
+        ('dcim', '0172_larger_power_draw_values'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name="CiscoSupport",
+            name='CiscoDeviceTypeSupport',
             fields=[
-                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
-                ("created", models.DateTimeField(auto_now_add=True, null=True)),
-                ("last_updated", models.DateTimeField(auto_now=True, null=True)),
-                ("coverage_end_date", models.DateField(blank=True, null=True)),
-                ("service_contract_number", models.TextField(blank=True, null=True)),
-                ("service_line_descr", models.TextField(blank=True, null=True)),
-                ("warranty_type", models.TextField(blank=True, null=True)),
-                ("warranty_end_date", models.DateField(blank=True, null=True)),
-                ("is_covered", models.BooleanField(default=False)),
-                ("sr_no_owner", models.BooleanField(default=False)),
-                ("contract_supplier", models.TextField(blank=True, null=True)),
-                ("api_status", models.TextField(blank=True, null=True)),
-                ("recommended_release", models.TextField(blank=True, null=True)),
-                ("desired_release", models.TextField(blank=True, null=True)),
-                ("current_release", models.TextField(blank=True, null=True)),
-                ("desired_release_status", models.BooleanField(default=False)),
-                ("current_release_status", models.BooleanField(default=False)),
-                (
-                    "device",
-                    models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to="dcim.device"),
-                ),
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
+                ('created', models.DateTimeField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
+                ('name', models.CharField(blank=True, max_length=100, null=True)),
+                ('pid', models.CharField(blank=True, max_length=100, null=True)),
+                ('eox_has_error', models.BooleanField(default=False)),
+                ('eox_error', models.CharField(blank=True, max_length=100, null=True)),
+                ('eox_announcement_date', models.DateField(blank=True, null=True)),
+                ('end_of_sale_date', models.DateField(blank=True, null=True)),
+                ('end_of_sw_maintenance_releases', models.DateField(blank=True, null=True)),
+                ('end_of_security_vul_support_date', models.DateField(blank=True, null=True)),
+                ('end_of_routine_failure_analysis_date', models.DateField(blank=True, null=True)),
+                ('end_of_service_contract_renewal', models.DateField(blank=True, null=True)),
+                ('end_of_svc_attach_date', models.DateField(blank=True, null=True)),
+                ('last_date_of_support', models.DateField(blank=True, null=True)),
+                ('device_type', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to='dcim.devicetype')),
             ],
             options={
-                "abstract": False,
+                'abstract': False,
             },
         ),
         migrations.CreateModel(
-            name="CiscoDeviceTypeSupport",
+            name='CiscoDeviceSupport',
             fields=[
-                ("id", models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
-                ("created", models.DateTimeField(auto_now_add=True, null=True)),
-                ("last_updated", models.DateTimeField(auto_now=True, null=True)),
-                ("eox_has_error", models.BooleanField(default=False)),
-                ("eox_error", models.TextField(blank=True, null=True)),
-                ("eox_announcement_date", models.DateField(blank=True, null=True)),
-                ("end_of_sale_date", models.DateField(blank=True, null=True)),
-                ("end_of_sw_maintenance_releases", models.DateField(blank=True, null=True)),
-                ("end_of_security_vul_support_date", models.DateField(blank=True, null=True)),
-                ("end_of_routine_failure_analysis_date", models.DateField(blank=True, null=True)),
-                ("end_of_service_contract_renewal", models.DateField(blank=True, null=True)),
-                ("last_date_of_support", models.DateField(blank=True, null=True)),
-                ("end_of_svc_attach_date", models.DateField(blank=True, null=True)),
-                (
-                    "device_type",
-                    models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to="dcim.devicetype"),
-                ),
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False)),
+                ('created', models.DateTimeField(auto_now_add=True, null=True)),
+                ('last_updated', models.DateTimeField(auto_now=True, null=True)),
+                ('name', models.CharField(blank=True, max_length=100, null=True)),
+                ('serial', models.CharField(blank=True, max_length=100, null=True)),
+                ('coverage_end_date', models.DateField(blank=True, null=True)),
+                ('service_contract_number', models.CharField(blank=True, max_length=100, null=True)),
+                ('service_line_descr', models.CharField(blank=True, max_length=100, null=True)),
+                ('warranty_type', models.CharField(blank=True, max_length=100, null=True)),
+                ('warranty_end_date', models.DateField(blank=True, null=True)),
+                ('is_covered', models.BooleanField(default=False)),
+                ('sr_no_owner', models.BooleanField(default=False)),
+                ('contract_supplier', models.CharField(blank=True, max_length=100, null=True)),
+                ('api_status', models.CharField(blank=True, max_length=100, null=True)),
+                ('recommended_release', models.TextField(blank=True, max_length=100, null=True)),
+                ('desired_release', models.CharField(blank=True, max_length=100, null=True)),
+                ('current_release', models.CharField(blank=True, max_length=100, null=True)),
+                ('desired_release_status', models.BooleanField(default=False)),
+                ('current_release_status', models.BooleanField(default=False)),
+                ('partner_status', models.CharField(blank=True, max_length=100, null=True)),
+                ('partner_service_level', models.CharField(blank=True, max_length=100, null=True)),
+                ('partner_customer_number', models.CharField(blank=True, max_length=100, null=True)),
+                ('partner_coverage_end_date', models.DateField(blank=True, null=True)),
+                ('pid', models.CharField(blank=True, max_length=100, null=True)),
+                ('eox_has_error', models.BooleanField(default=False)),
+                ('eox_error', models.CharField(blank=True, max_length=100, null=True)),
+                ('eox_announcement_date', models.DateField(blank=True, null=True)),
+                ('end_of_sale_date', models.DateField(blank=True, null=True)),
+                ('end_of_sw_maintenance_releases', models.DateField(blank=True, null=True)),
+                ('end_of_security_vul_support_date', models.DateField(blank=True, null=True)),
+                ('end_of_routine_failure_analysis_date', models.DateField(blank=True, null=True)),
+                ('end_of_service_contract_renewal', models.DateField(blank=True, null=True)),
+                ('end_of_svc_attach_date', models.DateField(blank=True, null=True)),
+                ('last_date_of_support', models.DateField(blank=True, null=True)),
+                ('device', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to='dcim.device')),
             ],
             options={
-                "abstract": False,
+                'abstract': False,
             },
         ),
-    ]
+    ]
```

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/models.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/models.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/tables.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/template_content.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_contract_coverage_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_partner_contract_coverage_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_partner_contract_coverage_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eorfa_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eorfa_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eos_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eos_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eoscr_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eoscr_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosm_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosm_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvca_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvca_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvs_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eosvs_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_last_day_support_bar.html` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_last_day_support_bar.html`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/templatetags/filters.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/templatetags/filters.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/urls.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin/views.py` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin/views.py`

 * *Files identical despite different names*

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/PKG-INFO` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-cisco-support-plugin
-Version: 0.0.60
+Version: 0.0.61
 Summary: Cisco device support, device type support, and software release information with the Cisco support APIs
 Author: Willi Kubny
 Author-email: willi.kubny@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Information Technology
```

### Comparing `netbox-cisco-support-plugin-0.0.60/netbox_cisco_support_plugin.egg-info/SOURCES.txt` & `netbox-cisco-support-plugin-0.0.61/netbox_cisco_support_plugin.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -22,20 +22,14 @@
 netbox_cisco_support_plugin/api/serializers.py
 netbox_cisco_support_plugin/api/urls.py
 netbox_cisco_support_plugin/api/views.py
 netbox_cisco_support_plugin/management/__init__.py
 netbox_cisco_support_plugin/management/commands/__init__.py
 netbox_cisco_support_plugin/management/commands/sync_cisco_support_data.py
 netbox_cisco_support_plugin/migrations/0001_initial.py
-netbox_cisco_support_plugin/migrations/0002_ciscodevicesupport_and_more.py
-netbox_cisco_support_plugin/migrations/0003_rename_model_ciscodevicesupport_pid.py
-netbox_cisco_support_plugin/migrations/0004_ciscodevicesupport_name_ciscodevicetypesupport_name_and_more.py
-netbox_cisco_support_plugin/migrations/0005_ciscodevicesupport_partner_coverage_end_date_and_more.py
-netbox_cisco_support_plugin/migrations/0006_alter_ciscodevicesupport_partner_coverage_end_date.py
-netbox_cisco_support_plugin/migrations/0007_alter_ciscodevicesupport_recommended_release.py
 netbox_cisco_support_plugin/migrations/__init__.py
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device.html
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/cisco_support_device_type.html
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_contract_coverage_bar.html
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_partner_contract_coverage_bar.html
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eorfa_bar.html
 netbox_cisco_support_plugin/templates/netbox_cisco_support_plugin/inc/device_type_eos_bar.html
```

### Comparing `netbox-cisco-support-plugin-0.0.60/setup.py` & `netbox-cisco-support-plugin-0.0.61/setup.py`

 * *Files identical despite different names*

