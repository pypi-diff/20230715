# Comparing `tmp/gitlabform-3.6.1.tar.gz` & `tmp/gitlabform-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.6.1.tar", last modified: Thu Jul 13 08:00:12 2023, max compression
+gzip compressed data, was "gitlabform-3.7.0.tar", last modified: Sat Jul 15 14:46:17 2023, max compression
```

## Comparing `gitlabform-3.6.1.tar` & `gitlabform-3.7.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-13 08:00:09.000000 gitlabform-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 08:00:12.483162 gitlabform-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-13 08:00:09.000000 gitlabform-3.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.471162 gitlabform-3.6.1/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.475162 gitlabform-3.6.1/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.475162 gitlabform-3.6.1/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 08:00:09.000000 gitlabform-3.6.1/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.467162 gitlabform-3.6.1/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-13 08:00:12.000000 gitlabform-3.6.1/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-13 08:00:12.487162 gitlabform-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-13 08:00:09.000000 gitlabform-3.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.479162 gitlabform-3.6.1/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8047 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4136 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_badges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9639 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10353 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7264 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5045 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_token_from_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5559 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:12.483162 gitlabform-3.6.1/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-13 08:00:09.000000 gitlabform-3.6.1/tests/unit/test_non_empty_configs_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.416719 gitlabform-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-15 14:46:14.000000 gitlabform-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-15 14:46:17.416719 gitlabform-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-15 14:46:14.000000 gitlabform-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.400719 gitlabform-3.7.0/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (123)    23870 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.400719 gitlabform-3.7.0/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12541 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15180 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.408719 gitlabform-3.7.0/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.408719 gitlabform-3.7.0/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.408719 gitlabform-3.7.0/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.408719 gitlabform-3.7.0/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14003 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-15 14:46:14.000000 gitlabform-3.7.0/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.400719 gitlabform-3.7.0/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 14:46:17.000000 gitlabform-3.7.0/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-15 14:46:17.416719 gitlabform-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-15 14:46:14.000000 gitlabform-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8047 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1951 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4136 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9639 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      882 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5622 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10353 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2071 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2231 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      544 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1664 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10507 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5045 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_token_from_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5559 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.412719 gitlabform-3.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.416719 gitlabform-3.7.0/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3042 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:17.416719 gitlabform-3.7.0/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-15 14:46:14.000000 gitlabform-3.7.0/tests/unit/test_non_empty_configs_provider.py
```

### Comparing `gitlabform-3.6.1/LICENSE` & `gitlabform-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/PKG-INFO` & `gitlabform-3.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.6.1
+Version: 3.7.0
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.6.1 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.7.0 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.6.1/README.md` & `gitlabform-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/__init__.py` & `gitlabform-3.7.0/gitlabform/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/configuration/common.py` & `gitlabform-3.7.0/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/configuration/core.py` & `gitlabform-3.7.0/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/configuration/groups.py` & `gitlabform-3.7.0/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/configuration/projects.py` & `gitlabform-3.7.0/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/configuration/transform.py` & `gitlabform-3.7.0/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/__init__.py` & `gitlabform-3.7.0/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/branches.py` & `gitlabform-3.7.0/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/commits.py` & `gitlabform-3.7.0/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/core.py` & `gitlabform-3.7.0/gitlabform/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/group_badges.py` & `gitlabform-3.7.0/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.7.0/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/group_variables.py` & `gitlabform-3.7.0/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/groups.py` & `gitlabform-3.7.0/gitlabform/gitlab/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/integrations.py` & `gitlabform-3.7.0/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/members.py` & `gitlabform-3.7.0/gitlabform/gitlab/members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.7.0/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/pipelines.py` & `gitlabform-3.7.0/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/project_badges.py` & `gitlabform-3.7.0/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.7.0/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.7.0/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.7.0/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/projects.py` & `gitlabform-3.7.0/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/repositories.py` & `gitlabform-3.7.0/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.7.0/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/schedules.py` & `gitlabform-3.7.0/gitlabform/gitlab/schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/tags.py` & `gitlabform-3.7.0/gitlabform/gitlab/tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/users.py` & `gitlabform-3.7.0/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/gitlab/variables.py` & `gitlabform-3.7.0/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/lists/__init__.py` & `gitlabform-3.7.0/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/lists/filter.py` & `gitlabform-3.7.0/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/lists/groups.py` & `gitlabform-3.7.0/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/lists/projects.py` & `gitlabform-3.7.0/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/output.py` & `gitlabform-3.7.0/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/__init__.py` & `gitlabform-3.7.0/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/abstract_processor.py` & `gitlabform-3.7.0/gitlabform/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/defining_keys.py` & `gitlabform-3.7.0/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/group/__init__.py` & `gitlabform-3.7.0/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.7.0/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.7.0/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.7.0/gitlabform/processors/group/group_members_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
             )
             if proper_users_to_set_by_username:
                 users_to_set_by_username = proper_users_to_set_by_username
             else:
                 users_to_set_by_username.pop("enforce", None)
                 users_to_set_by_username.pop("users", None)
                 users_to_set_by_username.pop("groups", None)
+                users_to_set_by_username.pop("keep_bots", None)
 
         return groups_to_set_by_group_path, users_to_set_by_username
 
     def _process_groups(
         self, group: str, groups_to_set_by_group_path: dict, enforce_group_members: bool
     ):
         # group users before by group name
```

### Comparing `gitlabform-3.6.1/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.7.0/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.7.0/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/__init__.py` & `gitlabform-3.7.0/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/files_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/members_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.7.0/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.7.0/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/project_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/schedules_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/schedules_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,30 @@
 
 
 class SchedulesProcessor(AbstractProcessor):
     def __init__(self, gitlab: GitLab):
         super().__init__("schedules", gitlab)
 
     def _process_configuration(self, project_and_group: str, configuration: dict):
+        configured_schedules = configuration.get("schedules", {})
+        enforce_schedules = configuration.get("schedules|enforce", False)
+
+        # Remove 'enforce' key from the config so that it's not treated as a "schedule"
+        if enforce_schedules:
+            configured_schedules.pop("enforce")
+
         existing_schedules = self.gitlab.get_all_pipeline_schedules(project_and_group)
         schedule_ids_by_description = self.__group_schedule_ids_by_description(
             existing_schedules
         )
 
-        for schedule_description in sorted(configuration["schedules"]):
+        for schedule_description in sorted(configured_schedules):
             schedule_ids = schedule_ids_by_description.get(schedule_description)
-            if configuration.get("schedules|" + schedule_description + "|delete"):
+
+            if configured_schedules[schedule_description].get("delete"):
                 if schedule_ids:
                     debug("Deleting pipeline schedules '%s'", schedule_description)
                     for schedule_id in schedule_ids:
                         self.gitlab.delete_pipeline_schedule(
                             project_and_group, schedule_id
                         )
                 else:
@@ -62,14 +70,29 @@
                     )
                 else:
                     debug("Creating pipeline schedule '%s'", schedule_description)
                     self.create_schedule_with_variables(
                         configuration, project_and_group, schedule_description
                     )
 
+        if enforce_schedules:
+            debug("Delete unconfigured schedules because enforce is enabled")
+
+            for schedule in existing_schedules:
+                schedule_description = schedule["description"]
+                schedule_id = schedule["id"]
+
+                debug(f"processing {schedule_id}: {schedule_description}")
+                if schedule_description not in configured_schedules:
+                    debug(
+                        "Deleting pipeline schedule named '%s', because it is not in gitlabform configuration",
+                        schedule_description,
+                    )
+                    self.gitlab.delete_pipeline_schedule(project_and_group, schedule_id)
+
     def create_schedule_with_variables(
         self, configuration, project_and_group, schedule_description
     ):
         data = configuration.get("schedules|" + schedule_description)
         created_schedule = self.gitlab.create_pipeline_schedule(
             project_and_group,
             schedule_description,
```

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.7.0/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.7.0/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.7.0/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.7.0/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/util/decorators.py` & `gitlabform-3.7.0/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.7.0/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.7.0/gitlabform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.6.1
+Version: 3.7.0
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.6.1 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.7.0 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
```

### Comparing `gitlabform-3.6.1/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.7.0/gitlabform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/setup.py` & `gitlabform-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/__init__.py` & `gitlabform-3.7.0/tests/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/conftest.py` & `gitlabform-3.7.0/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_badges.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_branches.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_files.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_files_all.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_group_members_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,7 +228,34 @@
         run_gitlabform(add_shared_with, group)
 
         members = group.members.list()
         assert len(members) == no_of_members_before, members
 
         shared_with = gl.groups.get(group.id).shared_with_groups
         assert len(shared_with) == 2
+
+    def test__ignore_keep_bots_and_enforce(self, gl, group, users, groups, one_owner):
+        no_of_members_before = len(group.members.list())
+
+        add_shared_with = f"""
+            projects_and_groups:
+              {group.full_path}/*:
+                group_members:
+                  enforce: true
+                  keep_bots: true
+                  users:
+                  {users[0].username}:
+                    access_level: owner
+                  groups:
+                    {groups[0].full_path}:
+                      group_access: developer
+                    {groups[1].full_path}:
+                      group_access: developer
+            """
+
+        run_gitlabform(add_shared_with, group)
+
+        members = group.members.list()
+        assert len(members) == no_of_members_before, members
+
+        shared_with = gl.groups.get(group.id).shared_with_groups
+        assert len(shared_with) == 2
```

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_members.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_project_settings.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_running.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_running.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_schedules.py`

 * *Files 27% similar despite different names*

```diff
@@ -195,14 +195,103 @@
         run_gitlabform(delete_schedule, project)
 
         schedule = self.__find_pipeline_schedule_by_description_and_get_first(
             project, "Redundant schedule"
         )
         assert schedule is None
 
+    def test__schedule_enforce_new_schedule(self, project, schedules):
+        new_schedule = f"""
+        projects_and_groups:
+          {project.path_with_namespace}:
+            schedules:
+              enforce: true
+              "New schedule to test enforce config":
+                ref: main
+                cron: "30 1 * * *"
+        """
+
+        schedules_before = project.pipelineschedules.list()
+
+        run_gitlabform(new_schedule, project)
+
+        schedules_after = project.pipelineschedules.list()
+
+        schedule = self.__find_pipeline_schedule_by_description_and_get_first(
+            project, "New schedule to test enforce config"
+        )
+        assert len(schedules_before) == 6
+        assert len(schedules_after) == 1
+        assert schedule is not None
+        assert schedule.description == "New schedule to test enforce config"
+        assert schedule.ref == "main"
+        assert schedule.cron == "30 1 * * *"
+        assert schedule.cron_timezone == "UTC"
+        assert schedule.active is True
+
+    def test__schedule_enforce_new_and_existing_schedule(self, project, schedules):
+        new_schedule = f"""
+        projects_and_groups:
+          {project.path_with_namespace}:
+            schedules:
+              enforce: true
+              "New schedule to test enforce config":
+                ref: main
+                cron: "30 1 * * *"
+              "New schedule with variables":
+                ref: main
+                cron: "30 1 * * *"
+                variables:
+                    var1:
+                        value: value123
+                    var2:
+                        value: value987
+                        variable_type: file
+        """
+
+        schedules_before = project.pipelineschedules.list()
+
+        run_gitlabform(new_schedule, project)
+
+        schedules_after = project.pipelineschedules.list()
+
+        schedule1 = self.__find_pipeline_schedule_by_description_and_get_first(
+            project, "New schedule to test enforce config"
+        )
+        schedule2 = self.__find_pipeline_schedule_by_description_and_get_first(
+            project, "New schedule with variables"
+        )
+        assert len(schedules_before) == 1
+        assert len(schedules_after) == 2
+
+        assert schedule1 is not None
+        assert schedule1.description == "New schedule to test enforce config"
+        assert schedule1.ref == "main"
+        assert schedule1.cron == "30 1 * * *"
+        assert schedule1.cron_timezone == "UTC"
+        assert schedule1.active is True
+
+        assert schedule2 is not None
+        assert schedule2.description == "New schedule with variables"
+        assert schedule2.ref == "main"
+        assert schedule2.cron == "30 1 * * *"
+        assert schedule2.cron_timezone == "UTC"
+        assert schedule2.active is True
+
+        variables = schedule2.attributes["variables"]
+        assert variables is not None
+        assert len(variables) == 2
+        assert variables[0]["variable_type"] == "env_var"
+        assert variables[0]["key"] == "var1"
+        assert variables[0]["value"] == "value123"
+
+        assert variables[1]["variable_type"] == "file"
+        assert variables[1]["key"] == "var2"
+        assert variables[1]["value"] == "value987"
+
     @classmethod
     def __find_pipeline_schedule_by_description_and_get_first(
         cls, project, description
     ):
         try:
             return cls.__find_pipeline_schedules_by_description(project, description)[0]
         except IndexError:
```

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_tags.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/acceptance/standard/test_variables.py` & `gitlabform-3.7.0/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.7.0/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.7.0/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.7.0/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.7.0/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.7.0/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.7.0/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.7.0/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.7.0/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.7.0/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/test_access_levels.py` & `gitlabform-3.7.0/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.6.1/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.7.0/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

