# Comparing `tmp/mercoa-0.2.1.tar.gz` & `tmp/mercoa-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.2.1.tar", max compression
+gzip compressed data, was "mercoa-0.2.2.tar", max compression
```

## Comparing `mercoa-0.2.1.tar` & `mercoa-0.2.2.tar`

### file list

```diff
@@ -1,183 +1,196 @@
--rw-r--r--   0        0        0     1930 2023-07-11 00:12:39.048495 mercoa-0.2.1/README.md
--rw-r--r--   0        0        0      368 2023-07-11 00:12:39.048495 mercoa-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7261 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/__init__.py
--rw-r--r--   0        0        0     2384 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/py.typed
--rw-r--r--   0        0        0     7370 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     3801 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      499 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      314 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      225 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      469 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0      824 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0      994 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0      857 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0      855 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0      471 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    33579 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0      453 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      228 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    17689 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4109 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    11242 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    22306 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    12767 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    15327 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0     1911 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/__init__.py
--rw-r--r--   0        0        0     2766 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/__init__.py
--rw-r--r--   0        0        0      487 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/account_type.py
--rw-r--r--   0        0        0      849 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/amount_trigger.py
--rw-r--r--   0        0        0       88 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_id.py
--rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_request.py
--rw-r--r--   0        0        0     1036 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_response.py
--rw-r--r--   0        0        0     1067 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      963 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approver_rule.py
--rw-r--r--   0        0        0     1535 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_type.py
--rw-r--r--   0        0        0     1013 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/counterparty_response.py
--rw-r--r--   0        0        0      741 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/ein.py
--rw-r--r--   0        0        0      914 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
--rw-r--r--   0        0        0       80 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_id.py
--rw-r--r--   0        0        0     2432 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_request.py
--rw-r--r--   0        0        0     1814 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_update_request.py
--rw-r--r--   0        0        0       84 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_id.py
--rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_request.py
--rw-r--r--   0        0        0     1224 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_response.py
--rw-r--r--   0        0        0     1446 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/find_counterparties_response.py
--rw-r--r--   0        0        0      633 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/identifier_list.py
--rw-r--r--   0        0        0     1372 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_response.py
--rw-r--r--   0        0        0      974 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_response.py
--rw-r--r--   0        0        0       88 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_id.py
--rw-r--r--   0        0        0     1370 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_request.py
--rw-r--r--   0        0        0     1539 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_response.py
--rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/responsibilities.py
--rw-r--r--   0        0        0      391 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/rule.py
--rw-r--r--   0        0        0      761 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/tax_id.py
--rw-r--r--   0        0        0      573 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/trigger.py
--rw-r--r--   0        0        0      163 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    20834 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      154 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0     6559 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    15332 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     3870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0      907 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/__init__.py
--rw-r--r--   0        0        0     1346 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/__init__.py
--rw-r--r--   0        0        0     1017 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approval_request.py
--rw-r--r--   0        0        0      631 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approver_action.py
--rw-r--r--   0        0        0      905 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/assigned_approver.py
--rw-r--r--   0        0        0      984 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/associated_approval_action.py
--rw-r--r--   0        0        0       81 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_id.py
--rw-r--r--   0        0        0      934 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_request.py
--rw-r--r--   0        0        0     1428 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_response.py
--rw-r--r--   0        0        0      851 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/document_response.py
--rw-r--r--   0        0        0     1409 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_approver_response.py
--rw-r--r--   0        0        0       81 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_id.py
--rw-r--r--   0        0        0     1331 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
--rw-r--r--   0        0        0     1072 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
--rw-r--r--   0        0        0      870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3439 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_request.py
--rw-r--r--   0        0        0     4252 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_status.py
--rw-r--r--   0        0        0      155 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4424 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      189 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      642 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/vendor_network.py
--rw-r--r--   0        0        0      983 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    10870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1151 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      843 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    12375 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0     2501 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/__init__.py
--rw-r--r--   0        0        0     3514 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/__init__.py
--rw-r--r--   0        0        0     1287 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
--rw-r--r--   0        0        0     1466 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
--rw-r--r--   0        0        0     1026 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_request.py
--rw-r--r--   0        0        0     1014 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_type.py
--rw-r--r--   0        0        0     1247 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_request.py
--rw-r--r--   0        0        0     1468 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_response.py
--rw-r--r--   0        0        0      819 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_brand.py
--rw-r--r--   0        0        0      961 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_request.py
--rw-r--r--   0        0        0      935 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_response.py
--rw-r--r--   0        0        0      750 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_type.py
--rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_request.py
--rw-r--r--   0        0        0     1494 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_response.py
--rw-r--r--   0        0        0      967 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_request.py
--rw-r--r--   0        0        0      941 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/currency_code.py
--rw-r--r--   0        0        0     1607 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
--rw-r--r--   0        0        0     2026 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
--rw-r--r--   0        0        0     1040 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     1028 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1613 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
--rw-r--r--   0        0        0     1071 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0       87 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_id.py
--rw-r--r--   0        0        0     1264 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_request.py
--rw-r--r--   0        0        0     1298 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_response.py
--rw-r--r--   0        0        0     1984 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0       93 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
--rw-r--r--   0        0        0     1581 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1693 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
--rw-r--r--   0        0        0     1229 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_type.py
--rw-r--r--   0        0        0      514 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
--rw-r--r--   0        0        0      271 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1138 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1582 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-07-15 18:45:03.417414 mercoa-0.2.2/README.md
+-rw-r--r--   0        0        0      368 2023-07-15 18:45:03.417414 mercoa-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7697 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/py.typed
+-rw-r--r--   0        0        0     7806 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      499 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      469 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-07-15 18:45:03.417414 mercoa-0.2.2/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      523 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    37562 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0      501 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17689 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4109 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    11215 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/notification_policy/__init__.py
+-rw-r--r--   0        0        0    10326 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/notification_policy/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22306 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12767 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0      131 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    15620 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0      122 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/user/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/user/resources/notifications/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity/resources/user/resources/notifications/client.py
+-rw-r--r--   0        0        0     2295 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0     3367 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      849 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1100 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1036 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1067 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     1451 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1509 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0     1013 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      741 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0      914 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1446 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0     1343 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/find_entity_response.py
+-rw-r--r--   0        0        0     1367 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/find_notification_response.py
+-rw-r--r--   0        0        0      633 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0       86 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/notification_id.py
+-rw-r--r--   0        0        0     1051 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/notification_policy_request.py
+-rw-r--r--   0        0        0     1127 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/notification_policy_response.py
+-rw-r--r--   0        0        0     1129 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/notification_response.py
+-rw-r--r--   0        0        0     1945 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/notification_type.py
+-rw-r--r--   0        0        0      974 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      391 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      761 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0      573 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0      163 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    20874 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6559 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15332 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3870 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0      959 2023-07-15 18:45:03.421414 mercoa-0.2.2/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0     1428 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0      631 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0      905 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/assigned_approver.py
+-rw-r--r--   0        0        0      984 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1428 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      851 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1347 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/find_invoice_response.py
+-rw-r--r--   0        0        0     1409 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_approver_response.py
+-rw-r--r--   0        0        0       81 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     1331 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1258 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1072 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      870 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3439 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     4252 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      155 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4424 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      189 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1258 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      642 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/ocr/types/vendor_network.py
+-rw-r--r--   0        0        0      983 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    10870 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1151 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    12375 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2501 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0     3514 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
+-rw-r--r--   0        0        0     1466 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
+-rw-r--r--   0        0        0     1026 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1014 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0     1247 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_base_request.py
+-rw-r--r--   0        0        0     1468 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_base_response.py
+-rw-r--r--   0        0        0      819 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0      961 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0      935 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1258 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_base_request.py
+-rw-r--r--   0        0        0     1494 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_base_response.py
+-rw-r--r--   0        0        0      967 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0      941 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1607 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
+-rw-r--r--   0        0        0     2026 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
+-rw-r--r--   0        0        0     1040 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1028 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1613 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
+-rw-r--r--   0        0        0     1071 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1264 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     1984 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1581 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1693 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1229 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0      271 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1138 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1582 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-07-15 18:45:03.425414 mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.2/PKG-INFO
```

### Comparing `mercoa-0.2.1/README.md` & `mercoa-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/__init__.py` & `mercoa-0.2.2/src/mercoa/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,14 +65,17 @@
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
+    FindEntityResponse,
+    FindInvoiceResponse,
+    FindNotificationResponse,
     FullName,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
     IndividualGovernmentId,
     IndividualProfileRequest,
     IndividualProfileResponse,
@@ -82,14 +85,19 @@
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
     Itin,
+    NotificationId,
+    NotificationPolicyRequest,
+    NotificationPolicyResponse,
+    NotificationResponse,
+    NotificationType,
     OcrResponse,
     OrderDirection,
     OrganizationId,
     OrganizationRequest,
     OrganizationResponse,
     PaymentMethodId,
     PaymentMethodRequest,
@@ -213,14 +221,17 @@
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
+    "FindEntityResponse",
+    "FindInvoiceResponse",
+    "FindNotificationResponse",
     "FullName",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
@@ -231,14 +242,19 @@
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "Itin",
     "MercoaEnvironment",
+    "NotificationId",
+    "NotificationPolicyRequest",
+    "NotificationPolicyResponse",
+    "NotificationResponse",
+    "NotificationType",
     "OcrResponse",
     "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
     "PaymentMethodId",
     "PaymentMethodRequest",
```

### Comparing `mercoa-0.2.1/src/mercoa/client.py` & `mercoa-0.2.2/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.2/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.2/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,26 @@
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
+    FindEntityResponse,
+    FindNotificationResponse,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    NotificationId,
+    NotificationPolicyRequest,
+    NotificationPolicyResponse,
+    NotificationResponse,
+    NotificationType,
     ProfileRequest,
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     Rule,
@@ -73,14 +80,15 @@
     ApproverAction,
     AssignedApprover,
     AssociatedApprovalAction,
     CommentId,
     CommentRequest,
     CommentResponse,
     DocumentResponse,
+    FindInvoiceResponse,
     InvoiceApproverResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
@@ -217,14 +225,17 @@
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
+    "FindEntityResponse",
+    "FindInvoiceResponse",
+    "FindNotificationResponse",
     "FullName",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualGovernmentId",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
@@ -234,14 +245,19 @@
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
     "Itin",
+    "NotificationId",
+    "NotificationPolicyRequest",
+    "NotificationPolicyResponse",
+    "NotificationResponse",
+    "NotificationType",
     "OcrResponse",
     "OrderDirection",
     "OrganizationId",
     "OrganizationRequest",
     "OrganizationResponse",
     "PaymentMethodId",
     "PaymentMethodRequest",
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.2/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.2/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.2/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.2/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,32 +16,35 @@
 from ..commons.errors.unauthorized import Unauthorized
 from ..entity_types.types.entity_add_payees_request import EntityAddPayeesRequest
 from ..entity_types.types.entity_id import EntityId
 from ..entity_types.types.entity_request import EntityRequest
 from ..entity_types.types.entity_response import EntityResponse
 from ..entity_types.types.entity_status import EntityStatus
 from ..entity_types.types.entity_update_request import EntityUpdateRequest
+from ..entity_types.types.find_entity_response import FindEntityResponse
 from .resources.approval_policy.client import ApprovalPolicyClient, AsyncApprovalPolicyClient
 from .resources.counterparty.client import AsyncCounterpartyClient, CounterpartyClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
+from .resources.notification_policy.client import AsyncNotificationPolicyClient, NotificationPolicyClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
 from .resources.user.client import AsyncUserClient, UserClient
 
 
 class EntityClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.user = UserClient(environment=self._environment, token=self._token)
         self.approval_policy = ApprovalPolicyClient(environment=self._environment, token=self._token)
         self.counterparty = CounterpartyClient(environment=self._environment, token=self._token)
         self.invoice = InvoiceClient(environment=self._environment, token=self._token)
+        self.notification_policy = NotificationPolicyClient(environment=self._environment, token=self._token)
         self.payment_method = PaymentMethodClient(environment=self._environment, token=self._token)
         self.representative = RepresentativeClient(environment=self._environment, token=self._token)
-        self.user = UserClient(environment=self._environment, token=self._token)
 
     def get_all(
         self, *, is_payee: typing.Optional[bool] = None, is_payor: typing.Optional[bool] = None
     ) -> typing.List[EntityResponse]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "entities"),
@@ -63,31 +66,47 @@
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+        self,
+        *,
+        foreign_id: typing.Union[typing.Optional[str], typing.List[str]],
+        status: typing.Union[typing.Optional[EntityStatus], typing.List[EntityStatus]],
+        is_payee: typing.Optional[bool] = None,
+        is_payor: typing.Optional[bool] = None,
+        name: typing.Optional[str] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[EntityId] = None,
+    ) -> FindEntityResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-            params={"foreignId": foreign_id, "status": status},
+            params={
+                "foreignId": foreign_id,
+                "status": status,
+                "isPayee": is_payee,
+                "isPayor": is_payor,
+                "name": name,
+                "limit": limit,
+                "startingAfter": starting_after,
+            },
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindEntityResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
@@ -187,29 +206,53 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    def accept_terms_of_service(self, entity_id: EntityId) -> None:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
             timeout=60,
         )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    def initiate_kyb(self, entity_id: EntityId) -> None:
+        _response = httpx.request(
+            "POST",
+            urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/request-kyb"),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
@@ -313,20 +356,21 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncEntityClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.user = AsyncUserClient(environment=self._environment, token=self._token)
         self.approval_policy = AsyncApprovalPolicyClient(environment=self._environment, token=self._token)
         self.counterparty = AsyncCounterpartyClient(environment=self._environment, token=self._token)
         self.invoice = AsyncInvoiceClient(environment=self._environment, token=self._token)
+        self.notification_policy = AsyncNotificationPolicyClient(environment=self._environment, token=self._token)
         self.payment_method = AsyncPaymentMethodClient(environment=self._environment, token=self._token)
         self.representative = AsyncRepresentativeClient(environment=self._environment, token=self._token)
-        self.user = AsyncUserClient(environment=self._environment, token=self._token)
 
     async def get_all(
         self, *, is_payee: typing.Optional[bool] = None, is_payor: typing.Optional[bool] = None
     ) -> typing.List[EntityResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
@@ -349,32 +393,48 @@
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def find(
-        self, *, foreign_id: typing.Optional[str] = None, status: typing.Optional[EntityStatus] = None
-    ) -> typing.List[EntityResponse]:
+        self,
+        *,
+        foreign_id: typing.Union[typing.Optional[str], typing.List[str]],
+        status: typing.Union[typing.Optional[EntityStatus], typing.List[EntityStatus]],
+        is_payee: typing.Optional[bool] = None,
+        is_payor: typing.Optional[bool] = None,
+        name: typing.Optional[str] = None,
+        limit: typing.Optional[int] = None,
+        starting_after: typing.Optional[EntityId] = None,
+    ) -> FindEntityResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "entity"),
-                params={"foreignId": foreign_id, "status": status},
+                params={
+                    "foreignId": foreign_id,
+                    "status": status,
+                    "isPayee": is_payee,
+                    "isPayor": is_payor,
+                    "name": name,
+                    "limit": limit,
+                    "startingAfter": starting_after,
+                },
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[EntityResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindEntityResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
@@ -478,30 +538,55 @@
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def accept_terms_of_service(self, entity_id: EntityId) -> str:
+    async def accept_terms_of_service(self, entity_id: EntityId) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/accept-tos"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
+        if 200 <= _response.status_code < 300:
+            return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
+        if "errorName" in _response_json:
+            if _response_json["errorName"] == "AuthHeaderMissingError":
+                raise AuthHeaderMissingError()
+            if _response_json["errorName"] == "AuthHeaderMalformedError":
+                raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+            if _response_json["errorName"] == "Unauthorized":
+                raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def initiate_kyb(self, entity_id: EntityId) -> None:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "POST",
+                urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/request-kyb"),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
+            return
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
 from ....commons.types.order_direction import OrderDirection
 from ....entity_types.types.entity_id import EntityId
+from ....invoice_types.types.find_invoice_response import FindInvoiceResponse
 from ....invoice_types.types.invoice_id import InvoiceId
 from ....invoice_types.types.invoice_metrics_response import InvoiceMetricsResponse
 from ....invoice_types.types.invoice_order_by_field import InvoiceOrderByField
-from ....invoice_types.types.invoice_response import InvoiceResponse
 from ....invoice_types.types.invoice_status import InvoiceStatus
 from ....payment_method_types.types.currency_code import CurrencyCode
 
 
 class InvoiceClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
@@ -38,15 +38,15 @@
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
+    ) -> FindInvoiceResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
             params={
                 "startDate": serialize_datetime(start_date) if start_date is not None else None,
                 "endDate": serialize_datetime(end_date) if end_date is not None else None,
                 "orderBy": order_by,
@@ -62,15 +62,15 @@
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
@@ -134,15 +134,15 @@
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
+    ) -> FindInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/invoices"),
                 params={
                     "startDate": serialize_datetime(start_date) if start_date is not None else None,
                     "endDate": serialize_datetime(end_date) if end_date is not None else None,
@@ -159,15 +159,15 @@
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.2.2/src/mercoa/resources/entity/resources/user/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
 from ....entity_types.types.entity_id import EntityId
 from ....entity_types.types.entity_user_id import EntityUserId
 from ....entity_types.types.entity_user_request import EntityUserRequest
 from ....entity_types.types.entity_user_response import EntityUserResponse
+from .resources.notifications.client import AsyncNotificationsClient, NotificationsClient
 
 
 class UserClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.notifications = NotificationsClient(environment=self._environment, token=self._token)
 
     def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
@@ -148,14 +150,15 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncUserClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
+        self.notifications = AsyncNotificationsClient(environment=self._environment, token=self._token)
 
     async def get_all(self, entity_id: EntityId) -> typing.List[EntityUserResponse]:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"entity/{entity_id}/users"),
                 headers=remove_none_from_headers(
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,19 +19,26 @@
     EntityResponse,
     EntityStatus,
     EntityUpdateRequest,
     EntityUserId,
     EntityUserRequest,
     EntityUserResponse,
     FindCounterpartiesResponse,
+    FindEntityResponse,
+    FindNotificationResponse,
     IdentifierList,
     IdentifierList_RolesList,
     IdentifierList_UserList,
     IndividualProfileRequest,
     IndividualProfileResponse,
+    NotificationId,
+    NotificationPolicyRequest,
+    NotificationPolicyResponse,
+    NotificationResponse,
+    NotificationType,
     ProfileRequest,
     ProfileResponse,
     RepresentativeId,
     RepresentativeRequest,
     RepresentativeResponse,
     Responsibilities,
     Rule,
@@ -61,19 +68,26 @@
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
+    "FindEntityResponse",
+    "FindNotificationResponse",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "NotificationId",
+    "NotificationPolicyRequest",
+    "NotificationPolicyResponse",
+    "NotificationResponse",
+    "NotificationType",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,17 +18,24 @@
 from .entity_response import EntityResponse
 from .entity_status import EntityStatus
 from .entity_update_request import EntityUpdateRequest
 from .entity_user_id import EntityUserId
 from .entity_user_request import EntityUserRequest
 from .entity_user_response import EntityUserResponse
 from .find_counterparties_response import FindCounterpartiesResponse
+from .find_entity_response import FindEntityResponse
+from .find_notification_response import FindNotificationResponse
 from .identifier_list import IdentifierList, IdentifierList_RolesList, IdentifierList_UserList
 from .individual_profile_request import IndividualProfileRequest
 from .individual_profile_response import IndividualProfileResponse
+from .notification_id import NotificationId
+from .notification_policy_request import NotificationPolicyRequest
+from .notification_policy_response import NotificationPolicyResponse
+from .notification_response import NotificationResponse
+from .notification_type import NotificationType
 from .profile_request import ProfileRequest
 from .profile_response import ProfileResponse
 from .representative_id import RepresentativeId
 from .representative_request import RepresentativeRequest
 from .representative_response import RepresentativeResponse
 from .responsibilities import Responsibilities
 from .rule import Rule, Rule_Approver
@@ -54,19 +61,26 @@
     "EntityResponse",
     "EntityStatus",
     "EntityUpdateRequest",
     "EntityUserId",
     "EntityUserRequest",
     "EntityUserResponse",
     "FindCounterpartiesResponse",
+    "FindEntityResponse",
+    "FindNotificationResponse",
     "IdentifierList",
     "IdentifierList_RolesList",
     "IdentifierList_UserList",
     "IndividualProfileRequest",
     "IndividualProfileResponse",
+    "NotificationId",
+    "NotificationPolicyRequest",
+    "NotificationPolicyResponse",
+    "NotificationResponse",
+    "NotificationType",
     "ProfileRequest",
     "ProfileResponse",
     "RepresentativeId",
     "RepresentativeRequest",
     "RepresentativeResponse",
     "Responsibilities",
     "Rule",
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/amount_trigger.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_update_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approver_rule.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     legal_business_name: str = pydantic.Field(alias="legalBusinessName")
     business_type: typing.Optional[BusinessType] = pydantic.Field(alias="businessType")
     phone: typing.Optional[PhoneNumber]
     doing_business_as: typing.Optional[str] = pydantic.Field(alias="doingBusinessAs")
     website: typing.Optional[str]
     description: typing.Optional[str]
     address: typing.Optional[Address]
-    owners_provided: typing.Optional[bool] = pydantic.Field(alias="ownersProvided")
     tax_id: typing.Optional[TaxId] = pydantic.Field(alias="taxId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     legal_business_name: str = pydantic.Field(alias="legalBusinessName")
     business_type: typing.Optional[BusinessType] = pydantic.Field(alias="businessType")
     phone: typing.Optional[PhoneNumber]
     doing_business_as: typing.Optional[str] = pydantic.Field(alias="doingBusinessAs")
     website: typing.Optional[str]
     description: typing.Optional[str]
     address: typing.Optional[Address]
-    owners_provided: bool = pydantic.Field(alias="ownersProvided")
+    owners_provided: typing.Optional[bool] = pydantic.Field(alias="ownersProvided")
     tax_id_provided: bool = pydantic.Field(alias="taxIDProvided")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_type.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/counterparty_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/ein.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_add_payees_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_add_payees_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_status.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_update_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/find_counterparties_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/identifier_list.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_request.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_response.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/responsibilities.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/tax_id.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/entity_types/types/trigger.py` & `mercoa-0.2.2/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.2/src/mercoa/resources/invoice/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
 from ..commons.types.order_direction import OrderDirection
 from ..entity_types.types.entity_id import EntityId
+from ..invoice_types.types.find_invoice_response import FindInvoiceResponse
 from ..invoice_types.types.invoice_id import InvoiceId
 from ..invoice_types.types.invoice_order_by_field import InvoiceOrderByField
 from ..invoice_types.types.invoice_request import InvoiceRequest
 from ..invoice_types.types.invoice_response import InvoiceResponse
 from ..invoice_types.types.invoice_status import InvoiceStatus
 from .resources.approval.client import ApprovalClient, AsyncApprovalClient
 from .resources.comment.client import AsyncCommentClient, CommentClient
@@ -44,15 +45,15 @@
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
+    ) -> FindInvoiceResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
             params={
                 "entityIds": entity_ids,
                 "startDate": serialize_datetime(start_date) if start_date is not None else None,
                 "endDate": serialize_datetime(end_date) if end_date is not None else None,
@@ -69,15 +70,15 @@
             timeout=60,
         )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
@@ -222,15 +223,15 @@
         end_date: typing.Optional[dt.datetime] = None,
         order_by: typing.Optional[InvoiceOrderByField] = None,
         order_direction: typing.Optional[OrderDirection] = None,
         limit: typing.Optional[int] = None,
         starting_after: typing.Optional[InvoiceId] = None,
         search: typing.Optional[str] = None,
         status: typing.Union[typing.Optional[InvoiceStatus], typing.List[InvoiceStatus]],
-    ) -> typing.List[InvoiceResponse]:
+    ) -> FindInvoiceResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "invoices"),
                 params={
                     "entityIds": entity_ids,
                     "startDate": serialize_datetime(start_date) if start_date is not None else None,
@@ -248,15 +249,15 @@
                 timeout=60,
             )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(typing.List[InvoiceResponse], _response_json)  # type: ignore
+            return pydantic.parse_obj_as(FindInvoiceResponse, _response_json)  # type: ignore
         if "errorName" in _response_json:
             if _response_json["errorName"] == "AuthHeaderMissingError":
                 raise AuthHeaderMissingError()
             if _response_json["errorName"] == "AuthHeaderMalformedError":
                 raise AuthHeaderMalformedError(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
             if _response_json["errorName"] == "Unauthorized":
                 raise Unauthorized(pydantic.parse_obj_as(str, _response_json["content"]))  # type: ignore
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.2.2/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.2.2/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.2.2/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     ApproverAction,
     AssignedApprover,
     AssociatedApprovalAction,
     CommentId,
     CommentRequest,
     CommentResponse,
     DocumentResponse,
+    FindInvoiceResponse,
     InvoiceApproverResponse,
     InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
     InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
@@ -25,14 +26,15 @@
     "ApproverAction",
     "AssignedApprover",
     "AssociatedApprovalAction",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "DocumentResponse",
+    "FindInvoiceResponse",
     "InvoiceApproverResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .approver_action import ApproverAction
 from .assigned_approver import AssignedApprover
 from .associated_approval_action import AssociatedApprovalAction
 from .comment_id import CommentId
 from .comment_request import CommentRequest
 from .comment_response import CommentResponse
 from .document_response import DocumentResponse
+from .find_invoice_response import FindInvoiceResponse
 from .invoice_approver_response import InvoiceApproverResponse
 from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_metrics_response import InvoiceMetricsResponse
 from .invoice_order_by_field import InvoiceOrderByField
 from .invoice_request import InvoiceRequest
@@ -23,14 +24,15 @@
     "ApproverAction",
     "AssignedApprover",
     "AssociatedApprovalAction",
     "CommentId",
     "CommentRequest",
     "CommentResponse",
     "DocumentResponse",
+    "FindInvoiceResponse",
     "InvoiceApproverResponse",
     "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
     "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
```

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approval_request.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approver_action.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/assigned_approver.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/assigned_approver.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/associated_approval_action.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_request.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/document_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_approver_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_approver_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_request.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_response.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_status.py` & `mercoa-0.2.2/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.2/src/mercoa/resources/ocr/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.2/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/ocr/types/vendor_network.py` & `mercoa-0.2.2/src/mercoa/resources/ocr/types/vendor_network.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/client.py` & `mercoa-0.2.2/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.2.2/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_schema/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/__init__.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_account_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_status.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_type.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_brand.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_type.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/check_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/currency_code.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_type.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py` & `mercoa-0.2.2/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/transaction/client.py` & `mercoa-0.2.2/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.2/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.1/PKG-INFO` & `mercoa-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.2.1
+Version: 0.2.2
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

