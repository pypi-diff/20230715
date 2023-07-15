# Comparing `tmp/bovine-0.2.6.tar.gz` & `tmp/bovine-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine-0.2.6.tar", max compression
+gzip compressed data, was "bovine-0.3.0.tar", max compression
```

## Comparing `bovine-0.2.6.tar` & `bovine-0.3.0.tar`

### file list

```diff
@@ -1,106 +1,60 @@
--rw-r--r--   0        0        0     1363 2023-06-04 18:31:36.354114 bovine-0.2.6/README.md
--rw-r--r--   0        0        0     9472 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/__init__.py
--rw-r--r--   0        0        0     4957 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-04 18:32:41.834765 bovine-0.2.6/bovine/activitystreams/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4483 2023-06-04 18:32:41.834765 bovine-0.2.6/bovine/activitystreams/__pycache__/activity_factory.cpython-310.pyc
--rw-r--r--   0        0        0     2145 2023-06-04 18:32:41.842765 bovine-0.2.6/bovine/activitystreams/__pycache__/collection_helper.cpython-310.pyc
--rw-r--r--   0        0        0     4369 2023-06-04 18:32:41.838765 bovine-0.2.6/bovine/activitystreams/__pycache__/object_factory.cpython-310.pyc
--rw-r--r--   0        0        0     4584 2023-06-04 18:32:42.814775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_activity_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3327 2023-06-04 18:32:42.822775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_actor.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      795 2023-06-04 18:32:42.826775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_collection_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3113 2023-06-04 18:32:42.834775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_object_factory.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1951 2023-06-04 18:32:42.838775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_builder.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1386 2023-06-04 18:32:42.842775 bovine-0.2.6/bovine/activitystreams/__pycache__/test_ordered_collection_page.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4386 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/activity_factory.py
--rw-r--r--   0        0        0     2151 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/collection_helper.py
--rw-r--r--   0        0        0     4515 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/object_factory.py
--rw-r--r--   0        0        0     2195 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_activity_factory.py
--rw-r--r--   0        0        0     1442 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_actor.py
--rw-r--r--   0        0        0      471 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_collection_helper.py
--rw-r--r--   0        0        0     1257 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_object_factory.py
--rw-r--r--   0        0        0     1034 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_ordered_collection_builder.py
--rw-r--r--   0        0        0      817 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/test_ordered_collection_page.py
--rw-r--r--   0        0        0     2354 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/__init__.py
--rw-r--r--   0        0        0     2836 2023-06-04 18:32:41.838765 bovine-0.2.6/bovine/activitystreams/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4763 2023-06-04 18:32:42.854776 bovine-0.2.6/bovine/activitystreams/utils/__pycache__/test_utils.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      865 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/print.py
--rw-r--r--   0        0        0     2266 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/activitystreams/utils/test_utils.py
--rw-r--r--   0        0        0     3968 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/__init__.py
--rw-r--r--   0        0        0     4002 2023-06-04 18:32:41.842765 bovine-0.2.6/bovine/clients/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3683 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/authorization_wrapper.cpython-310.pyc
--rw-r--r--   0        0        0     1916 2023-06-04 18:32:42.402771 bovine-0.2.6/bovine/clients/__pycache__/bearer.cpython-310.pyc
--rw-r--r--   0        0        0      268 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/consts.cpython-310.pyc
--rw-r--r--   0        0        0     1719 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/event_source.cpython-310.pyc
--rw-r--r--   0        0        0     1084 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/lookup_account.cpython-310.pyc
--rw-r--r--   0        0        0     2534 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/moo_auth.cpython-310.pyc
--rw-r--r--   0        0        0     1237 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/clients/__pycache__/nodeinfo.cpython-310.pyc
--rw-r--r--   0        0        0     1529 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/signed_http.cpython-310.pyc
--rw-r--r--   0        0        0     2479 2023-06-04 18:32:42.406771 bovine-0.2.6/bovine/clients/__pycache__/signed_http_methods.cpython-310.pyc
--rw-r--r--   0        0        0     1507 2023-06-04 18:32:42.858775 bovine-0.2.6/bovine/clients/__pycache__/test_event_source.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2844 2023-06-04 18:32:42.862776 bovine-0.2.6/bovine/clients/__pycache__/test_lookup_account.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1217 2023-06-04 18:32:42.866776 bovine-0.2.6/bovine/clients/__pycache__/test_nodeinfo.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2102 2023-06-04 18:32:42.870776 bovine-0.2.6/bovine/clients/__pycache__/test_signed_http.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      814 2023-06-04 18:32:42.870776 bovine-0.2.6/bovine/clients/__pycache__/test_signed_http_client.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3451 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/authorization_wrapper.py
--rw-r--r--   0        0        0     1794 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/bearer.py
--rw-r--r--   0        0        0       91 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/consts.py
--rw-r--r--   0        0        0     1520 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/event_source.py
--rw-r--r--   0        0        0      868 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/lookup_account.py
--rw-r--r--   0        0        0     3001 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/moo_auth.py
--rw-r--r--   0        0        0      948 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/nodeinfo.py
--rw-r--r--   0        0        0     1150 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/signed_http.py
--rw-r--r--   0        0        0     3278 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/signed_http_methods.py
--rw-r--r--   0        0        0      651 2023-06-04 18:31:36.354114 bovine-0.2.6/bovine/clients/test_event_source.py
--rw-r--r--   0        0        0     1505 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_lookup_account.py
--rw-r--r--   0        0        0      319 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_nodeinfo.py
--rw-r--r--   0        0        0     1153 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_signed_http.py
--rw-r--r--   0        0        0      522 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/clients/test_signed_http_client.py
--rw-r--r--   0        0        0     4141 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/__init__.py
--rw-r--r--   0        0        0     3749 2023-06-04 18:32:42.154769 bovine-0.2.6/bovine/crypto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2863 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     2909 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/http_signature.cpython-310.pyc
--rw-r--r--   0        0        0     2257 2023-06-04 18:32:42.354771 bovine-0.2.6/bovine/crypto/__pycache__/signature_checker.cpython-310.pyc
--rw-r--r--   0        0        0     1784 2023-06-04 18:32:42.402771 bovine-0.2.6/bovine/crypto/__pycache__/signature_parser.cpython-310.pyc
--rw-r--r--   0        0        0     2363 2023-06-04 18:32:42.430771 bovine-0.2.6/bovine/crypto/__pycache__/test.cpython-310.pyc
--rw-r--r--   0        0        0     5821 2023-06-04 18:32:42.878776 bovine-0.2.6/bovine/crypto/__pycache__/test_crypto.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2742 2023-06-04 18:32:42.886776 bovine-0.2.6/bovine/crypto/__pycache__/test_helper.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7454 2023-06-04 18:32:42.898776 bovine-0.2.6/bovine/crypto/__pycache__/test_http_signature.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2674 2023-06-04 18:32:42.910776 bovine-0.2.6/bovine/crypto/__pycache__/test_signature_parser.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2664 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/helper.py
--rw-r--r--   0        0        0     2112 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/http_signature.py
--rw-r--r--   0        0        0     2942 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/signature_checker.py
--rw-r--r--   0        0        0     1266 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/signature_parser.py
--rw-r--r--   0        0        0     2199 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test.py
--rw-r--r--   0        0        0     4995 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_crypto.py
--rw-r--r--   0        0        0      896 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_helper.py
--rw-r--r--   0        0        0     5081 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_http_signature.py
--rw-r--r--   0        0        0     1207 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/crypto/test_signature_parser.py
--rw-r--r--   0        0        0      302 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/ed25519_key.py
--rw-r--r--   0        0        0     3342 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/jsonld.py
--rw-r--r--   0        0        0      826 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/msg.py
--rw-r--r--   0        0        0     3286 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/repl.py
--rw-r--r--   0        0        0     2757 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_bovine_actor.py
--rw-r--r--   0        0        0      178 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_bovine_client.py
--rw-r--r--   0        0        0     5250 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_jsonld.py
--rw-r--r--   0        0        0      282 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/test_types.py
--rw-r--r--   0        0        0     2397 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/types.py
--rw-r--r--   0        0        0      936 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/__init__.py
--rw-r--r--   0        0        0     1170 2023-06-04 18:32:42.150769 bovine-0.2.6/bovine/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      877 2023-06-04 18:32:42.358770 bovine-0.2.6/bovine/utils/__pycache__/date.cpython-310.pyc
--rw-r--r--   0        0        0     3240 2023-06-04 18:32:42.798775 bovine-0.2.6/bovine/utils/__pycache__/pyld_requests.cpython-310.pyc
--rw-r--r--   0        0        0     3465 2023-06-04 18:32:42.918776 bovine-0.2.6/bovine/utils/__pycache__/test_date.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1662 2023-06-04 18:32:42.922776 bovine-0.2.6/bovine/utils/__pycache__/test_parse.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1627 2023-06-04 18:32:42.926776 bovine-0.2.6/bovine/utils/__pycache__/test_webfinger.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      519 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/date.py
--rw-r--r--   0        0        0     1432 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/__init__.py
--rw-r--r--   0        0        0     1934 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1967 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/test_validation.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      659 2023-06-04 18:32:42.930776 bovine-0.2.6/bovine/utils/msg/__pycache__/validation.cpython-310.pyc
--rw-r--r--   0        0        0      599 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/test_validation.py
--rw-r--r--   0        0        0      261 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/msg/validation.py
--rw-r--r--   0        0        0     4736 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/pyld_requests.py
--rw-r--r--   0        0        0      761 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_date.py
--rw-r--r--   0        0        0      452 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_parse.py
--rw-r--r--   0        0        0      370 2023-06-04 18:31:36.358115 bovine-0.2.6/bovine/utils/test_webfinger.py
--rw-r--r--   0        0        0     1479 2023-06-04 18:31:36.362115 bovine-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 bovine-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-07-15 11:42:04.780655 bovine-0.3.0/README.md
+-rw-r--r--   0        0        0    10008 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/__init__.py
+-rw-r--r--   0        0        0     4957 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/__init__.py
+-rw-r--r--   0        0        0     4406 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/activity_factory.py
+-rw-r--r--   0        0        0     2670 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/collection_helper.py
+-rw-r--r--   0        0        0     4515 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/object_factory.py
+-rw-r--r--   0        0        0     2195 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_activity_factory.py
+-rw-r--r--   0        0        0     1442 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_actor.py
+-rw-r--r--   0        0        0      544 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_collection_helper.py
+-rw-r--r--   0        0        0     1257 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_object_factory.py
+-rw-r--r--   0        0        0     1034 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_ordered_collection_builder.py
+-rw-r--r--   0        0        0      817 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/test_ordered_collection_page.py
+-rw-r--r--   0        0        0     2354 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/utils/__init__.py
+-rw-r--r--   0        0        0      865 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/utils/print.py
+-rw-r--r--   0        0        0     2266 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/activitystreams/utils/test_utils.py
+-rw-r--r--   0        0        0     3968 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/__init__.py
+-rw-r--r--   0        0        0     3451 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/authorization_wrapper.py
+-rw-r--r--   0        0        0     1794 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/bearer.py
+-rw-r--r--   0        0        0       91 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/consts.py
+-rw-r--r--   0        0        0     1520 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/event_source.py
+-rw-r--r--   0        0        0      868 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/lookup_account.py
+-rw-r--r--   0        0        0     3001 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/moo_auth.py
+-rw-r--r--   0        0        0      948 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/nodeinfo.py
+-rw-r--r--   0        0        0     1150 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/signed_http.py
+-rw-r--r--   0        0        0     3278 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/signed_http_methods.py
+-rw-r--r--   0        0        0      651 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/test_event_source.py
+-rw-r--r--   0        0        0     1505 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/test_lookup_account.py
+-rw-r--r--   0        0        0      319 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/test_nodeinfo.py
+-rw-r--r--   0        0        0     1153 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/test_signed_http.py
+-rw-r--r--   0        0        0      522 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/clients/test_signed_http_client.py
+-rw-r--r--   0        0        0     4141 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/__init__.py
+-rw-r--r--   0        0        0     2687 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/helper.py
+-rw-r--r--   0        0        0     2112 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/http_signature.py
+-rw-r--r--   0        0        0     2942 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/signature_checker.py
+-rw-r--r--   0        0        0     1266 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/signature_parser.py
+-rw-r--r--   0        0        0     2199 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/test.py
+-rw-r--r--   0        0        0     4995 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/test_crypto.py
+-rw-r--r--   0        0        0      896 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/test_helper.py
+-rw-r--r--   0        0        0     5081 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/test_http_signature.py
+-rw-r--r--   0        0        0     1207 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/crypto/test_signature_parser.py
+-rw-r--r--   0        0        0      302 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/ed25519_key.py
+-rw-r--r--   0        0        0     3418 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/jsonld.py
+-rw-r--r--   0        0        0      826 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/msg.py
+-rw-r--r--   0        0        0     3286 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/repl.py
+-rw-r--r--   0        0        0     2757 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/test_bovine_actor.py
+-rw-r--r--   0        0        0      178 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/test_bovine_client.py
+-rw-r--r--   0        0        0     5250 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/test_jsonld.py
+-rw-r--r--   0        0        0      282 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/test_types.py
+-rw-r--r--   0        0        0     2397 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/types.py
+-rw-r--r--   0        0        0      936 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/__init__.py
+-rw-r--r--   0        0        0      519 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/date.py
+-rw-r--r--   0        0        0     1432 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/msg/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/msg/test_validation.py
+-rw-r--r--   0        0        0      261 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/msg/validation.py
+-rw-r--r--   0        0        0     4736 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/pyld_requests.py
+-rw-r--r--   0        0        0      761 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/test_date.py
+-rw-r--r--   0        0        0      452 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/test_parse.py
+-rw-r--r--   0        0        0      370 2023-07-15 11:42:04.780655 bovine-0.3.0/bovine/utils/test_webfinger.py
+-rw-r--r--   0        0        0     1479 2023-07-15 11:42:04.784655 bovine-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2608 1970-01-01 00:00:00.000000 bovine-0.3.0/PKG-INFO
```

### Comparing `bovine-0.2.6/README.md` & `bovine-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/__init__.py` & `bovine-0.3.0/bovine/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 from typing import Optional
-from urllib.parse import urlparse
+from urllib.parse import urlencode, urlparse
 
 import tomli
 
 from .activitystreams import Collection
 from .activitystreams.activity_factory import ActivityFactory
 from .activitystreams.collection_helper import CollectionHelper
 from .activitystreams.object_factory import ObjectFactory
@@ -107,15 +107,15 @@
     async def proxy_element(self, target: str):
         """Retrieve's an element through the actos' proxyUrl endpoint
         as specified in ActivityPub.
 
             :param target: The URL of the object to retrieve"""
         response = await self.client.post(
             self.information["endpoints"]["proxyUrl"],
-            f"id={target}",
+            urlencode({"id": target}),
             content_type="application/x-www-form-urlencoded",
         )
         response.raise_for_status()
         return await response.json()
 
     async def event_source(self):
         """Returns an EventSource corresponding to the actor's
@@ -164,28 +164,41 @@
         return urlparse(self.actor_id).netloc
 
     @property
     def followers(self) -> str:
         """The id of the follows collection"""
         return self.information["followers"]
 
-    async def inbox(self):
+    async def inbox(self, resolve=True):
         """Provides a CollectionHelper for the Actors inbox"""
         inbox_collection = CollectionHelper(
-            self.information["inbox"], self, resolve=True
+            self.information["inbox"], self, resolve=resolve
         )
         return inbox_collection
 
-    async def outbox(self):
+    async def outbox(self, resolve=True):
         """Provides a CollectionHelper for the Actors outbox"""
         inbox_collection = CollectionHelper(
-            self.information["outbox"], self, resolve=True
+            self.information["outbox"], self, resolve=resolve
         )
         return inbox_collection
 
+    def collection_helper(self, collection, resolve=False):
+        """Returns a CollectionHelper for the collection provided. Usage:
+
+        .. code-block:: python
+
+            async for x in client.collection_helper(uri_of_collection):
+                await do_something(x)
+
+        :param collection: Uri of the collection to irater over
+        :param resolve: If true objects are automatically fetched"""
+
+        return CollectionHelper(collection, self, resolve=resolve)
+
     @staticmethod
     def from_file(config_file: str):
         """Initializes the BovineClient from a toml config file"""
         with open(config_file, "rb") as fp:
             config = tomli.load(fp)
 
         return BovineClient(config)
```

### Comparing `bovine-0.2.6/bovine/activitystreams/__init__.py` & `bovine-0.3.0/bovine/activitystreams/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/activity_factory.py` & `bovine-0.3.0/bovine/activitystreams/activity_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,26 +82,26 @@
     def __init__(self, actor_information):
         self.information = actor_information
 
     def create(self, obj, **kwargs):
         """Activity of type Create from Object"""
         return Activity(
             type="Create",
-            actor=obj["attributedTo"],
+            actor=obj.get("attributedTo", None),
             cc=set(obj.get("cc", [])),
             to=set(obj.get("to", [])),
             object=obj,
             **kwargs
         )
 
     def update(self, obj, **kwargs):
         """Activity of type Update from Object"""
         return Activity(
             type="Update",
-            actor=obj["attributedTo"],
+            actor=obj.get("attributedTo", None),
             cc=set(obj.get("cc", [])),
             to=set(obj.get("to", [])),
             object=obj,
             **kwargs
         )
 
     def like(self, target, **kwargs):
```

### Comparing `bovine-0.2.6/bovine/activitystreams/collection_helper.py` & `bovine-0.3.0/bovine/activitystreams/collection_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from . import Collection
+
+
 class CollectionHelper:
     """Provides the ability to iterate over a Collection or OrderedCollection
 
     Usage:
 
     .. code-block:: python
 
@@ -13,14 +16,15 @@
     the data is provided by the remote server."""
 
     def __init__(self, collection_id: str, actor, resolve=False):
         self.actor = actor
         self.collection = collection_id
         self.items = []
         self.resolve = resolve
+        self.fetched_first = False
 
     def update_items(self):
         if not isinstance(self.collection, dict):
             return False
         if "orderedItems" in self.collection:
             self.items = self.collection["orderedItems"]
             return len(self.items) > 0
@@ -40,21 +44,32 @@
     async def __anext__(self):
         if len(self.items) > 0:
             return await self.resolve_item(self.items.pop(0))
         if isinstance(self.collection, str):
             self.collection = await self.actor.proxy_element(self.collection)
             if self.update_items():
                 return await self.resolve_item(self.items.pop(0))
-        if "first" in self.collection:
+        if not self.fetched_first and "first" in self.collection:
+            self.fetched_first = True
             self.collection = self.collection["first"]
             if self.update_items():
                 return await self.resolve_item(self.items.pop(0))
             else:
                 return await self.__anext__()
         if "next" in self.collection:
             self.collection = self.collection["next"]
             if self.update_items():
                 return await self.resolve_item(self.items.pop(0))
             else:
                 return await self.__anext__()
 
         raise StopAsyncIteration
+
+    async def as_collection(self):
+        items = [x async for x in self]
+        if isinstance(self.collection, dict):
+            collection_id = self.collection.get("part_of")
+            if not collection_id:
+                collection_id = self.collection["id"]
+        else:
+            collection_id = self.collection
+        return Collection(id=collection_id, items=items).build()
```

### Comparing `bovine-0.2.6/bovine/activitystreams/object_factory.py` & `bovine-0.3.0/bovine/activitystreams/object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/test_activity_factory.py` & `bovine-0.3.0/bovine/activitystreams/test_activity_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/test_actor.py` & `bovine-0.3.0/bovine/activitystreams/test_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/test_object_factory.py` & `bovine-0.3.0/bovine/activitystreams/test_object_factory.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/test_ordered_collection_builder.py` & `bovine-0.3.0/bovine/activitystreams/test_ordered_collection_builder.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/test_ordered_collection_page.py` & `bovine-0.3.0/bovine/activitystreams/test_ordered_collection_page.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/utils/__init__.py` & `bovine-0.3.0/bovine/activitystreams/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/utils/print.py` & `bovine-0.3.0/bovine/activitystreams/utils/print.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/activitystreams/utils/test_utils.py` & `bovine-0.3.0/bovine/activitystreams/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/__init__.py` & `bovine-0.3.0/bovine/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/authorization_wrapper.py` & `bovine-0.3.0/bovine/clients/authorization_wrapper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/bearer.py` & `bovine-0.3.0/bovine/clients/bearer.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/event_source.py` & `bovine-0.3.0/bovine/clients/event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/lookup_account.py` & `bovine-0.3.0/bovine/clients/lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/moo_auth.py` & `bovine-0.3.0/bovine/clients/moo_auth.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/nodeinfo.py` & `bovine-0.3.0/bovine/clients/nodeinfo.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/signed_http.py` & `bovine-0.3.0/bovine/clients/signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/signed_http_methods.py` & `bovine-0.3.0/bovine/clients/signed_http_methods.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/test_event_source.py` & `bovine-0.3.0/bovine/clients/test_event_source.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/test_lookup_account.py` & `bovine-0.3.0/bovine/clients/test_lookup_account.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/test_signed_http.py` & `bovine-0.3.0/bovine/clients/test_signed_http.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/clients/test_signed_http_client.py` & `bovine-0.3.0/bovine/clients/test_signed_http_client.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/__init__.py` & `bovine-0.3.0/bovine/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/__pycache__/test.cpython-310.pyc` & `bovine-0.3.0/bovine/crypto/test.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,148 +1,138 @@
-00000000: 6f0d 0d0a 0000 0000 88d8 7c64 9708 0000  o.........|d....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0001 0000 0040 0000 0073 0c00 0000 6400  .....@...s....d.
-00000030: 5a00 6401 5a01 6402 5300 2903 61c4 0100  Z.d.Z.d.S.).a...
-00000040: 000a 2d2d 2d2d 2d42 4547 494e 2050 5542  ..-----BEGIN PUB
-00000050: 4c49 4320 4b45 592d 2d2d 2d2d 0a4d 4949  LIC KEY-----.MII
-00000060: 4249 6a41 4e42 676b 7168 6b69 4739 7730  BIjANBgkqhkiG9w0
-00000070: 4241 5145 4641 414f 4341 5138 414d 4949  BAQEFAAOCAQ8AMII
-00000080: 4243 674b 4341 5145 4131 3576 6846 644b  BCgKCAQEA15vhFdK
-00000090: 3237 3262 6247 447a 4c74 7970 6f0a 344e  272bbGDzLtypo.4N
-000000a0: 6e38 6d4e 4659 3359 534c 6e72 414f 5834  n8mNFY3YSLnrAOX4
-000000b0: 7a5a 4b6b 4e6d 576d 6779 7067 4450 3871  zZKkNmWmgypgDP8q
-000000c0: 586a 4e69 5673 4266 3866 2b59 6b33 7448  XjNiVsBf8f+Yk3tH
-000000d0: 4473 3538 4c4d 6638 5144 5350 3039 0a41  Ds58LMf8QDSP09.A
-000000e0: 2b7a 726c 5742 484e 3172 4c45 4c6e 304a  +zrlWBHN1rLELn0J
-000000f0: 4267 7154 3978 6a38 5753 6f62 4449 6a4f  BgqT9xj8WSobDIjO
-00000100: 6a46 4241 7934 464b 556b 6f37 6b2f 4973  jFBAy4FKUko7k/Is
-00000110: 5977 546c 2f56 6e78 3174 796b 6850 520a  YwTl/Vnx1tykhPR.
-00000120: 3155 7a62 614e 714e 3179 5153 7930 7a47  1UzbaNqN1yQSy0zG
-00000130: 6249 6365 2f58 6871 6c7a 6d36 752b 7477  bIce/Xhqlzm6u+tw
-00000140: 7975 4856 4374 6247 5063 5068 3766 6f72  yuHVCtbGPcPh7for
-00000150: 356f 3061 764b 644d 7768 4158 7057 4d72  5o0avKdMwhAXpWMr
-00000160: 0a4e 6f63 394c 324c 2f39 6833 5567 6f65  .Noc9L2L/9h3Ugoe
-00000170: 5067 4176 4345 3648 5450 5845 4250 6573  PgAvCE6HTPXEBPes
-00000180: 5542 6c54 554c 6352 784d 5849 5a4a 3750  UBlTULcRxMXIZJ7P
-00000190: 3665 4d6b 6232 7047 5543 446c 5646 3445  6eMkb2pGUCDlVF4E
-000001a0: 4e0a 7663 785a 4147 3850 6237 4851 7039  N.vcxZAG8Pb7HQp9
-000001b0: 6e7a 5677 4b34 4f58 5a63 6c4b 7348 3159  nzVwK4OXZclKsH1Y
-000001c0: 4b30 4738 6f42 4754 786e 726f 4274 7137  K0G8oBGTxnroBtq7
-000001d0: 634a 6272 4a76 714e 4d4e 4f4f 3559 6733  cJbrJvqNMNOO5Yg3
-000001e0: 6375 0a36 5149 4441 5141 420a 2d2d 2d2d  cu.6QIDAQAB.----
-000001f0: 2d45 4e44 2050 5542 4c49 4320 4b45 592d  -END PUBLIC KEY-
-00000200: 2d2d 2d2d 0a61 a906 0000 0a2d 2d2d 2d2d  ----.a.....-----
-00000210: 4245 4749 4e20 5052 4956 4154 4520 4b45  BEGIN PRIVATE KE
-00000220: 592d 2d2d 2d2d 0a4d 4949 4576 6749 4241  Y-----.MIIEvgIBA
-00000230: 4441 4e42 676b 7168 6b69 4739 7730 4241  DANBgkqhkiG9w0BA
-00000240: 5145 4641 4153 4342 4b67 7767 6753 6b41  QEFAASCBKgwggSkA
-00000250: 6745 4141 6f49 4241 5144 586d 2b45 5630  gEAAoIBAQDXm+EV0
-00000260: 7262 765a 7473 590a 504d 7533 4b6d 6a67  rbvZtsY.PMu3Kmjg
-00000270: 3266 7959 3056 6a64 6849 7565 7341 3566  2fyY0VjdhIuesA5f
-00000280: 6a4e 6b71 5132 5a61 6144 4b6d 414d 2f79  jNkqQ2ZaaDKmAM/y
-00000290: 7065 4d32 4a57 7746 2f78 2f35 6954 6530  peM2JWwF/x/5iTe0
-000002a0: 634f 7a6e 7773 782f 0a78 414e 492f 5430  cOznwsx/.xANI/T0
-000002b0: 4437 4f75 5659 4563 3357 7373 5175 6651  D7OuVYEc3WssQufQ
-000002c0: 6b47 4370 5033 4750 785a 4b68 734d 694d  kGCpP3GPxZKhsMiM
-000002d0: 364d 5545 444c 6755 7053 536a 7554 3869  6MUEDLgUpSSjuT8i
-000002e0: 786a 424f 5839 5766 480a 5733 4b53 4539  xjBOX9WfH.W3KSE9
-000002f0: 4856 544e 746f 326f 3358 4a42 4c4c 544d  HVTNto2o3XJBLLTM
-00000300: 5a73 6878 3739 6547 7158 4f62 7137 3633  Zshx79eGqXObq763
-00000310: 444b 3464 554b 3173 5939 772b 4874 2b69  DK4dUK1sY9w+Ht+i
-00000320: 766d 6a52 7138 7030 7a43 0a45 4265 6c59  vmjRq8p0zC.EBelY
-00000330: 7973 3268 7a30 7659 762f 3248 6453 4368  ys2hz0vYv/2HdSCh
-00000340: 342b 4143 3849 546f 644d 3963 5145 3936  4+AC8ITodM9cQE96
-00000350: 7851 4756 4e51 7478 4845 7863 686b 6e73  xQGVNQtxHExchkns
-00000360: 2f70 3479 5276 616b 5a51 490a 4f56 5558  /p4yRvakZQI.OVUX
-00000370: 6751 3239 7a46 6b41 6277 3976 7364 436e  gQ29zFkAbw9vsdCn
-00000380: 3266 4e58 4172 6735 646c 7955 7177 6656  2fNXArg5dlyUqwfV
-00000390: 6772 5162 7967 455a 5047 6575 6747 3272  grQbygEZPGeugG2r
-000003a0: 7477 6c75 736d 2b6f 3077 3034 0a37 6c69  twlusm+o0w04.7li
-000003b0: 4464 7937 7041 674d 4241 4145 4367 6745  Ddy7pAgMBAAECggE
-000003c0: 4153 3954 7459 346d 4c41 6353 4252 704d  AS9TtY4mLAcSBRpM
-000003d0: 4c61 3036 6c4f 4941 7930 5754 4142 706b  La06lOIAy0WTABpk
-000003e0: 3571 6752 7436 626c 5749 4145 340a 6e49  5qgRt6blWIAE4.nI
-000003f0: 2b4e 554d 6c30 5766 6c79 596e 6269 2b58  +NUMl0WflyYnbi+X
-00000400: 447a 7841 5934 3632 5055 5475 6336 6d61  DzxAY462PUTuc6ma
-00000410: 314e 496e 792b 3277 5358 4479 4366 7135  1NIny+2wSXDyCfq5
-00000420: 3570 5557 6131 7359 5132 5459 524d 0a4f  5pUWa1sYQ2TYRM.O
-00000430: 6e69 5772 4163 7555 4b64 4749 4749 744f  niWrAcuUKdGIGItO
-00000440: 6f6f 6174 5561 6d5a 5a76 4977 4764 3171  ooatUamZZvIwGd1q
-00000450: 7135 464b 342b 412b 3635 6564 5242 3556  q5FK4+A+65edRB5V
-00000460: 724f 2f55 4857 6554 456c 7834 742b 7a0a  rO/UHWeTElx4t+z.
-00000470: 3053 5579 6662 7065 4348 7675 4545 4b33  0SUyfbpeCHvuEEK3
-00000480: 4f79 5934 3634 5634 5a57 2f44 2f7a 4141  OyY464V4ZW/D/zAA
-00000490: 4f4e 6143 4633 6e2b 4659 3975 4253 302b  ONaCF3n+FY9uBS0+
-000004a0: 394c 456d 6530 7876 6142 7132 346f 4639  9LEme0xvaBq24oF9
-000004b0: 0a7a 6d62 464a 3544 6a46 5352 704e 566f  .zmbFJ5DjFSRpNVo
-000004c0: 7547 526d 4f30 3355 6839 2b75 4e72 5459  uGRmO03Uh9+uNrTY
-000004d0: 6b63 796c 444e 6751 6146 4374 3757 6351  kcylDNgQaFCt7WcQ
-000004e0: 4f2f 336c 4373 2b64 714e 6632 7073 4968  O/3lCs+dqNf2psIh
-000004f0: 740a 5043 624c 5271 6658 5153 6a51 3667  t.PCbLRqfXQSjQ6g
-00000500: 5162 6e59 5047 6d49 4665 7356 5677 4a70  QbnYPGmIFesVVwJp
-00000510: 5379 4d58 7046 4d63 6749 5351 4b42 6751  SyMXpFMcgISQKBgQ
-00000520: 4466 4273 6d43 424e 3070 4669 6234 7661  DfBsmCBN0pFib4va
-00000530: 4d66 0a31 4b53 4c56 7867 3744 4646 6945  Mf.1KSLVxg7DFFiE
-00000540: 4c66 3144 306f 6b34 7253 6137 4835 656f  Lf1D0ok4rSa7H5eo
-00000550: 3566 6c4e 4e44 3978 752b 4553 5751 7063  5flNND9xu+ESWQpc
-00000560: 7139 4a30 5056 475a 7166 5837 7065 6e39  q9J0PVGZqfX7pen9
-00000570: 454a 560a 486d 4e50 4d59 7341 656a 5471  EJV.HmNPMYsAejTq
-00000580: 484d 2f31 6267 3354 6457 3341 3458 6e30  HM/1bg3TdW3A4Xn0
-00000590: 4932 5368 6c5a 6c4e 4b30 417a 4c59 5a52  I2ShlZlNK0AzLYZR
-000005a0: 4942 4630 5a69 4357 756e 5a42 7438 786a  IBF0ZiCWunZBt8xj
-000005b0: 534c 546d 0a42 4748 5a78 7668 6f31 545a  SLTm.BGHZxvho1TZ
-000005c0: 4966 6675 7564 6378 5035 6f6c 5933 774b  IffuudcxP5olY3wK
-000005d0: 4267 5144 3366 466a 5151 742f 6277 2f32  BgQD3fFjQQt/bw/2
-000005e0: 4a59 5542 4676 6a50 6956 4f4a 356a 354d  JYUBFvjPiVOJ5j5M
-000005f0: 7a61 474c 780a 6774 7044 4d55 4654 7547  zaGLx.gtpDMUFTuG
-00000600: 2f44 5058 5576 5457 7036 7849 6b51 6a34  /DPXUvTWp6xIkQj4
-00000610: 784f 3544 3953 666b 5471 4245 504f 4748  xO5D9SfkTqBEPOGH
-00000620: 2f7a 6337 4356 6f54 4d73 6835 7648 444a  /zc7CVoTMsh5vHDJ
-00000630: 3966 4b45 2f6c 0a46 796e 5161 437a 424f  9fKE/l.FynQaCzBO
-00000640: 7255 2b7a 4b65 4876 4273 6353 3931 6f72  rU+zKeHvBscS91or
-00000650: 4630 6e4e 7244 334a 5974 6234 4755 6531  F0nNrD3JYtb4GUe1
-00000660: 6f53 5a2f 426c 6277 486a 5a4d 5a51 4f41  oSZ/BlbwHjZMZQOA
-00000670: 7373 614c 4473 310a 4264 7135 5370 4c4a  ssaLDs1.Bdq5SpLJ
-00000680: 4e77 4b42 6744 5869 552b 6b2f 3935 636e  NwKBgDXiU+k/95cn
-00000690: 7250 3749 4170 4e38 4d73 3066 6d39 4559  rP7IApN8Ms0fm9EY
-000006a0: 5a73 6c45 744d 3157 686c 6c6e 464b 2b68  ZslEtM1WhllnFK+h
-000006b0: 6c39 3652 732b 3943 0a31 594f 612f 7439  l96Rs+9C.1YOa/t9
-000006c0: 3951 392f 6e76 3459 6349 4561 4549 7555  9Q9/nv4YcIEaEIuU
-000006d0: 2b31 6846 554b 4871 6350 7534 7855 4234  +1hFUKHqcPu4xUB4
-000006e0: 7261 4946 7675 4b62 5a6b 696d 5734 342b  raIFvuKbZkimW44+
-000006f0: 4961 6f69 627a 494a 6c0a 7649 5979 6675  IaoibzIJl.vIYyfu
-00000700: 3565 6632 6332 556b 4648 4d33 5233 5648  5ef2c2UkFHM3R3VH
-00000710: 3849 5179 3978 7235 4d72 562b 4466 2b38  8IQy9xr5MrV+Df+8
-00000720: 4349 5576 6373 7952 5162 6a65 4e34 465a  CIUvcsyRQbjeN4FZ
-00000730: 4d4e 416f 4742 414f 4b42 0a4e 7850 6373  MNAoGBAOKB.NxPcs
-00000740: 4e2b 4659 4331 3143 5973 4c53 7063 7945  N+FYC11CYsLSpcyE
-00000750: 316b 6f63 3550 5154 5159 334f 6158 586c  1koc5PQTQY3OaXXl
-00000760: 612b 5846 5172 2b32 3571 6759 767a 626c  a+XFQr+25qgYvzbl
-00000770: 5972 4870 7157 7074 7436 380a 5844 7847  YrHpqWptt68.XDxG
-00000780: 4450 7936 5a5a 6965 594a 6142 7738 4655  DPy6ZZieYJaBw8FU
-00000790: 6c39 6b30 6a30 5262 4d38 7737 522f 544b  l9k0j0RbM8w7R/TK
-000007a0: 3833 4d69 5654 4756 7778 7179 7161 6c62  83MiVTGVwxqyqalb
-000007b0: 4d64 6755 4d4f 6d72 3334 6c44 0a48 6d6e  MdgUMOmr34lD.Hmn
-000007c0: 4856 5356 464e 6e56 7353 7055 7a38 6962  HVSVFNnVsSpUz8ib
-000007d0: 7566 6b2f 5964 4b53 4f71 4e32 6462 784b  ufk/YdKSOqN2dbxK
-000007e0: 3430 7545 2f41 6f47 4241 4c47 7252 3546  40uE/AoGBALGrR5F
-000007f0: 5532 7531 7663 7355 6a31 4976 540a 6570  U2u1vcsUj1IvT.ep
-00000800: 6641 352b 386b 6951 354d 6455 5755 2b45  fA5+8kiQ5MdUWU+E
-00000810: 374f 524d 2b53 526c 6e69 6373 6453 2f49  7ORM+SRlnicsdS/I
-00000820: 5054 344b 5245 4263 6b2f 2b47 7658 592f  PT4KREBck/+GvXY/
-00000830: 585a 644d 5954 2b54 3361 346f 3350 0a52  XZdMYT+T3a4o3P.R
-00000840: 344f 332f 3265 6771 5463 6875 506b 7766  4O3/2egqTchuPkwf
-00000850: 5341 7937 4c38 6a74 3247 4e7a 4676 786d  SAy7L8jt2GNzFvxm
-00000860: 6372 7670 4b59 415a 7a6a 6831 4b43 725a  crvpKYAZzjh1KCrZ
-00000870: 3135 4f59 7237 5a68 6c45 5773 364d 510a  15OYr7ZhlEWs6MQ.
-00000880: 5262 6444 7133 364f 3435 7570 6c4f 6530  RbdDq36O45uplOe0
-00000890: 6865 654f 7350 686a 0a2d 2d2d 2d2d 454e  heeOsPhj.-----EN
-000008a0: 4420 5052 4956 4154 4520 4b45 592d 2d2d  D PRIVATE KEY---
-000008b0: 2d2d 0a4e 2902 da0a 7075 626c 6963 5f6b  --.N)...public_k
-000008c0: 6579 da0b 7072 6976 6174 655f 6b65 79a9  ey..private_key.
-000008d0: 0072 0300 0000 7203 0000 00fa 472f 776f  .r....r.....G/wo
-000008e0: 6f64 7065 636b 6572 2f73 7263 2f63 6f64  odpecker/src/cod
-000008f0: 6562 6572 672e 6f72 672f 626f 7669 6e65  eberg.org/bovine
-00000900: 2f62 6f76 696e 652f 626f 7669 6e65 2f62  /bovine/bovine/b
-00000910: 6f76 696e 652f 6372 7970 746f 2f74 6573  ovine/crypto/tes
-00000920: 742e 7079 da08 3c6d 6f64 756c 653e 0100  t.py..<module>..
-00000930: 0000 7304 0000 0004 0008 0c              ..s........
+00000000: 7075 626c 6963 5f6b 6579 203d 2022 2222  public_key = """
+00000010: 0a2d 2d2d 2d2d 4245 4749 4e20 5055 424c  .-----BEGIN PUBL
+00000020: 4943 204b 4559 2d2d 2d2d 2d0a 4d49 4942  IC KEY-----.MIIB
+00000030: 496a 414e 4267 6b71 686b 6947 3977 3042  IjANBgkqhkiG9w0B
+00000040: 4151 4546 4141 4f43 4151 3841 4d49 4942  AQEFAAOCAQ8AMIIB
+00000050: 4367 4b43 4151 4541 3135 7668 4664 4b32  CgKCAQEA15vhFdK2
+00000060: 3732 6262 4744 7a4c 7479 706f 0a34 4e6e  72bbGDzLtypo.4Nn
+00000070: 386d 4e46 5933 5953 4c6e 7241 4f58 347a  8mNFY3YSLnrAOX4z
+00000080: 5a4b 6b4e 6d57 6d67 7970 6744 5038 7158  ZKkNmWmgypgDP8qX
+00000090: 6a4e 6956 7342 6638 662b 596b 3374 4844  jNiVsBf8f+Yk3tHD
+000000a0: 7335 384c 4d66 3851 4453 5030 390a 412b  s58LMf8QDSP09.A+
+000000b0: 7a72 6c57 4248 4e31 724c 454c 6e30 4a42  zrlWBHN1rLELn0JB
+000000c0: 6771 5439 786a 3857 536f 6244 496a 4f6a  gqT9xj8WSobDIjOj
+000000d0: 4642 4179 3446 4b55 6b6f 376b 2f49 7359  FBAy4FKUko7k/IsY
+000000e0: 7754 6c2f 566e 7831 7479 6b68 5052 0a31  wTl/Vnx1tykhPR.1
+000000f0: 557a 6261 4e71 4e31 7951 5379 307a 4762  UzbaNqN1yQSy0zGb
+00000100: 4963 652f 5868 716c 7a6d 3675 2b74 7779  Ice/Xhqlzm6u+twy
+00000110: 7548 5643 7462 4750 6350 6837 666f 7235  uHVCtbGPcPh7for5
+00000120: 6f30 6176 4b64 4d77 6841 5870 574d 720a  o0avKdMwhAXpWMr.
+00000130: 4e6f 6339 4c32 4c2f 3968 3355 676f 6550  Noc9L2L/9h3UgoeP
+00000140: 6741 7643 4536 4854 5058 4542 5065 7355  gAvCE6HTPXEBPesU
+00000150: 426c 5455 4c63 5278 4d58 495a 4a37 5036  BlTULcRxMXIZJ7P6
+00000160: 654d 6b62 3270 4755 4344 6c56 4634 454e  eMkb2pGUCDlVF4EN
+00000170: 0a76 6378 5a41 4738 5062 3748 5170 396e  .vcxZAG8Pb7HQp9n
+00000180: 7a56 774b 344f 585a 636c 4b73 4831 594b  zVwK4OXZclKsH1YK
+00000190: 3047 386f 4247 5478 6e72 6f42 7471 3763  0G8oBGTxnroBtq7c
+000001a0: 4a62 724a 7671 4e4d 4e4f 4f35 5967 3363  JbrJvqNMNOO5Yg3c
+000001b0: 750a 3651 4944 4151 4142 0a2d 2d2d 2d2d  u.6QIDAQAB.-----
+000001c0: 454e 4420 5055 424c 4943 204b 4559 2d2d  END PUBLIC KEY--
+000001d0: 2d2d 2d0a 2222 220a 0a70 7269 7661 7465  ---."""..private
+000001e0: 5f6b 6579 203d 2022 2222 0a2d 2d2d 2d2d  _key = """.-----
+000001f0: 4245 4749 4e20 5052 4956 4154 4520 4b45  BEGIN PRIVATE KE
+00000200: 592d 2d2d 2d2d 0a4d 4949 4576 6749 4241  Y-----.MIIEvgIBA
+00000210: 4441 4e42 676b 7168 6b69 4739 7730 4241  DANBgkqhkiG9w0BA
+00000220: 5145 4641 4153 4342 4b67 7767 6753 6b41  QEFAASCBKgwggSkA
+00000230: 6745 4141 6f49 4241 5144 586d 2b45 5630  gEAAoIBAQDXm+EV0
+00000240: 7262 765a 7473 590a 504d 7533 4b6d 6a67  rbvZtsY.PMu3Kmjg
+00000250: 3266 7959 3056 6a64 6849 7565 7341 3566  2fyY0VjdhIuesA5f
+00000260: 6a4e 6b71 5132 5a61 6144 4b6d 414d 2f79  jNkqQ2ZaaDKmAM/y
+00000270: 7065 4d32 4a57 7746 2f78 2f35 6954 6530  peM2JWwF/x/5iTe0
+00000280: 634f 7a6e 7773 782f 0a78 414e 492f 5430  cOznwsx/.xANI/T0
+00000290: 4437 4f75 5659 4563 3357 7373 5175 6651  D7OuVYEc3WssQufQ
+000002a0: 6b47 4370 5033 4750 785a 4b68 734d 694d  kGCpP3GPxZKhsMiM
+000002b0: 364d 5545 444c 6755 7053 536a 7554 3869  6MUEDLgUpSSjuT8i
+000002c0: 786a 424f 5839 5766 480a 5733 4b53 4539  xjBOX9WfH.W3KSE9
+000002d0: 4856 544e 746f 326f 3358 4a42 4c4c 544d  HVTNto2o3XJBLLTM
+000002e0: 5a73 6878 3739 6547 7158 4f62 7137 3633  Zshx79eGqXObq763
+000002f0: 444b 3464 554b 3173 5939 772b 4874 2b69  DK4dUK1sY9w+Ht+i
+00000300: 766d 6a52 7138 7030 7a43 0a45 4265 6c59  vmjRq8p0zC.EBelY
+00000310: 7973 3268 7a30 7659 762f 3248 6453 4368  ys2hz0vYv/2HdSCh
+00000320: 342b 4143 3849 546f 644d 3963 5145 3936  4+AC8ITodM9cQE96
+00000330: 7851 4756 4e51 7478 4845 7863 686b 6e73  xQGVNQtxHExchkns
+00000340: 2f70 3479 5276 616b 5a51 490a 4f56 5558  /p4yRvakZQI.OVUX
+00000350: 6751 3239 7a46 6b41 6277 3976 7364 436e  gQ29zFkAbw9vsdCn
+00000360: 3266 4e58 4172 6735 646c 7955 7177 6656  2fNXArg5dlyUqwfV
+00000370: 6772 5162 7967 455a 5047 6575 6747 3272  grQbygEZPGeugG2r
+00000380: 7477 6c75 736d 2b6f 3077 3034 0a37 6c69  twlusm+o0w04.7li
+00000390: 4464 7937 7041 674d 4241 4145 4367 6745  Ddy7pAgMBAAECggE
+000003a0: 4153 3954 7459 346d 4c41 6353 4252 704d  AS9TtY4mLAcSBRpM
+000003b0: 4c61 3036 6c4f 4941 7930 5754 4142 706b  La06lOIAy0WTABpk
+000003c0: 3571 6752 7436 626c 5749 4145 340a 6e49  5qgRt6blWIAE4.nI
+000003d0: 2b4e 554d 6c30 5766 6c79 596e 6269 2b58  +NUMl0WflyYnbi+X
+000003e0: 447a 7841 5934 3632 5055 5475 6336 6d61  DzxAY462PUTuc6ma
+000003f0: 314e 496e 792b 3277 5358 4479 4366 7135  1NIny+2wSXDyCfq5
+00000400: 3570 5557 6131 7359 5132 5459 524d 0a4f  5pUWa1sYQ2TYRM.O
+00000410: 6e69 5772 4163 7555 4b64 4749 4749 744f  niWrAcuUKdGIGItO
+00000420: 6f6f 6174 5561 6d5a 5a76 4977 4764 3171  ooatUamZZvIwGd1q
+00000430: 7135 464b 342b 412b 3635 6564 5242 3556  q5FK4+A+65edRB5V
+00000440: 724f 2f55 4857 6554 456c 7834 742b 7a0a  rO/UHWeTElx4t+z.
+00000450: 3053 5579 6662 7065 4348 7675 4545 4b33  0SUyfbpeCHvuEEK3
+00000460: 4f79 5934 3634 5634 5a57 2f44 2f7a 4141  OyY464V4ZW/D/zAA
+00000470: 4f4e 6143 4633 6e2b 4659 3975 4253 302b  ONaCF3n+FY9uBS0+
+00000480: 394c 456d 6530 7876 6142 7132 346f 4639  9LEme0xvaBq24oF9
+00000490: 0a7a 6d62 464a 3544 6a46 5352 704e 566f  .zmbFJ5DjFSRpNVo
+000004a0: 7547 526d 4f30 3355 6839 2b75 4e72 5459  uGRmO03Uh9+uNrTY
+000004b0: 6b63 796c 444e 6751 6146 4374 3757 6351  kcylDNgQaFCt7WcQ
+000004c0: 4f2f 336c 4373 2b64 714e 6632 7073 4968  O/3lCs+dqNf2psIh
+000004d0: 740a 5043 624c 5271 6658 5153 6a51 3667  t.PCbLRqfXQSjQ6g
+000004e0: 5162 6e59 5047 6d49 4665 7356 5677 4a70  QbnYPGmIFesVVwJp
+000004f0: 5379 4d58 7046 4d63 6749 5351 4b42 6751  SyMXpFMcgISQKBgQ
+00000500: 4466 4273 6d43 424e 3070 4669 6234 7661  DfBsmCBN0pFib4va
+00000510: 4d66 0a31 4b53 4c56 7867 3744 4646 6945  Mf.1KSLVxg7DFFiE
+00000520: 4c66 3144 306f 6b34 7253 6137 4835 656f  Lf1D0ok4rSa7H5eo
+00000530: 3566 6c4e 4e44 3978 752b 4553 5751 7063  5flNND9xu+ESWQpc
+00000540: 7139 4a30 5056 475a 7166 5837 7065 6e39  q9J0PVGZqfX7pen9
+00000550: 454a 560a 486d 4e50 4d59 7341 656a 5471  EJV.HmNPMYsAejTq
+00000560: 484d 2f31 6267 3354 6457 3341 3458 6e30  HM/1bg3TdW3A4Xn0
+00000570: 4932 5368 6c5a 6c4e 4b30 417a 4c59 5a52  I2ShlZlNK0AzLYZR
+00000580: 4942 4630 5a69 4357 756e 5a42 7438 786a  IBF0ZiCWunZBt8xj
+00000590: 534c 546d 0a42 4748 5a78 7668 6f31 545a  SLTm.BGHZxvho1TZ
+000005a0: 4966 6675 7564 6378 5035 6f6c 5933 774b  IffuudcxP5olY3wK
+000005b0: 4267 5144 3366 466a 5151 742f 6277 2f32  BgQD3fFjQQt/bw/2
+000005c0: 4a59 5542 4676 6a50 6956 4f4a 356a 354d  JYUBFvjPiVOJ5j5M
+000005d0: 7a61 474c 780a 6774 7044 4d55 4654 7547  zaGLx.gtpDMUFTuG
+000005e0: 2f44 5058 5576 5457 7036 7849 6b51 6a34  /DPXUvTWp6xIkQj4
+000005f0: 784f 3544 3953 666b 5471 4245 504f 4748  xO5D9SfkTqBEPOGH
+00000600: 2f7a 6337 4356 6f54 4d73 6835 7648 444a  /zc7CVoTMsh5vHDJ
+00000610: 3966 4b45 2f6c 0a46 796e 5161 437a 424f  9fKE/l.FynQaCzBO
+00000620: 7255 2b7a 4b65 4876 4273 6353 3931 6f72  rU+zKeHvBscS91or
+00000630: 4630 6e4e 7244 334a 5974 6234 4755 6531  F0nNrD3JYtb4GUe1
+00000640: 6f53 5a2f 426c 6277 486a 5a4d 5a51 4f41  oSZ/BlbwHjZMZQOA
+00000650: 7373 614c 4473 310a 4264 7135 5370 4c4a  ssaLDs1.Bdq5SpLJ
+00000660: 4e77 4b42 6744 5869 552b 6b2f 3935 636e  NwKBgDXiU+k/95cn
+00000670: 7250 3749 4170 4e38 4d73 3066 6d39 4559  rP7IApN8Ms0fm9EY
+00000680: 5a73 6c45 744d 3157 686c 6c6e 464b 2b68  ZslEtM1WhllnFK+h
+00000690: 6c39 3652 732b 3943 0a31 594f 612f 7439  l96Rs+9C.1YOa/t9
+000006a0: 3951 392f 6e76 3459 6349 4561 4549 7555  9Q9/nv4YcIEaEIuU
+000006b0: 2b31 6846 554b 4871 6350 7534 7855 4234  +1hFUKHqcPu4xUB4
+000006c0: 7261 4946 7675 4b62 5a6b 696d 5734 342b  raIFvuKbZkimW44+
+000006d0: 4961 6f69 627a 494a 6c0a 7649 5979 6675  IaoibzIJl.vIYyfu
+000006e0: 3565 6632 6332 556b 4648 4d33 5233 5648  5ef2c2UkFHM3R3VH
+000006f0: 3849 5179 3978 7235 4d72 562b 4466 2b38  8IQy9xr5MrV+Df+8
+00000700: 4349 5576 6373 7952 5162 6a65 4e34 465a  CIUvcsyRQbjeN4FZ
+00000710: 4d4e 416f 4742 414f 4b42 0a4e 7850 6373  MNAoGBAOKB.NxPcs
+00000720: 4e2b 4659 4331 3143 5973 4c53 7063 7945  N+FYC11CYsLSpcyE
+00000730: 316b 6f63 3550 5154 5159 334f 6158 586c  1koc5PQTQY3OaXXl
+00000740: 612b 5846 5172 2b32 3571 6759 767a 626c  a+XFQr+25qgYvzbl
+00000750: 5972 4870 7157 7074 7436 380a 5844 7847  YrHpqWptt68.XDxG
+00000760: 4450 7936 5a5a 6965 594a 6142 7738 4655  DPy6ZZieYJaBw8FU
+00000770: 6c39 6b30 6a30 5262 4d38 7737 522f 544b  l9k0j0RbM8w7R/TK
+00000780: 3833 4d69 5654 4756 7778 7179 7161 6c62  83MiVTGVwxqyqalb
+00000790: 4d64 6755 4d4f 6d72 3334 6c44 0a48 6d6e  MdgUMOmr34lD.Hmn
+000007a0: 4856 5356 464e 6e56 7353 7055 7a38 6962  HVSVFNnVsSpUz8ib
+000007b0: 7566 6b2f 5964 4b53 4f71 4e32 6462 784b  ufk/YdKSOqN2dbxK
+000007c0: 3430 7545 2f41 6f47 4241 4c47 7252 3546  40uE/AoGBALGrR5F
+000007d0: 5532 7531 7663 7355 6a31 4976 540a 6570  U2u1vcsUj1IvT.ep
+000007e0: 6641 352b 386b 6951 354d 6455 5755 2b45  fA5+8kiQ5MdUWU+E
+000007f0: 374f 524d 2b53 526c 6e69 6373 6453 2f49  7ORM+SRlnicsdS/I
+00000800: 5054 344b 5245 4263 6b2f 2b47 7658 592f  PT4KREBck/+GvXY/
+00000810: 585a 644d 5954 2b54 3361 346f 3350 0a52  XZdMYT+T3a4o3P.R
+00000820: 344f 332f 3265 6771 5463 6875 506b 7766  4O3/2egqTchuPkwf
+00000830: 5341 7937 4c38 6a74 3247 4e7a 4676 786d  SAy7L8jt2GNzFvxm
+00000840: 6372 7670 4b59 415a 7a6a 6831 4b43 725a  crvpKYAZzjh1KCrZ
+00000850: 3135 4f59 7237 5a68 6c45 5773 364d 510a  15OYr7ZhlEWs6MQ.
+00000860: 5262 6444 7133 364f 3435 7570 6c4f 6530  RbdDq36O45uplOe0
+00000870: 6865 654f 7350 686a 0a2d 2d2d 2d2d 454e  heeOsPhj.-----EN
+00000880: 4420 5052 4956 4154 4520 4b45 592d 2d2d  D PRIVATE KEY---
+00000890: 2d2d 0a22 2222 0a                        --.""".
```

### Comparing `bovine-0.2.6/bovine/crypto/helper.py` & `bovine-0.3.0/bovine/crypto/helper.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 
 def verify_signature(public_key, message, signature):
     public_key_loaded = load_pem_public_key(public_key.encode("utf-8"))
 
     assert isinstance(public_key_loaded, rsa.RSAPublicKey)
 
     try:
+        print(message)
         public_key_loaded.verify(
             base64.standard_b64decode(signature),
             message.encode("utf-8"),
             padding.PKCS1v15(),
             hashes.SHA256(),
         )
     except InvalidSignature:
```

### Comparing `bovine-0.2.6/bovine/crypto/http_signature.py` & `bovine-0.3.0/bovine/crypto/http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/signature_checker.py` & `bovine-0.3.0/bovine/crypto/signature_checker.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/signature_parser.py` & `bovine-0.3.0/bovine/crypto/signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/test_crypto.py` & `bovine-0.3.0/bovine/crypto/test_crypto.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/test_helper.py` & `bovine-0.3.0/bovine/crypto/test_helper.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/test_http_signature.py` & `bovine-0.3.0/bovine/crypto/test_http_signature.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/crypto/test_signature_parser.py` & `bovine-0.3.0/bovine/crypto/test_signature_parser.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/jsonld.py` & `bovine-0.3.0/bovine/jsonld.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     {
         "publicKey": {"@id": "https://w3id.org/security#publicKey", "@type": "@id"},
         "publicKeyPem": "https://w3id.org/security#publicKeyPem",
         "owner": {"@id": "https://w3id.org/security#owner", "@type": "@id"},
         "to": {"@id": "as:to", "@type": "@id", "@container": "@set"},
         "cc": {"@id": "as:cc", "@type": "@id", "@container": "@set"},
         "tag": {"@id": "as:tag", "@type": "@id", "@container": "@set"},
+        "items": {"@id": "as:items", "@type": "@id", "@container": "@set"},
         "attachment": {"@id": "as:attachment", "@type": "@id", "@container": "@set"},
         "Hashtag": "as:Hashtag",
     },
 ]
 """ Defines the context about:bovine used internally in the bovine stack"""
```

### Comparing `bovine-0.2.6/bovine/msg.py` & `bovine-0.3.0/bovine/msg.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/repl.py` & `bovine-0.3.0/bovine/repl.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/test_bovine_actor.py` & `bovine-0.3.0/bovine/test_bovine_actor.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/test_jsonld.py` & `bovine-0.3.0/bovine/test_jsonld.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/types.py` & `bovine-0.3.0/bovine/types.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/__init__.py` & `bovine-0.3.0/bovine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/date.py` & `bovine-0.3.0/bovine/utils/date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/msg/__init__.py` & `bovine-0.3.0/bovine/utils/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/msg/test_validation.py` & `bovine-0.3.0/bovine/utils/msg/test_validation.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/pyld_requests.py` & `bovine-0.3.0/bovine/utils/pyld_requests.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/bovine/utils/test_date.py` & `bovine-0.3.0/bovine/utils/test_date.py`

 * *Files identical despite different names*

### Comparing `bovine-0.2.6/pyproject.toml` & `bovine-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bovine"
-version = "0.2.6"
+version = "0.3.0"
 description = "Core functionality of bovine needed to build fediverse applications"
 authors = ["Helge <helge.krueger@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bovine" }]
 repository = "https://codeberg.org/bovine/bovine"
 documentation = "https://bovine.readthedocs.io/en/latest/"
```

### Comparing `bovine-0.2.6/PKG-INFO` & `bovine-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bovine
-Version: 0.2.6
+Version: 0.3.0
 Summary: Core functionality of bovine needed to build fediverse applications
 Home-page: https://codeberg.org/bovine/bovine
 License: MIT
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

