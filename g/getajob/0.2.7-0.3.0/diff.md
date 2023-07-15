# Comparing `tmp/getajob-0.2.7.tar.gz` & `tmp/getajob-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getajob-0.2.7.tar", max compression
+gzip compressed data, was "getajob-0.3.0.tar", max compression
```

## Comparing `getajob-0.2.7.tar` & `getajob-0.3.0.tar`

### file list

```diff
@@ -1,83 +1,116 @@
--rw-r--r--   0        0        0    11357 2023-06-13 02:01:30.836240 getajob-0.2.7/LICENSE
--rw-r--r--   0        0        0       69 2023-06-13 02:01:30.840240 getajob-0.2.7/README.md
--rw-r--r--   0        0        0       22 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/abstractions/models.py
--rw-r--r--   0        0        0     8332 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/abstractions/repository.py
--rw-r--r--   0        0        0     1308 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/config/settings.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/__init__.py
--rw-r--r--   0        0        0      141 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/models.py
--rw-r--r--   0        0        0      394 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/search/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/__init__.py
--rw-r--r--   0        0        0      620 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/models.py
--rw-r--r--   0        0        0      598 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/admin/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/__init__.py
--rw-r--r--   0        0        0      823 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/models.py
--rw-r--r--   0        0        0     2470 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/ai/text/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/__init__.py
--rw-r--r--   0        0        0      145 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/models.py
--rw-r--r--   0        0        0      444 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/invitations/repository.py
--rw-r--r--   0        0        0      102 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/models.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/__init__.py
--rw-r--r--   0        0        0      117 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/models.py
--rw-r--r--   0        0        0      402 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/recruiters/repository.py
--rw-r--r--   0        0        0      395 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/companies/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/__init__.py
--rw-r--r--   0        0        0     3021 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/models.py
--rw-r--r--   0        0        0     1120 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/repository.py
--rw-r--r--   0        0        0      462 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/jobs/unit_of_work.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/__init__.py
--rw-r--r--   0        0        0     1155 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/models.py
--rw-r--r--   0        0        0     1556 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/scheduled_events/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/static/__init__.py
--rw-r--r--   0        0        0     1327 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/static/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/__init__.py
--rw-r--r--   0        0        0      277 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/models.py
--rw-r--r--   0        0        0      516 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/cover_letters/repository.py
--rw-r--r--   0        0        0       89 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/models.py
--rw-r--r--   0        0        0      568 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/__init__.py
--rw-r--r--   0        0        0      196 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/models.py
--rw-r--r--   0        0        0      462 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/resumes/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/sessions/__init__.py
--rw-r--r--   0        0        0      306 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/sessions/models.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/__init__.py
--rw-r--r--   0        0        0      404 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/models.py
--rw-r--r--   0        0        0      491 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/contexts/users/skills/repository.py
--rw-r--r--   0        0        0     2318 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/exceptions.py
--rw-r--r--   0        0        0      375 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/utils.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/__init__.py
--rw-r--r--   0        0        0      165 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/aiocron.py
--rw-r--r--   0        0        0      702 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/algolia/models.py
--rw-r--r--   0        0        0     1056 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/algolia/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/__init__.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/__init__.py
--rw-r--r--   0        0        0      894 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/models.py
--rw-r--r--   0        0        0     1848 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/companies/repository.py
--rw-r--r--   0        0        0      103 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/exceptions.py
--rw-r--r--   0        0        0      413 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/models.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/__init__.py
--rw-r--r--   0        0        0      747 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/models.py
--rw-r--r--   0        0        0     2486 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/__init__.py
--rw-r--r--   0        0        0     1748 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/models.py
--rw-r--r--   0        0        0     2774 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/recruiters/repository.py
--rw-r--r--   0        0        0     3101 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/repository.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/__init__.py
--rw-r--r--   0        0        0     1320 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/models.py
--rw-r--r--   0        0        0     1839 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/clerk/users/repository.py
--rw-r--r--   0        0        0     9580 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/firebase.py
--rw-r--r--   0        0        0        0 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/__init__.py
--rw-r--r--   0        0        0      724 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/authentication.py
--rw-r--r--   0        0        0      320 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/exceptions.py
--rw-r--r--   0        0        0     1254 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/kafka.py
--rw-r--r--   0        0        0      221 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/mock.py
--rw-r--r--   0        0        0     1480 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/models.py
--rw-r--r--   0        0        0      589 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/kafka/repository.py
--rw-r--r--   0        0        0     1862 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/openai.py
--rw-r--r--   0        0        0      599 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/sendgrid/sendgrid.py
--rw-r--r--   0        0        0      251 2023-06-13 02:01:30.840240 getajob-0.2.7/getajob/vendor/sentry.py
--rw-r--r--   0        0        0     1742 2023-06-13 02:01:30.844240 getajob-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-15 17:20:29.141148 getajob-0.3.0/LICENSE
+-rw-r--r--   0        0        0       69 2023-07-15 17:20:29.141148 getajob-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/__init__.py
+-rw-r--r--   0        0        0     2372 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/abstractions/models.py
+-rw-r--r--   0        0        0    14436 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/abstractions/repository.py
+-rw-r--r--   0        0        0      383 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/abstractions/vendor_client_factory.py
+-rw-r--r--   0        0        0     1307 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/config/settings.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/search/__init__.py
+-rw-r--r--   0        0        0      141 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/search/models.py
+-rw-r--r--   0        0        0      406 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/search/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/users/__init__.py
+-rw-r--r--   0        0        0      620 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/users/models.py
+-rw-r--r--   0        0        0      684 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/admin/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/applications/__init__.py
+-rw-r--r--   0        0        0      870 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/applications/models.py
+-rw-r--r--   0        0        0     2962 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/applications/repository.py
+-rw-r--r--   0        0        0     2176 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/applications/unit_of_work.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/details/__init__.py
+-rw-r--r--   0        0        0      658 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/details/models.py
+-rw-r--r--   0        0        0      686 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/details/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/invitations/__init__.py
+-rw-r--r--   0        0        0      145 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/invitations/models.py
+-rw-r--r--   0        0        0      653 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/invitations/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/jobs/__init__.py
+-rw-r--r--   0        0        0     4842 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/jobs/models.py
+-rw-r--r--   0        0        0     1200 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/jobs/repository.py
+-rw-r--r--   0        0        0      454 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/jobs/unit_of_work.py
+-rw-r--r--   0        0        0      102 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/models.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/recruiters/__init__.py
+-rw-r--r--   0        0        0      117 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/recruiters/models.py
+-rw-r--r--   0        0        0      581 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/recruiters/repository.py
+-rw-r--r--   0        0        0      481 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/companies/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/scheduled_events/__init__.py
+-rw-r--r--   0        0        0     1155 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/scheduled_events/models.py
+-rw-r--r--   0        0        0     1659 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/scheduled_events/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/static/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/static/enumerations.py
+-rw-r--r--   0        0        0     1327 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/static/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/contact_info/__init__.py
+-rw-r--r--   0        0        0      417 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/contact_info/models.py
+-rw-r--r--   0        0        0      718 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/contact_info/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/cover_letters/__init__.py
+-rw-r--r--   0        0        0      277 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/cover_letters/models.py
+-rw-r--r--   0        0        0      681 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/cover_letters/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/demographics/__init__.py
+-rw-r--r--   0        0        0      916 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/demographics/models.py
+-rw-r--r--   0        0        0      682 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/demographics/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/job_preferences/__init__.py
+-rw-r--r--   0        0        0     1617 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/job_preferences/models.py
+-rw-r--r--   0        0        0      712 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/job_preferences/repository.py
+-rw-r--r--   0        0        0       89 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/models.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/qualifications/__init__.py
+-rw-r--r--   0        0        0     2592 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/qualifications/models.py
+-rw-r--r--   0        0        0      681 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/qualifications/repository.py
+-rw-r--r--   0        0        0      632 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/resumes/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/resumes/models.py
+-rw-r--r--   0        0        0      637 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/resumes/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/sessions/__init__.py
+-rw-r--r--   0        0        0      376 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/contexts/users/sessions/models.py
+-rw-r--r--   0        0        0     2463 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/exceptions.py
+-rw-r--r--   0        0        0      375 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/utils.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/aiocron.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/algolia/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/algolia/client_factory.py
+-rw-r--r--   0        0        0      835 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/algolia/mock.py
+-rw-r--r--   0        0        0      702 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/algolia/models.py
+-rw-r--r--   0        0        0     1189 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/algolia/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/__init__.py
+-rw-r--r--   0        0        0     2188 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/client.py
+-rw-r--r--   0        0        0      340 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/client_factory.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/companies/__init__.py
+-rw-r--r--   0        0        0      894 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/companies/models.py
+-rw-r--r--   0        0        0     1972 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/companies/repository.py
+-rw-r--r--   0        0        0     2553 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/mock.py
+-rw-r--r--   0        0        0      413 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/models.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiter_invitation/__init__.py
+-rw-r--r--   0        0        0      747 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiter_invitation/models.py
+-rw-r--r--   0        0        0     2040 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiter_invitation/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiters/__init__.py
+-rw-r--r--   0        0        0     1588 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiters/models.py
+-rw-r--r--   0        0        0     2368 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/recruiters/repository.py
+-rw-r--r--   0        0        0     2318 2023-07-15 17:20:29.141148 getajob-0.3.0/getajob/vendor/clerk/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/clerk/users/__init__.py
+-rw-r--r--   0        0        0     1320 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/clerk/users/models.py
+-rw-r--r--   0        0        0     1963 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/clerk/users/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/__init__.py
+-rw-r--r--   0        0        0      582 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/client_factory.py
+-rw-r--r--   0        0        0     1102 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/helpers.py
+-rw-r--r--   0        0        0      507 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/mock.py
+-rw-r--r--   0        0        0     1975 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/models.py
+-rw-r--r--   0        0        0     9116 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/firestore/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/__init__.py
+-rw-r--r--   0        0        0      725 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/authentication.py
+-rw-r--r--   0        0        0     1369 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/client_factory.py
+-rw-r--r--   0        0        0      320 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/exceptions.py
+-rw-r--r--   0        0        0      617 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/mock.py
+-rw-r--r--   0        0        0     1480 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/models.py
+-rw-r--r--   0        0        0     1517 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/kafka/repository.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/openai/__init__.py
+-rw-r--r--   0        0        0      443 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/openai/client_factory.py
+-rw-r--r--   0        0        0      690 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/openai/mock.py
+-rw-r--r--   0        0        0      985 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/openai/repository.py
+-rw-r--r--   0        0        0      579 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/openai/settings.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sendgrid/__init__.py
+-rw-r--r--   0        0        0      420 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sendgrid/client_factory.py
+-rw-r--r--   0        0        0      227 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sendgrid/mock.py
+-rw-r--r--   0        0        0      678 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sendgrid/repository.py
+-rw-r--r--   0        0        0       45 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sendgrid/templates/example.html
+-rw-r--r--   0        0        0      251 2023-07-15 17:20:29.145148 getajob-0.3.0/getajob/vendor/sentry.py
+-rw-r--r--   0        0        0     1742 2023-07-15 17:20:29.145148 getajob-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2805 1970-01-01 00:00:00.000000 getajob-0.3.0/PKG-INFO
```

### Comparing `getajob-0.2.7/LICENSE` & `getajob-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/config/settings.py` & `getajob-0.3.0/getajob/config/settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     CLERK_JWT_PEM_KEY: str = os.getenv("CLERK_JWT_PEM_KEY", "").replace(r"\n", "\n")
     CLERK_TOKEN_LEEWAY: int = 300
     CLERK_USER_WEBHOOK_SECRET: str = ""
     CLERK_SECRET_KEY: str = ""
 
     DEFAULT_PAGE_LIMIT: int = 20
 
-    LOCAL_TESTING: bool = get_bool_from_string(os.getenv("LOCAL_TESTING", "false"))
+    LOCAL_TESTING: bool = get_bool_from_string(os.getenv("LOCAL_TESTING", "true"))
     ENABLED_KAFKA_EVENTS: bool = get_bool_from_string(
         os.getenv("ENABLED_KAFKA_EVENTS", "false")
     )
 
     # Algolia config
     ALGOLA_APP_ID: str = ""
     ALGOLIA_API_KEY: str = ""
```

### Comparing `getajob-0.2.7/getajob/contexts/admin/users/models.py` & `getajob-0.3.0/getajob/contexts/admin/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/contexts/admin/users/repository.py` & `getajob-0.3.0/getajob/contexts/users/resumes/repository.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,23 @@
-from getajob.vendor.firebase import FirestoreDB
-from getajob.abstractions.repository import BaseRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.abstractions.repository import (
+    MultipleChildrenRepository,
+    RepositoryDependencies,
+)
 from getajob.abstractions.models import Entity, EntityModels
 
-from .models import AdminUser, CreateAdminUser, UpdateAdminUser
+from .models import Resume, CreateResume
 
 
 entity_models = EntityModels(
-    entity=AdminUser, create=CreateAdminUser, update=UpdateAdminUser
+    entity=Resume,
+    create=CreateResume,
+    update=CreateResume,
 )
 
 
-class AdminUserRepository(BaseRepository):
+class ResumeRepository(MultipleChildrenRepository):
     def __init__(self, db: FirestoreDB):
-        super().__init__(db, Entity.ADMIN_USERS.value, entity_models)
-
-    def get_by_user_id(self, user_id: str):
-        return self.get_one_by_attribute("user_id", user_id)
+        super().__init__(
+            RepositoryDependencies(db, Entity.RESUMES.value, entity_models),
+            required_parent_keys=[Entity.USERS.value],
+        )
```

### Comparing `getajob-0.2.7/getajob/contexts/jobs/repository.py` & `getajob-0.3.0/getajob/contexts/companies/jobs/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import typing as t
-from getajob.vendor.firebase import FirestoreDB
-from getajob.vendor.kafka.repository import KafkaRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.vendor.kafka.repository import KafkaProducerRepository
 from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
-from getajob.abstractions.repository import BaseRepository
+from getajob.abstractions.repository import (
+    MultipleChildrenRepository,
+    RepositoryDependencies,
+)
 from getajob.abstractions.models import Entity, EntityModels
-from getajob.contexts.companies.repository import CompanyRepository
 
 from .models import CreateJob, UpdateJob, Job
 from .unit_of_work import JobsUnitOfWork
 
 
 entity_models = EntityModels(entity=Job, create=CreateJob, update=UpdateJob)
 
 
-class JobsRepository(BaseRepository):
-    def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
+class JobsRepository(MultipleChildrenRepository):
+    def __init__(
+        self, db: FirestoreDB, kafka: t.Optional[KafkaProducerRepository] = None
+    ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.jobs, create=True, update=True, delete=True, get=True
         )
         super().__init__(
-            db, Entity.JOBS.value, entity_models, kafka, kafka_event_config
+            RepositoryDependencies(
+                db, Entity.JOBS.value, entity_models, kafka, kafka_event_config
+            ),
+            required_parent_keys=[Entity.COMPANIES.value],
         )
-        self.kafka = kafka
 
-    def create_job(self, job: CreateJob):
-        return JobsUnitOfWork(self).create_job(
-            company_repo=CompanyRepository(db=self.db), data=job
-        )
+    def create_job(self, company_id: str, job: CreateJob):
+        return JobsUnitOfWork(self).create_job(company_id, job)
```

### Comparing `getajob-0.2.7/getajob/contexts/scheduled_events/models.py` & `getajob-0.3.0/getajob/contexts/scheduled_events/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/contexts/scheduled_events/repository.py` & `getajob-0.3.0/getajob/contexts/scheduled_events/repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from datetime import datetime
-from getajob.vendor.firebase import FirestoreDB, FirestoreFilters, FirestorePagination
-from getajob.abstractions.repository import BaseRepository
+from getajob.vendor.firestore.repository import (
+    FirestoreDB,
+    FirestoreFilters,
+    FirestorePagination,
+)
+from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import EntityModels, Entity
 
 from .models import (
     CreateScheduledEvent,
     UpdateScheduledEvent,
     ScheduledEvent,
 )
@@ -12,17 +16,19 @@
 entity_models = EntityModels(
     entity=ScheduledEvent,
     create=CreateScheduledEvent,
     update=UpdateScheduledEvent,
 )
 
 
-class ScheduledEventsRepository(BaseRepository):
+class ScheduledEventsRepository(ParentRepository):
     def __init__(self, db: FirestoreDB):
-        super().__init__(db, Entity.SCHEDULED_EVENTS.value, entity_models)
+        super().__init__(
+            RepositoryDependencies(db, Entity.SCHEDULED_EVENTS.value, entity_models)
+        )
 
     def create_scheduled_event(self, data: CreateScheduledEvent):
         data.next_run_time = data.calculate_next_invocation()
         return super().create(data)
 
     def get_current_scheduled_events(self, page: dict | None = None):
         if not page:
```

### Comparing `getajob-0.2.7/getajob/contexts/static/repository.py` & `getajob-0.3.0/getajob/contexts/static/repository.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/contexts/users/cover_letters/repository.py` & `getajob-0.3.0/getajob/contexts/companies/invitations/repository.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from getajob.vendor.firebase import FirestoreDB
-from getajob.abstractions.repository import BaseRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.abstractions.repository import (
+    MultipleChildrenRepository,
+    RepositoryDependencies,
+)
 from getajob.abstractions.models import Entity, EntityModels
 
-from .models import CoverLetter, CreateCoverLetter, UpdateCoverLetter
+from .models import RecruiterInvitation
 
-entity_models = EntityModels(
-    entity=CoverLetter,
-    create=CreateCoverLetter,
-    update=UpdateCoverLetter,
-)
+entity_models = EntityModels(entity=RecruiterInvitation)
 
 
-class CoverLetterRepository(BaseRepository):
+class RecruiterInvitationsRepository(MultipleChildrenRepository):
     def __init__(self, db: FirestoreDB):
-        super().__init__(db, Entity.COVER_LETTERS.value, entity_models)
+        super().__init__(
+            RepositoryDependencies(
+                db, Entity.RECRUITER_INVITATIONS.value, entity_models
+            ),
+            required_parent_keys=[Entity.COMPANIES.value],
+        )
```

### Comparing `getajob-0.2.7/getajob/contexts/users/repository.py` & `getajob-0.3.0/getajob/contexts/users/demographics/repository.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from getajob.vendor.firebase import FirestoreDB
-from getajob.abstractions.repository import BaseRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.abstractions.repository import (
+    SingleChildRepository,
+    RepositoryDependencies,
+)
 from getajob.abstractions.models import Entity, EntityModels
-from .models import User
 
+from .models import UserDemographicData, DemographicData
 
-entity_models = EntityModels(entity=User)
 
-
-class UserRepository(BaseRepository):
-    def __init__(
-        self,
-        db: FirestoreDB,
-    ):
-        super().__init__(db, Entity.USERS.value, entity_models)
-
-    def get_user(self, id: str):
-        return super().get(id)
-
-    def get_by_email(self, email: str):
-        return self.get_one_by_attribute("email", email)
+entity_models = EntityModels(
+    entity=UserDemographicData,
+    create=DemographicData,
+    update=DemographicData,
+)
+
+
+class UserDemographicsRepository(SingleChildRepository):
+    def __init__(self, db: FirestoreDB):
+        super().__init__(
+            RepositoryDependencies(db, Entity.USER_DEMOGRAPHICS.value, entity_models),
+            required_parent_keys=[Entity.USERS.value],
+        )
```

### Comparing `getajob-0.2.7/getajob/exceptions.py` & `getajob-0.3.0/getajob/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -57,7 +57,12 @@
             detail=detail_string,
         )
 
 
 class KafkaEventTopicNotProvidedError(Exception):
     def __init__(self):
         super().__init__("Kafka event topic must be provided")
+
+
+class MissingParentKeyError(Exception):
+    def __init__(self, parent_key: str):
+        super().__init__(f"Missing parent key: {parent_key}")
```

### Comparing `getajob-0.2.7/getajob/vendor/algolia/models.py` & `getajob-0.3.0/getajob/vendor/algolia/models.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import Enum
-from pydantic import BaseModel
 from typing import Optional, List
+from pydantic import BaseModel
 
 
 class AlgoliaIndex(str, Enum):
     job_search = "job_search"
     company_search = "company_search"
     candidate_search = "candidate_search"
```

### Comparing `getajob-0.2.7/getajob/vendor/algolia/repository.py` & `getajob-0.3.0/getajob/vendor/algolia/repository.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from algoliasearch.search_client import SearchClient
 
+from .client_factory import AlgoliaClientFactory
 from .models import AlgoliaIndex, AlgoliaSearchParams, AlgoliaSearchResults
 
 
-def get_client(app_id: str, api_key: str):
-    return SearchClient.create(app_id, api_key)
+class AlgoliaSearchRepository:
+    def __init__(self, client: SearchClient = AlgoliaClientFactory().get_client()):  # type: ignore
+        self.client = client
 
-
-class AlgoliaSearch:
-    def __init__(self, client: SearchClient, index_name: AlgoliaIndex):
-        self.index = client.init_index(index_name.value)
-
-    def search(self, query: AlgoliaSearchParams):
+    def search(self, index_name: AlgoliaIndex, query: AlgoliaSearchParams):
         search_params = {
             "query": query.query,
             "page": query.page,
             "hitsPerPage": query.hits_per_page,
         }
         if query.filters:
             search_params["filters"] = query.filters
         if query.facet_filters:
             search_params["facetFilters"] = query.facet_filters
         if query.attributes_to_retrieve:
             search_params["attributesToRetrieve"] = query.attributes_to_retrieve
-        res = self.index.search(query, search_params)
+        index = self.client.init_index(index_name.value)
+        res = index.search(query.query, search_params)
         return AlgoliaSearchResults(**res)
 
-    def get_object(self, object_id):
-        return self.index.get_object(object_id)
+    def get_object(self, index_name: AlgoliaIndex, object_id: str):
+        index = self.client.init_index(index_name.value)
+        return index.get_object(object_id)
```

### Comparing `getajob-0.2.7/getajob/vendor/clerk/companies/models.py` & `getajob-0.3.0/getajob/vendor/clerk/companies/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/vendor/clerk/companies/repository.py` & `getajob-0.3.0/getajob/vendor/clerk/companies/repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import typing as t
 
-from getajob.vendor.firebase import FirestoreDB
-from getajob.vendor.kafka.repository import KafkaRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.vendor.kafka.repository import KafkaProducerRepository
 from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
-from getajob.abstractions.repository import BaseRepository
+from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import Entity, EntityModels
 
 from .models import (
     ClerkCompanyWebhookEvent,
     ClerkCompany,
     ClerkCompanyDeleted,
     ClerkCompanyWebhookType,
 )
 
 entity_models = EntityModels(entity=ClerkCompany)
 
 
-class WebhookCompanyRepository(BaseRepository):
-    def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
+class WebhookCompanyRepository(ParentRepository):
+    def __init__(
+        self, db: FirestoreDB, kafka: t.Optional[KafkaProducerRepository] = None
+    ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.companies,
             create=True,
             update=True,
             delete=True,
         )
         super().__init__(
-            db, Entity.COMPANIES.value, entity_models, kafka, kafka_event_config
+            RepositoryDependencies(
+                db, Entity.COMPANIES.value, entity_models, kafka, kafka_event_config
+            )
         )
 
     def handle_webhook_event(self, event: ClerkCompanyWebhookEvent):
         event_dict = {
             ClerkCompanyWebhookType.organization_created: self.create_company,
             ClerkCompanyWebhookType.organization_updated: self.update_company,
             ClerkCompanyWebhookType.organization_deleted: self.delete_company,
```

### Comparing `getajob-0.2.7/getajob/vendor/clerk/recruiter_invitation/models.py` & `getajob-0.3.0/getajob/vendor/clerk/recruiter_invitation/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/vendor/clerk/recruiters/models.py` & `getajob-0.3.0/getajob/vendor/clerk/recruiters/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,32 +16,26 @@
 
 
 class ClerkCompanyMembershipWebhookEvent(ClerkWebhookEvent):
     type: ClerkCompanyMembershipWebhookType
 
 
 class CreateClerkCompanyMember(BaseModel):
-    first_name: str
-    identifier: str
     image_url: str | None = None
-    last_name: str
     profile_image_url: str | None = None
     user_id: str
 
 
 class ClerkCompanyMember(CreateClerkCompanyMember):
     id: str
     role: ClerkCompanyMemberType
 
 
 class UpdateClerkCompanyMember(BaseModel):
-    first_name: str | None = None
-    identifier: str | None = None
     image_url: str | None = None
-    last_name: str | None = None
     profile_image_url: str | None = None
     user_id: str | None = None
 
 
 class UpdateClerkCompanyMemberWithRole(UpdateClerkCompanyMember):
     role: ClerkCompanyMemberType | None = None
```

### Comparing `getajob-0.2.7/getajob/vendor/clerk/recruiters/repository.py` & `getajob-0.3.0/getajob/vendor/clerk/recruiters/repository.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,27 @@
-import typing as t
-
-from getajob.vendor.firebase import FirestoreDB
-from getajob.vendor.kafka.repository import KafkaRepository
-from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
-from getajob.abstractions.repository import BaseRepository
+from getajob.vendor.firestore.repository import FirestoreDB
 from getajob.abstractions.models import Entity, EntityModels
+from getajob.contexts.companies.recruiters.repository import RecruiterRepository
 
 
 from .models import (
     ClerkCompanyMembershipWebhookEvent,
     ClerkCompanyMembership,
     ClerkCompanyMembershipWebhookType,
     ClerkUpdateCompanyMembership,
     ClerkCompanyMember,
     UpdateClerkCompanyMemberWithRole,
 )
 
 entity_models = EntityModels(entity=ClerkCompanyMember)
 
 
-class WebhookCompanyMembershipRepository(BaseRepository):
-    def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
-        kafka_event_config = KafkaEventConfig(
-            topic=KafkaTopic.recruiters,
-            create=True,
-            update=True,
-            delete=True,
-        )
-        super().__init__(
-            db, Entity.RECRUITERS.value, entity_models, kafka, kafka_event_config
-        )
+class WebhookCompanyMembershipRepository:
+    def __init__(self, db: FirestoreDB):
+        self.repo = RecruiterRepository(db)
 
     def handle_webhook_event(self, event: ClerkCompanyMembershipWebhookEvent):
         event_dict = {
             ClerkCompanyMembershipWebhookType.organization_membership_created: self.create_recruiter,
             ClerkCompanyMembershipWebhookType.organization_membership_updated: self.update_recruiter,
             ClerkCompanyMembershipWebhookType.organization_membership_deleted: self.delete_recruiter,
         }
@@ -42,30 +30,30 @@
     def create_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         create_event = ClerkCompanyMembership(**event.data)
         recruiter = ClerkCompanyMember(
             **create_event.public_user_data.dict(),
             id=create_event.id,
             role=create_event.role
         )
-        return self.create(
+        return self.repo.create(
             data=recruiter,
             provided_id=create_event.id,
             parent_collections={Entity.COMPANIES.value: create_event.organization.id},
         )
 
     def delete_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         delete_event = ClerkUpdateCompanyMembership(**event.data)
-        return self.delete(
+        return self.repo.delete(
             doc_id=delete_event.id,
             parent_collections={Entity.COMPANIES.value: delete_event.organization.id},
         )
 
     def update_recruiter(self, event: ClerkCompanyMembershipWebhookEvent):
         update_event = ClerkUpdateCompanyMembership(**event.data)
         recruiter = UpdateClerkCompanyMemberWithRole(
             **update_event.public_user_data.dict(), role=update_event.role
         )
-        return self.update(
+        return self.repo.update(
             doc_id=update_event.id,
             data=recruiter,
             parent_collections={Entity.COMPANIES.value: update_event.organization.id},
         )
```

### Comparing `getajob-0.2.7/getajob/vendor/clerk/repository.py` & `getajob-0.3.0/getajob/vendor/clerk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,61 @@
-import requests
-from requests import Response
-from pydantic import BaseModel
-
-from .exceptions import UserNotFoundException, CompanyNotFoundException
-from .companies.models import ClerkCompany
-from .users.models import ClerkUser
-from .recruiter_invitation.models import ClerkCompanyInvitation
-from .recruiters.models import ClerkCompanyMembership
+from fastapi import HTTPException
+from requests import request, Response
 
+from getajob.config.settings import SETTINGS
+from getajob.exceptions import EntityNotFound
 
-class ClerkAPI:
-    def __init__(self, api_key):
-        self.api_key = api_key
+
+class ClerkClient:
+    def __init__(self):
+        self.api_key = SETTINGS.CLERK_SECRET_KEY
         self.base_url = "https://api.clerk.dev"
 
-    def _get_headers(self):
+    def _headers(self):
         return {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
         }
 
     def _make_request(
         self, method: str, endpoint: str, payload: dict | None = None
     ) -> Response:
         url = self.base_url + endpoint
-        request = {"method": method, "url": url, "headers": self._get_headers()}
+        request_payload = {"method": method, "url": url, "headers": self._headers()}
         if payload:
-            request["json"] = payload
-        response = requests.request(**request, timeout=10)
+            request_payload["json"] = payload
+        response = request(**request_payload, timeout=10)
+        if response.status_code == 404:
+            raise EntityNotFound(endpoint)
+        if response.status_code != 200:
+            raise HTTPException(
+                status_code=500, detail=f"Error: {response.status_code} {response.text}"
+            )
         return response
 
-    def _format_response_to_model(self, response: Response, model: BaseModel):
-        response_json = response.json()
-        if "data" in response_json:
-            response_json = response_json["data"]
-        if isinstance(response_json, list):
-            return [model(**item) for item in response_json]  # type: ignore
-        return model(**response_json)  # type: ignore
-
     def get_user(self, user_id: str):
         endpoint = f"/v1/users/{user_id}"
-        res = self._make_request("GET", endpoint)
-        if res.status_code == 404:
-            raise UserNotFoundException()
-        return self._format_response_to_model(res, ClerkUser)  # type: ignore
+        return self._make_request("GET", endpoint).json()
 
     def get_company(self, company_id: str):
         endpoint = f"/v1/organizations/{company_id}"
-        res = self._make_request("GET", endpoint)
-        if res.status_code == 404:
-            raise CompanyNotFoundException()
-        return self._format_response_to_model(res, ClerkCompany)  # type: ignore
+        return self._make_request("GET", endpoint).json()
 
     def get_company_invitations(self, company_id: str):
         endpoint = f"/v1/organizations/{company_id}/invitations/pending"
-        res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkCompanyInvitation)  # type: ignore
+        return self._make_request("GET", endpoint).json()
 
     def get_company_recruiters(self, company_id):
         endpoint = f"/v1/organizations/{company_id}/memberships"
-        res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkCompanyMembership)
+        return self._make_request("GET", endpoint).json()
 
     def get_companies_by_user_id(self, user_id):
         endpoint = f"/v1/users/{user_id}/organization_memberships"
-        res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkCompanyMembership)
+        return self._make_request("GET", endpoint).json()
 
     def get_all_users(self):
         endpoint = "/v1/users"
-        res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkUser)
+        return self._make_request("GET", endpoint).json()
 
     def get_all_companies(self):
         endpoint = "/v1/organizations"
-        res = self._make_request("GET", endpoint)
-        return self._format_response_to_model(res, ClerkCompany)
+        return self._make_request("GET", endpoint).json()
```

### Comparing `getajob-0.2.7/getajob/vendor/clerk/users/models.py` & `getajob-0.3.0/getajob/vendor/clerk/users/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/getajob/vendor/clerk/users/repository.py` & `getajob-0.3.0/getajob/vendor/clerk/users/repository.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import typing as t
 
-from getajob.vendor.firebase import FirestoreDB
-from getajob.vendor.kafka.repository import KafkaRepository
+from getajob.vendor.firestore.repository import FirestoreDB
+from getajob.vendor.kafka.repository import KafkaProducerRepository
 from getajob.vendor.kafka.models import KafkaEventConfig, KafkaTopic
-from getajob.abstractions.repository import BaseRepository
+from getajob.abstractions.repository import ParentRepository, RepositoryDependencies
 from getajob.abstractions.models import Entity, EntityModels
 
 from .models import (
     ClerkUser,
     ClerkUserWebhookEvent,
     ClerkUserWebhookType,
     ClerkWebhookUserDeleted,
     ClerkWebhookUserUpdated,
 )
 
 entity_models = EntityModels(entity=ClerkUser, update=ClerkWebhookUserUpdated)
 
 
-class WebhookUserRepository(BaseRepository):
-    def __init__(self, db: FirestoreDB, kafka: t.Optional[KafkaRepository] = None):
+class WebhookUserRepository(ParentRepository):
+    def __init__(
+        self, db: FirestoreDB, kafka: t.Optional[KafkaProducerRepository] = None
+    ):
         kafka_event_config = KafkaEventConfig(
             topic=KafkaTopic.users,
             create=True,
             update=True,
             delete=True,
         )
         super().__init__(
-            db, Entity.USERS.value, entity_models, kafka, kafka_event_config
+            RepositoryDependencies(
+                db, Entity.USERS.value, entity_models, kafka, kafka_event_config
+            )
         )
 
     def handle_webhook_event(self, event: ClerkUserWebhookEvent):
         event_dict = {
             ClerkUserWebhookType.user_created: self.create_user,
             ClerkUserWebhookType.user_updated: self.update_user,
             ClerkUserWebhookType.user_deleted: self.delete_user,
```

### Comparing `getajob-0.2.7/getajob/vendor/firebase.py` & `getajob-0.3.0/getajob/vendor/firestore/repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,136 +1,53 @@
-from enum import Enum
 import typing as t
-import json
 
-from pydantic import BaseModel
-import firebase_admin
-from firebase_admin import credentials, firestore
 from google.cloud.firestore_v1.client import Client
 from google.cloud.firestore_v1.base_query import BaseQuery
 
-from getajob.config.settings import SETTINGS
 from getajob.exceptions import EntityNotFound, MultipleEntitiesReturned
 
-
-class FirestorePagination(BaseModel):
-    start_after: t.Optional[dict] = None
-    limit: int = SETTINGS.DEFAULT_PAGE_LIMIT
-
-    class Config:
-        arbitrary_types_allowed = True
-
-
-class FirestoreFilters(BaseModel):
-    field: str
-    operator: t.Literal[
-        "==",
-        ">",
-        "<",
-        ">=",
-        "<=",
-        "array-contains",
-        "in",
-        "array-contains-any",
-        "not-in",
-        "like",  # The like operator is custom soft text
-    ]
-    value: t.Any
-
-
-class FirestoreOrderBy(BaseModel):
-    field: str
-    direction: t.Literal["ASCENDING", "DESCENDING"]
-
-
-class FirestoreDocument(BaseModel):
-    id: str
-    data: t.Dict[str, t.Any]
-
-
-class FirestorePaginatedResponse(BaseModel):
-    results: t.List[FirestoreDocument]
-    start_after: t.Optional[dict] = None
-    count: int = 0
-
-    class Config:
-        arbitrary_types_allowed = True
-
-
-class FirestoreBatchActionType(str, Enum):
-    CREATE = "create"
-    UPDATE = "update"
-    DELETE = "delete"
-
-
-class FirestoreBatchAction(BaseModel):
-    action: FirestoreBatchActionType
-    parent_collections: dict
-    collection_name: str
-    document_data: dict
-    document_id: str
-
-
-class ParentAndCollection(BaseModel):
-    parents: dict
-    collection: str
-    id: str
-
-
-def list_of_parent_collections(input_dict: dict) -> t.List[ParentAndCollection]:
-    output_list = []
-    parent_dict: t.Dict[str, str] = {}
-    for key in input_dict:
-        parent_dict_copy = parent_dict.copy()
-        output_list.append(
-            ParentAndCollection(
-                parents=parent_dict_copy, collection=key, id=input_dict[key]
-            )
-        )
-        parent_dict[key] = input_dict[key]
-    return output_list
-
-
-def get_client():
-    cred = credentials.Certificate(json.loads(SETTINGS.FIRESTORE_JSON_CONFIG))
-    firebase_admin.initialize_app(cred)
-    return firestore.client()
-
-
-def add_filters_to_query(query_reference: BaseQuery, filters: t.List[FirestoreFilters]):
-    for _filter in filters:
-        if _filter.operator == "like":
-            query_reference = query_reference.where(
-                _filter.field, ">=", _filter.value
-            ).where(_filter.field, "<=", _filter.value + "\uf8ff")
-        else:
-            query_reference = query_reference.where(
-                _filter.field, _filter.operator, _filter.value
-            )
-    return query_reference
+from .mock import MockFirestoreClient
+from .client_factory import FirestoreClientFactory
+from .helpers import get_list_of_parent_collections_from_dict, add_filters_to_query
+from .models import (
+    FirestoreDocument,
+    FirestoreFilters,
+    FirestoreOrderBy,
+    FirestorePagination,
+    FirestorePaginatedResponse,
+    FirestoreBatchAction,
+    FirestoreBatchActionType,
+    GetWithJoins,
+    QueryWithJoins,
+)
 
 
 class FirestoreDB:
-    def __init__(self, client: Client):
+    def __init__(self, client: Client = FirestoreClientFactory.get_client()):  # type: ignore
         self._client = client
 
     def disconnect(self):
-        if isinstance(self._client, Client):
-            self._client.close()
+        self._client.close()
+
+    def _reset_mock(self):
+        if isinstance(self._client, MockFirestoreClient):
+            self._client.reset()
 
     def _get_collection_ref(self, parent_collections: dict, collection_name: str):
         collection_ref = self._client
         for parent, parent_id in parent_collections.items():
             collection_ref = collection_ref.collection(parent).document(parent_id)  # type: ignore
         return collection_ref.collection(collection_name)
 
     def _verify_parent_exists(self, parent_collections: dict):
         if not parent_collections:
             return
-        all_parent_collections = list_of_parent_collections(parent_collections)
+        all_parent_collections = get_list_of_parent_collections_from_dict(
+            parent_collections
+        )
         for parent_collection in all_parent_collections:
             # This will raise an exception if the parent doesn't exist
             self.get(
                 parent_collection.parents,
                 parent_collection.collection,
                 parent_collection.id,
             )
@@ -241,41 +158,77 @@
 
     def get_one_by_attribute(
         self,
         parent_collections: dict,
         collection_name: str,
         attribute: str,
         value: str,
-    ) -> t.Union[FirestoreDocument, None]:
+    ) -> FirestoreDocument:
         res = self.query(
             parent_collections=parent_collections,
             collection_name=collection_name,
             filters=[FirestoreFilters(field=attribute, operator="==", value=value)],
         )
         if len(res.results) == 1:
             return res.results[0]
         if len(res.results) > 1:
             raise MultipleEntitiesReturned(collection_name, value)
-        return None
+        raise EntityNotFound(collection_name, value)
 
     def batch_action(self, writes: t.List[FirestoreBatchAction]) -> list:
         batch = self._client.batch()
         for write in writes:
-            if write.action == "create":
+            if write.action == FirestoreBatchActionType.CREATE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
                 batch.set(doc_ref, write.document_data)
-            elif write.action == "update":
+            elif write.action == FirestoreBatchActionType.UPDATE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
                 batch.update(doc_ref, write.document_data)
-            elif write.action == "delete":
+            elif write.action == FirestoreBatchActionType.DELETE:
                 collection_ref = self._get_collection_ref(
                     write.parent_collections, write.collection_name
                 )
                 doc_ref = collection_ref.document(write.document_id)
                 batch.delete(doc_ref)
         return batch.commit()
+
+    def get_with_joins(self, join_model: GetWithJoins) -> FirestoreDocument:
+        """
+        This is limited to single depth
+        """
+        res = self.get(
+            join_model.parent_collections, join_model.get_collection, join_model.get_id
+        )
+        for join in join_model.joins:
+            if join.attribute in res.data and res.data[join.attribute]:
+                joined_value = self.get(
+                    join.parent_collections, join.collection, res.data[join.attribute]
+                )
+                res.data[join.attribute] = joined_value.data
+        return res
+
+    def query_with_joins(
+        self, join_query: QueryWithJoins
+    ) -> FirestorePaginatedResponse:
+        results_page = self.query(
+            join_query.parent_collections,
+            join_query.collection_name,
+            join_query.filters,
+            join_query.order_by,
+            join_query.pagination,
+        )
+        for idx, res in enumerate(results_page.results):
+            for join in join_query.joins:
+                if join.attribute in res.data and res.data[join.attribute]:
+                    joined_value = self.get(
+                        join.parent_collections,
+                        join.collection,
+                        res.data[join.attribute],
+                    )
+                    results_page.results[idx].data[join.attribute] = joined_value.data
+        return results_page
```

### Comparing `getajob-0.2.7/getajob/vendor/kafka/authentication.py` & `getajob-0.3.0/getajob/vendor/kafka/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime, timedelta
 import jwt
+
 from .exceptions import ExpiredTokenException, InvalidTokenException
 
 
 def generate_kafka_jwt(
     kafka_username: str,
     kafka_jwt_secret: str,
     expire_datetime: datetime = (datetime.utcnow() + timedelta(seconds=60)),
```

### Comparing `getajob-0.2.7/getajob/vendor/kafka/kafka.py` & `getajob-0.3.0/getajob/vendor/kafka/client_factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from kafka import KafkaProducer, KafkaConsumer
 
+from getajob.abstractions.vendor_client_factory import VendorClientFactory
 from getajob.config.settings import SETTINGS
+
+from .mock import MockKafkaProducer, MockKafkaConsumer
 from .models import KafkaTopic
-from .authentication import generate_kafka_jwt
 
 
-def get_producer():
-    return KafkaProducer(
-        bootstrap_servers=[SETTINGS.KAFKA_BOOTSTRAP_SERVER],
-        sasl_mechanism="SCRAM-SHA-256",
-        security_protocol="SASL_SSL",
-        sasl_plain_username=SETTINGS.KAFKA_USERNAME,
-        sasl_plain_password=SETTINGS.KAFKA_PASSWORD,
-    )
-
-
-def get_consumer():
-    consumer = KafkaConsumer(
-        bootstrap_servers=[SETTINGS.KAFKA_BOOTSTRAP_SERVER],
-        sasl_mechanism="SCRAM-SHA-256",
-        security_protocol="SASL_SSL",
-        sasl_plain_username=SETTINGS.KAFKA_USERNAME,
-        sasl_plain_password=SETTINGS.KAFKA_PASSWORD,
-        auto_offset_reset="earliest",
-        group_id="default",
-    )
-    consumer.subscribe(KafkaTopic.get_all_topics())
-    return consumer
-
-
-def produce_message(producer: KafkaProducer, topic: KafkaTopic, message_json: str):
-    message_token = generate_kafka_jwt(
-        SETTINGS.KAFKA_USERNAME, SETTINGS.KAFKA_JWT_SECRET
-    )
-    producer.send(
-        topic.value,
-        message_json.encode("utf-8"),
-        headers=[("authorization", message_token.encode("utf-8"))],
-    )
+class KafkaProducerFactory(VendorClientFactory):
+    @staticmethod
+    def _return_mock():
+        return MockKafkaProducer()
+
+    @staticmethod
+    def _return_client():
+        return KafkaProducer(
+            bootstrap_servers=[SETTINGS.KAFKA_BOOTSTRAP_SERVER],
+            sasl_mechanism="SCRAM-SHA-256",
+            security_protocol="SASL_SSL",
+            sasl_plain_username=SETTINGS.KAFKA_USERNAME,
+            sasl_plain_password=SETTINGS.KAFKA_PASSWORD,
+        )
+
+
+class KafkaConsumerFactory(VendorClientFactory):
+    @staticmethod
+    def _return_mock():
+        return MockKafkaConsumer()
+
+    @staticmethod
+    def _return_client():
+        consumer = KafkaConsumer(
+            bootstrap_servers=[SETTINGS.KAFKA_BOOTSTRAP_SERVER],
+            sasl_mechanism="SCRAM-SHA-256",
+            security_protocol="SASL_SSL",
+            sasl_plain_username=SETTINGS.KAFKA_USERNAME,
+            sasl_plain_password=SETTINGS.KAFKA_PASSWORD,
+            auto_offset_reset="earliest",
+            group_id="default",
+        )
+        consumer.subscribe(KafkaTopic.get_all_topics())
+        return consumer
```

### Comparing `getajob-0.2.7/getajob/vendor/kafka/models.py` & `getajob-0.3.0/getajob/vendor/kafka/models.py`

 * *Files identical despite different names*

### Comparing `getajob-0.2.7/pyproject.toml` & `getajob-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "getajob"
-version = "0.2.7"
+version = "0.3.0"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "3.8.4"
```

### Comparing `getajob-0.2.7/PKG-INFO` & `getajob-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getajob
-Version: 0.2.7
+Version: 0.3.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiocron (>=1.8,<2.0)
```

