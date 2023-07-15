# Comparing `tmp/types-stripe-3.5.2.8.tar.gz` & `tmp/types-stripe-3.5.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-stripe-3.5.2.8.tar", last modified: Mon Feb 27 15:18:23 2023, max compression
+gzip compressed data, was "types-stripe-3.5.2.9.tar", last modified: Tue Mar 28 12:33:09 2023, max compression
```

## Comparing `types-stripe-3.5.2.8.tar` & `types-stripe-3.5.2.9.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.223143 types-stripe-3.5.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-27 15:18:21.000000 types-stripe-3.5.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 15:18:21.000000 types-stripe-3.5.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-27 15:18:23.223143 types-stripe-3.5.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 15:18:23.223143 types-stripe-3.5.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-02-27 15:18:21.000000 types-stripe-3.5.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.195143 types-stripe-3.5.2.8/stripe-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-27 15:18:21.000000 types-stripe-3.5.2.8/stripe-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_requestor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.207143 types-stripe-3.5.2.8/stripe-stubs/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.211143 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/createable_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/custom_method.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/deletable_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/listable_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/nested_resource_class_methods.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/searchable_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/singleton_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/updateable_api_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/verify_mixin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/account_link.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/alipay_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/apple_pay_domain.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/application_fee.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/application_fee_refund.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/balance.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/balance_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/bank_account.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.211143 types-stripe-3.5.2.8/stripe-stubs/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/billing_portal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/billing_portal/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/billing_portal/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/bitcoin_receiver.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/bitcoin_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/capability.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/charge.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.211143 types-stripe-3.5.2.8/stripe-stubs/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/checkout/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/checkout/session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/country_spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/coupon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/credit_note.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/credit_note_line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/customer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/customer_balance_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/dispute.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/ephemeral_key.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/error_object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/exchange_rate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/file.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/file_link.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.215143 types-stripe-3.5.2.8/stripe-stubs/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/identity/verification_report.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/identity/verification_session.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/invoice.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/invoice_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/invoice_line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuer_fraud_record.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.215143 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/authorization.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/card_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/cardholder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/dispute.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/issuing/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/list_object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/login_link.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/mandate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/order.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/payment_intent.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/payout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/person.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/plan.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/price.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/promotion_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/quote.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/stripe-stubs/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/radar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/radar/early_fraud_warning.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/radar/value_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/radar/value_list_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/recipient.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/recipient_transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/refund.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/stripe-stubs/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/reporting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/reporting/report_run.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/reporting/report_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/reversal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/review.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/search_result_object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/setup_attempt.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/setup_intent.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/stripe-stubs/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/sigma/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/sigma/scheduled_query_run.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/sku.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/source_transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/subscription.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/subscription_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/subscription_schedule.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/tax_code.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/tax_id.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/tax_rate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/stripe-stubs/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/terminal/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/terminal/connection_token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/terminal/location.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/terminal/reader.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/stripe-stubs/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/test_helpers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/test_helpers/test_clock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/three_d_secure.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/topup.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/transfer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/usage_record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/usage_record_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/api_resources/webhook_endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/http_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/multipart_data_generator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/oauth.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/oauth_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/object_classes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/request_metrics.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/stripe_object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/stripe_response.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-27 15:18:07.000000 types-stripe-3.5.2.8/stripe-stubs/webhook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:18:23.219143 types-stripe-3.5.2.8/types_stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-02-27 15:18:23.000000 types-stripe-3.5.2.8/types_stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-02-27 15:18:23.000000 types-stripe-3.5.2.8/types_stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:18:23.000000 types-stripe-3.5.2.8/types_stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-27 15:18:23.000000 types-stripe-3.5.2.8/types_stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.713198 types-stripe-3.5.2.9/stripe-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/stripe-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_requestor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/createable_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/custom_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/deletable_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/listable_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/nested_resource_class_methods.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/searchable_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/singleton_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/updateable_api_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/verify_mixin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/account_link.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/alipay_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/apple_pay_domain.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/application_fee.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/application_fee_refund.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/balance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/balance_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/bank_account.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/billing_portal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/billing_portal/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/billing_portal/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/bitcoin_receiver.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/bitcoin_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/capability.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/charge.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/checkout/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/checkout/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/country_spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/coupon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/credit_note.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/credit_note_line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/customer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/customer_balance_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/dispute.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/ephemeral_key.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/error_object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/exchange_rate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/file.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/file_link.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/identity/verification_report.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/identity/verification_session.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/invoice.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/invoice_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/invoice_line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuer_fraud_record.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/authorization.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/card_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/cardholder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/dispute.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/issuing/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/list_object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/login_link.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/mandate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/order.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/payment_intent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/payout.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/person.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/plan.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/price.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/promotion_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/quote.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.721198 types-stripe-3.5.2.9/stripe-stubs/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/radar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/radar/early_fraud_warning.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/radar/value_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/radar/value_list_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/recipient.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/recipient_transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/refund.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/stripe-stubs/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/reporting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/reporting/report_run.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/reporting/report_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/reversal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/review.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/search_result_object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/setup_attempt.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/setup_intent.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/stripe-stubs/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/sigma/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/sigma/scheduled_query_run.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/sku.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/source_transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/subscription.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/subscription_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/subscription_schedule.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/tax_code.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/tax_id.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/tax_rate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/stripe-stubs/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/terminal/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/terminal/connection_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/terminal/location.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/terminal/reader.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/stripe-stubs/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/test_helpers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/test_helpers/test_clock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/three_d_secure.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/topup.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/transfer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/usage_record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/usage_record_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/api_resources/webhook_endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/http_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/multipart_data_generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/oauth.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/oauth_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/object_classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/request_metrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/stripe_object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/stripe_response.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-28 12:32:25.000000 types-stripe-3.5.2.9/stripe-stubs/webhook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:09.725198 types-stripe-3.5.2.9/types_stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/types_stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/types_stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/types_stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 12:33:09.000000 types-stripe-3.5.2.9/types_stripe.egg-info/top_level.txt
```

### Comparing `types-stripe-3.5.2.8/CHANGELOG.md` & `types-stripe-3.5.2.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.5.2.9 (2023-03-28)
+
+Add defaults for third-party stubs Q-T (#9959)
+
 ## 3.5.2.8 (2023-02-27)
 
 [stripe] Add Session.expire() (#9814)
 
 ## 3.5.2.7 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-stripe-3.5.2.8/PKG-INFO` & `types-stripe-3.5.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-stripe
-Version: 3.5.2.8
+Version: 3.5.2.9
 Summary: Typing stubs for stripe
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stripe.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `stripe`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/stripe. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b98f7307ba12b86a44a8499bab58ae87e768529`.
+This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
```

### Comparing `types-stripe-3.5.2.8/setup.py` & `types-stripe-3.5.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `stripe`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/stripe. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b98f7307ba12b86a44a8499bab58ae87e768529`.
+This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.5.2.8",
+      version="3.5.2.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stripe.md",
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/__init__.pyi` & `types-stripe-3.5.2.9/stripe-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 app_info: Any
 enable_telemetry: bool
 max_network_retries: int
 ca_bundle_path: Any
 log: Any
 
 def set_app_info(
-    name, partner_id: Incomplete | None = ..., url: Incomplete | None = ..., version: Incomplete | None = ...
+    name, partner_id: Incomplete | None = None, url: Incomplete | None = None, version: Incomplete | None = None
 ) -> None: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_requestor.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_requestor.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -8,26 +8,31 @@
 class APIRequestor:
     api_base: Any
     api_key: Any
     api_version: Any
     stripe_account: Any
     def __init__(
         self,
-        key: Incomplete | None = ...,
-        client: Incomplete | None = ...,
-        api_base: Incomplete | None = ...,
-        api_version: Incomplete | None = ...,
-        account: Incomplete | None = ...,
+        key: Incomplete | None = None,
+        client: Incomplete | None = None,
+        api_base: Incomplete | None = None,
+        api_version: Incomplete | None = None,
+        account: Incomplete | None = None,
     ) -> None: ...
     @classmethod
     def format_app_info(cls, info): ...
-    def request(self, method, url, params: Incomplete | None = ..., headers: Incomplete | None = ...): ...
-    def request_stream(self, method, url, params: Incomplete | None = ..., headers: Incomplete | None = ...): ...
+    def request(self, method, url, params: Incomplete | None = None, headers: Incomplete | None = None): ...
+    def request_stream(self, method, url, params: Incomplete | None = None, headers: Incomplete | None = None): ...
     def handle_error_response(self, rbody, rcode, resp, rheaders) -> None: ...
     def specific_api_error(self, rbody, rcode, resp, rheaders, error_data): ...
     def specific_oauth_error(self, rbody, rcode, resp, rheaders, error_code): ...
     def request_headers(self, api_key, method): ...
     def request_raw(
-        self, method, url, params: Incomplete | None = ..., supplied_headers: Incomplete | None = ..., is_streaming: bool = ...
+        self,
+        method,
+        url,
+        params: Incomplete | None = None,
+        supplied_headers: Incomplete | None = None,
+        is_streaming: bool = False,
     ): ...
     def interpret_response(self, rbody, rcode, rheaders): ...
     def interpret_streaming_response(self, stream, rcode, rheaders): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/__init__.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/__init__.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/abstract/listable_api_resource.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/abstract/listable_api_resource.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 
 class ListableAPIResource(APIResource):
     @classmethod
     def auto_paging_iter(cls, *args, **params) -> Iterator[Any]: ...
     @classmethod
     def list(
         cls,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ) -> ListObject: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/account.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/customer.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,58 @@
-from _typeshed import Incomplete
-
-from stripe import oauth as oauth
+from stripe import api_requestor as api_requestor
 from stripe.api_resources.abstract import (
     CreateableAPIResource as CreateableAPIResource,
     DeletableAPIResource as DeletableAPIResource,
     ListableAPIResource as ListableAPIResource,
+    SearchableAPIResource as SearchableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
     nested_resource_class_methods as nested_resource_class_methods,
 )
 
-class Account(CreateableAPIResource, DeletableAPIResource, ListableAPIResource):
+class Customer(CreateableAPIResource, DeletableAPIResource, ListableAPIResource, SearchableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def reject(self, idempotency_key: str | None = ..., **params): ...
-    @classmethod
-    def retrieve(cls, id: Incomplete | None = ..., api_key: Incomplete | None = ..., **params): ...
+    def delete_discount(self, **params) -> None: ...
     @classmethod
-    def modify(cls, id: Incomplete | None = ..., **params): ...
-    def instance_url(self): ...
-    def persons(self, idempotency_key: str | None = ..., **params): ...
-    def deauthorize(self, **params): ...
-    def serialize(self, previous): ...
+    def balance_transactions_url(cls, id, nested_id=None): ...
     @classmethod
-    def capabilitys_url(cls, id, nested_id=...): ...
-    @classmethod
-    def capabilitys_request(
-        cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params
+    def balance_transactions_request(
+        cls, method, url, api_key=None, idempotency_key=None, stripe_version=None, stripe_account=None, **params
     ): ...
     @classmethod
-    def retrieve_capability(cls, id, nested_id, **params): ...
+    def create_balance_transaction(cls, id, **params): ...
+    @classmethod
+    def retrieve_balance_transaction(cls, id, nested_id, **params): ...
     @classmethod
-    def modify_capability(cls, id, nested_id, **params): ...
+    def modify_balance_transaction(cls, id, nested_id, **params): ...
     @classmethod
-    def list_capabilities(cls, id, **params): ...
+    def list_balance_transactions(cls, id, **params): ...
     @classmethod
-    def external_accounts_url(cls, id, nested_id=...): ...
+    def sources_url(cls, id, nested_id=None): ...
     @classmethod
-    def external_accounts_request(
-        cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params
+    def sources_request(
+        cls, method, url, api_key=None, idempotency_key=None, stripe_version=None, stripe_account=None, **params
     ): ...
     @classmethod
-    def create_external_account(cls, id, **params): ...
+    def create_source(cls, id, **params): ...
     @classmethod
-    def retrieve_external_account(cls, id, nested_id, **params): ...
+    def retrieve_source(cls, id, nested_id, **params): ...
     @classmethod
-    def modify_external_account(cls, id, nested_id, **params): ...
+    def modify_source(cls, id, nested_id, **params): ...
     @classmethod
-    def delete_external_account(cls, id, nested_id, **params): ...
+    def delete_source(cls, id, nested_id, **params): ...
     @classmethod
-    def list_external_accounts(cls, id, **params): ...
+    def list_sources(cls, id, **params): ...
     @classmethod
-    def login_links_url(cls, id, nested_id=...): ...
+    def tax_ids_url(cls, id, nested_id=None): ...
     @classmethod
-    def login_links_request(
-        cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params
+    def tax_ids_request(
+        cls, method, url, api_key=None, idempotency_key=None, stripe_version=None, stripe_account=None, **params
     ): ...
     @classmethod
-    def create_login_link(cls, id, **params): ...
-    @classmethod
-    def persons_url(cls, id, nested_id=...): ...
-    @classmethod
-    def persons_request(cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params): ...
-    @classmethod
-    def create_person(cls, id, **params): ...
-    @classmethod
-    def retrieve_person(cls, id, nested_id, **params): ...
+    def create_tax_id(cls, id, **params): ...
     @classmethod
-    def modify_person(cls, id, nested_id, **params): ...
+    def retrieve_tax_id(cls, id, nested_id, **params): ...
     @classmethod
-    def delete_person(cls, id, nested_id, **params): ...
+    def delete_tax_id(cls, id, nested_id, **params): ...
     @classmethod
-    def list_persons(cls, id, **params): ...
+    def list_tax_ids(cls, id, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/alipay_account.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/alipay_account.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -12,12 +12,12 @@
     def instance_url(self): ...
     @classmethod
     def modify(cls, customer, id, **params): ...
     @classmethod
     def retrieve(
         cls,
         id,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ) -> NoReturn: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/application_fee_refund.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/application_fee_refund.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 class ApplicationFeeRefund(UpdateableAPIResource):
     OBJECT_NAME: str
     @classmethod
     def modify(cls, fee, sid: str, **params) -> Self: ...  # type: ignore[override]
     def instance_url(self) -> str: ...
     @classmethod
-    def retrieve(cls, id, api_key: Incomplete | None = ..., **params) -> NoReturn: ...
+    def retrieve(cls, id, api_key: Incomplete | None = None, **params) -> NoReturn: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/bank_account.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/bank_account.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     def instance_url(self) -> str: ...
     @classmethod
     def modify(cls, sid, **params) -> NoReturn: ...
     @classmethod
     def retrieve(
         cls,
         id,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ) -> NoReturn: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/card.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/card.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     def instance_url(self) -> str: ...
     @classmethod
     def modify(cls, sid, **params) -> NoReturn: ...
     @classmethod
     def retrieve(
         cls,
         id,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ) -> NoReturn: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/charge.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/charge.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -5,13 +5,13 @@
     SearchableAPIResource as SearchableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class Charge(CreateableAPIResource, ListableAPIResource, SearchableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def capture(self, idempotency_key: str | None = ..., **params): ...
-    def refund(self, idempotency_key: str | None = ..., **params): ...
-    def update_dispute(self, idempotency_key: str | None = ..., **params): ...
-    def close_dispute(self, idempotency_key: str | None = ..., **params): ...
-    def mark_as_fraudulent(self, idempotency_key: str | None = ...): ...
-    def mark_as_safe(self, idempotency_key: str | None = ...): ...
+    def capture(self, idempotency_key: str | None = None, **params): ...
+    def refund(self, idempotency_key: str | None = None, **params): ...
+    def update_dispute(self, idempotency_key: str | None = None, **params): ...
+    def close_dispute(self, idempotency_key: str | None = None, **params): ...
+    def mark_as_fraudulent(self, idempotency_key: str | None = None): ...
+    def mark_as_safe(self, idempotency_key: str | None = None): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/checkout/session.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/checkout/session.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 class Session(CreateableAPIResource, ListableAPIResource):
     OBJECT_NAME: str
     @overload
     @classmethod
     def expire(cls, session, api_key=None, stripe_version=None, stripe_account=None, **params): ...
     @overload
     @classmethod
-    def expire(cls, idempotency_key: str | None = ..., **params): ...
+    def expire(cls, idempotency_key: str | None = None, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/credit_note.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/credit_note.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     ListableAPIResource as ListableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class CreditNote(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def void_credit_note(self, idempotency_key: str | None = ..., **params): ...
+    def void_credit_note(self, idempotency_key: str | None = None, **params): ...
     @classmethod
     def preview(
         cls,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/error_object.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/list_object.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,57 @@
 from _typeshed import Incomplete
+from collections.abc import Iterator
+from typing import Any
 
+from stripe import api_requestor as api_requestor
 from stripe.stripe_object import StripeObject as StripeObject
 
-class ErrorObject(StripeObject):
-    def refresh_from(
+class ListObject(StripeObject):
+    OBJECT_NAME: str
+    def list(
         self,
-        values,
-        api_key: Incomplete | None = ...,
-        partial: bool = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        last_response: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        **params,
+    ) -> ListObject: ...
+    def create(
+        self,
+        api_key: Incomplete | None = None,
+        idempotency_key: str | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        **params,
     ): ...
-
-class OAuthErrorObject(StripeObject):
-    def refresh_from(
+    def retrieve(
         self,
-        values,
-        api_key: Incomplete | None = ...,
-        partial: bool = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        last_response: Incomplete | None = ...,
+        id,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        **params,
     ): ...
+    def __getitem__(self, k): ...
+    def __iter__(self): ...
+    def __len__(self) -> int: ...
+    def __reversed__(self): ...
+    def auto_paging_iter(self) -> Iterator[Any]: ...
+    @classmethod
+    def empty_list(
+        cls, api_key: Incomplete | None = None, stripe_version: Incomplete | None = None, stripe_account: Incomplete | None = None
+    ) -> ListObject: ...
+    @property
+    def is_empty(self) -> bool: ...
+    def next_page(
+        self,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        **params,
+    ) -> ListObject: ...
+    def previous_page(
+        self,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        **params,
+    ) -> ListObject: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/file.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/file.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     OBJECT_NAME: str
     OBJECT_NAME_ALT: str
     @classmethod
     def class_url(cls): ...
     @classmethod
     def create(
         cls,
-        api_key: Incomplete | None = ...,
-        api_version: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        api_version: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ): ...
 
 FileUpload = File
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/invoice.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/invoice.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     SearchableAPIResource as SearchableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class Invoice(CreateableAPIResource, DeletableAPIResource, ListableAPIResource, SearchableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def finalize_invoice(self, idempotency_key: str | None = ..., **params) -> Self: ...
-    def mark_uncollectible(self, idempotency_key: str | None = ..., **params) -> Self: ...
-    def pay(self, idempotency_key: str | None = ..., **params) -> Self: ...
-    def send_invoice(self, idempotency_key: str | None = ..., **params) -> Self: ...
-    def void_invoice(self, idempotency_key: str | None = ..., **params) -> Self: ...
+    def finalize_invoice(self, idempotency_key: str | None = None, **params) -> Self: ...
+    def mark_uncollectible(self, idempotency_key: str | None = None, **params) -> Self: ...
+    def pay(self, idempotency_key: str | None = None, **params) -> Self: ...
+    def send_invoice(self, idempotency_key: str | None = None, **params) -> Self: ...
+    def void_invoice(self, idempotency_key: str | None = None, **params) -> Self: ...
     @classmethod
     def upcoming(
         cls,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ) -> Invoice: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/list_object.pyi` & `types-stripe-3.5.2.9/stripe-stubs/error.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,76 @@
 from _typeshed import Incomplete
-from collections.abc import Iterator
 from typing import Any
 
-from stripe import api_requestor as api_requestor
-from stripe.stripe_object import StripeObject as StripeObject
-
-class ListObject(StripeObject):
-    OBJECT_NAME: str
-    def list(
-        self,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        **params,
-    ) -> ListObject: ...
-    def create(
-        self,
-        api_key: Incomplete | None = ...,
-        idempotency_key: str | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        **params,
-    ): ...
-    def retrieve(
+class StripeError(Exception):
+    http_body: Any
+    http_status: Any
+    json_body: Any
+    headers: Any
+    code: Any
+    request_id: Any
+    error: Any
+    def __init__(
         self,
-        id,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        **params,
-    ): ...
-    def __getitem__(self, k): ...
-    def __iter__(self): ...
-    def __len__(self) -> int: ...
-    def __reversed__(self): ...
-    def auto_paging_iter(self) -> Iterator[Any]: ...
-    @classmethod
-    def empty_list(
-        cls, api_key: Incomplete | None = ..., stripe_version: Incomplete | None = ..., stripe_account: Incomplete | None = ...
-    ) -> ListObject: ...
+        message: Incomplete | None = None,
+        http_body: Incomplete | None = None,
+        http_status: Incomplete | None = None,
+        json_body: Incomplete | None = None,
+        headers: Incomplete | None = None,
+        code: Incomplete | None = None,
+    ) -> None: ...
     @property
-    def is_empty(self) -> bool: ...
-    def next_page(
+    def user_message(self): ...
+    def construct_error_object(self): ...
+
+class APIError(StripeError): ...
+
+class APIConnectionError(StripeError):
+    should_retry: Any
+    def __init__(
+        self,
+        message,
+        http_body: Incomplete | None = None,
+        http_status: Incomplete | None = None,
+        json_body: Incomplete | None = None,
+        headers: Incomplete | None = None,
+        code: Incomplete | None = None,
+        should_retry: bool = False,
+    ) -> None: ...
+
+class StripeErrorWithParamCode(StripeError): ...
+
+class CardError(StripeErrorWithParamCode):
+    param: Any
+    def __init__(
         self,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        **params,
-    ) -> ListObject: ...
-    def previous_page(
+        message,
+        param,
+        code,
+        http_body: Incomplete | None = None,
+        http_status: Incomplete | None = None,
+        json_body: Incomplete | None = None,
+        headers: Incomplete | None = None,
+    ) -> None: ...
+
+class IdempotencyError(StripeError): ...
+
+class InvalidRequestError(StripeErrorWithParamCode):
+    param: Any
+    def __init__(
         self,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        **params,
-    ) -> ListObject: ...
+        message,
+        param,
+        code: Incomplete | None = None,
+        http_body: Incomplete | None = None,
+        http_status: Incomplete | None = None,
+        json_body: Incomplete | None = None,
+        headers: Incomplete | None = None,
+    ) -> None: ...
+
+class AuthenticationError(StripeError): ...
+class PermissionError(StripeError): ...
+class RateLimitError(StripeError): ...
+
+class SignatureVerificationError(StripeError):
+    sig_header: Any
+    def __init__(self, message, sig_header, http_body: Incomplete | None = None) -> None: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/order.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/order.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -3,11 +3,11 @@
     ListableAPIResource as ListableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class Order(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def cancel(self, idempotency_key: str | None = ..., **params): ...
-    def list_line_items(self, idempotency_key: str | None = ..., **params): ...
-    def reopen(self, idempotency_key: str | None = ..., **params): ...
-    def submit(self, idempotency_key: str | None = ..., **params): ...
+    def cancel(self, idempotency_key: str | None = None, **params): ...
+    def list_line_items(self, idempotency_key: str | None = None, **params): ...
+    def reopen(self, idempotency_key: str | None = None, **params): ...
+    def submit(self, idempotency_key: str | None = None, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/payment_intent.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/payment_intent.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -6,17 +6,17 @@
     SearchableAPIResource as SearchableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class PaymentIntent(CreateableAPIResource, ListableAPIResource, SearchableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def cancel(self, idempotency_key: str | None = ..., **params): ...
-    def capture(self, idempotency_key: str | None = ..., **params): ...
+    def cancel(self, idempotency_key: str | None = None, **params): ...
+    def capture(self, idempotency_key: str | None = None, **params): ...
     @overload
     @classmethod
     def confirm(
         cls, intent: str, api_key: str | None = ..., stripe_version: str | None = ..., stripe_account: str | None = ..., **params
     ): ...
     @overload
     @classmethod
-    def confirm(cls, idempotency_key: str | None = ..., **params): ...
+    def confirm(cls, idempotency_key: str | None = None, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/payment_method.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/payment_method.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     ListableAPIResource as ListableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class PaymentMethod(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def attach(self, idempotency_key: str | None = ..., **params) -> Self: ...
-    def detach(self, idempotency_key: str | None = ..., **params) -> Self: ...
+    def attach(self, idempotency_key: str | None = None, **params) -> Self: ...
+    def detach(self, idempotency_key: str | None = None, **params) -> Self: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/quote.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/quote.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     ListableAPIResource as ListableAPIResource,
     UpdateableAPIResource as UpdateableAPIResource,
     custom_method as custom_method,
 )
 
 class Quote(CreateableAPIResource, ListableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
-    def accept(self, idempotency_key: str | None = ..., **params): ...
-    def cancel(self, idempotency_key: str | None = ..., **params): ...
-    def finalize_quote(self, idempotency_key: str | None = ..., **params): ...
-    def list_line_items(self, idempotency_key: str | None = ..., **params): ...
+    def accept(self, idempotency_key: str | None = None, **params): ...
+    def cancel(self, idempotency_key: str | None = None, **params): ...
+    def finalize_quote(self, idempotency_key: str | None = None, **params): ...
+    def list_line_items(self, idempotency_key: str | None = None, **params): ...
     def pdf(
         self,
-        api_key: Incomplete | None = ...,
-        api_version: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        api_version: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
         **params,
     ): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/source.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/source.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -5,9 +5,9 @@
     UpdateableAPIResource as UpdateableAPIResource,
     VerifyMixin as VerifyMixin,
     nested_resource_class_methods as nested_resource_class_methods,
 )
 
 class Source(CreateableAPIResource, UpdateableAPIResource, VerifyMixin):
     OBJECT_NAME: str
-    def detach(self, idempotency_key: str | None = ..., **params): ...
+    def detach(self, idempotency_key: str | None = None, **params): ...
     def source_transactions(self, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/subscription.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/subscription.pyi`

 * *Files identical despite different names*

### Comparing `types-stripe-3.5.2.8/stripe-stubs/api_resources/subscription_item.pyi` & `types-stripe-3.5.2.9/stripe-stubs/api_resources/subscription_item.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,22 @@
     nested_resource_class_methods as nested_resource_class_methods,
 )
 
 class SubscriptionItem(CreateableAPIResource, DeletableAPIResource, ListableAPIResource, UpdateableAPIResource):
     OBJECT_NAME: str
     def usage_record_summaries(self, **params): ...
     @classmethod
-    def usage_records_url(cls, id, nested_id=...): ...
+    def usage_records_url(cls, id, nested_id=None): ...
     @classmethod
     def usage_records_request(
-        cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params
+        cls, method, url, api_key=None, idempotency_key=None, stripe_version=None, stripe_account=None, **params
     ): ...
     @classmethod
     def create_usage_record(cls, id, **params): ...
     @classmethod
-    def usage_record_summarys_url(cls, id, nested_id=...): ...
+    def usage_record_summarys_url(cls, id, nested_id=None): ...
     @classmethod
     def usage_record_summarys_request(
-        cls, method, url, api_key=..., idempotency_key=..., stripe_version=..., stripe_account=..., **params
+        cls, method, url, api_key=None, idempotency_key=None, stripe_version=None, stripe_account=None, **params
     ): ...
     @classmethod
     def list_usage_record_summaries(cls, id, **params): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/http_client.pyi` & `types-stripe-3.5.2.9/stripe-stubs/http_client.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 
 def new_default_http_client(*args, **kwargs): ...
 
 class HTTPClient:
     MAX_DELAY: int
     INITIAL_DELAY: float
     MAX_RETRY_AFTER: int
-    def __init__(self, verify_ssl_certs: bool = ..., proxy: Incomplete | None = ...) -> None: ...
-    def request_with_retries(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request_stream_with_retries(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request(self, method, url, headers, post_data: Incomplete | None = ...) -> None: ...
-    def request_stream(self, method, url, headers, post_data: Incomplete | None = ...) -> None: ...
+    def __init__(self, verify_ssl_certs: bool = True, proxy: Incomplete | None = None) -> None: ...
+    def request_with_retries(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request_stream_with_retries(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request(self, method, url, headers, post_data: Incomplete | None = None) -> None: ...
+    def request_stream(self, method, url, headers, post_data: Incomplete | None = None) -> None: ...
     def close(self) -> None: ...
 
 class RequestsClient(HTTPClient):
     name: str
-    def __init__(self, timeout: int = ..., session: Incomplete | None = ..., **kwargs) -> None: ...
-    def request(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request_stream(self, method, url, headers, post_data: Incomplete | None = ...): ...
+    def __init__(self, timeout: int = 80, session: Incomplete | None = None, **kwargs) -> None: ...
+    def request(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request_stream(self, method, url, headers, post_data: Incomplete | None = None): ...
     def close(self) -> None: ...
 
 class UrlFetchClient(HTTPClient):
     name: str
-    def __init__(self, verify_ssl_certs: bool = ..., proxy: Incomplete | None = ..., deadline: int = ...) -> None: ...
-    def request(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request_stream(self, method, url, headers, post_data: Incomplete | None = ...): ...
+    def __init__(self, verify_ssl_certs: bool = True, proxy: Incomplete | None = None, deadline: int = 55) -> None: ...
+    def request(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request_stream(self, method, url, headers, post_data: Incomplete | None = None): ...
     def close(self) -> None: ...
 
 class PycurlClient(HTTPClient):
     name: str
-    def __init__(self, verify_ssl_certs: bool = ..., proxy: Incomplete | None = ...) -> None: ...
+    def __init__(self, verify_ssl_certs: bool = True, proxy: Incomplete | None = None) -> None: ...
     def parse_headers(self, data): ...
-    def request(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request_stream(self, method, url, headers, post_data: Incomplete | None = ...): ...
+    def request(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request_stream(self, method, url, headers, post_data: Incomplete | None = None): ...
     def close(self) -> None: ...
 
 class Urllib2Client(HTTPClient):
     name: str
-    def __init__(self, verify_ssl_certs: bool = ..., proxy: Incomplete | None = ...) -> None: ...
-    def request(self, method, url, headers, post_data: Incomplete | None = ...): ...
-    def request_stream(self, method, url, headers, post_data: Incomplete | None = ...): ...
+    def __init__(self, verify_ssl_certs: bool = True, proxy: Incomplete | None = None) -> None: ...
+    def request(self, method, url, headers, post_data: Incomplete | None = None): ...
+    def request_stream(self, method, url, headers, post_data: Incomplete | None = None): ...
     def close(self) -> None: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/oauth_error.pyi` & `types-stripe-3.5.2.9/stripe-stubs/oauth_error.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from stripe.error import StripeError as StripeError
 
 class OAuthError(StripeError):
     def __init__(
         self,
         code,
         description,
-        http_body: Incomplete | None = ...,
-        http_status: Incomplete | None = ...,
-        json_body: Incomplete | None = ...,
-        headers: Incomplete | None = ...,
+        http_body: Incomplete | None = None,
+        http_status: Incomplete | None = None,
+        json_body: Incomplete | None = None,
+        headers: Incomplete | None = None,
     ) -> None: ...
     def construct_error_object(self): ...
 
 class InvalidClientError(OAuthError): ...
 class InvalidGrantError(OAuthError): ...
 class InvalidRequestError(OAuthError): ...
 class InvalidScopeError(OAuthError): ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/stripe_object.pyi` & `types-stripe-3.5.2.9/stripe-stubs/stripe_object.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 class StripeObject(dict[Any, Any]):
     class ReprJSONEncoder(json.JSONEncoder):
         def default(self, obj): ...
 
     def __init__(
         self,
-        id: Incomplete | None = ...,
-        api_key: Incomplete | None = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        last_response: Incomplete | None = ...,
+        id: Incomplete | None = None,
+        api_key: Incomplete | None = None,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        last_response: Incomplete | None = None,
         **params,
     ) -> None: ...
     @property
     def last_response(self): ...
     def update(self, update_dict): ...
     def __setattr__(self, k: str, v) -> None: ...
     def __getattr__(self, k: str): ...
@@ -29,34 +29,34 @@
     def __delitem__(self, k) -> None: ...
     def __reduce__(self): ...
     @classmethod
     def construct_from(
         cls,
         values: Any,
         key: str | None,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        last_response: Incomplete | None = ...,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        last_response: Incomplete | None = None,
     ) -> Self: ...
     api_key: Any
     stripe_version: Any
     stripe_account: Any
     def refresh_from(
         self,
         values: Any,
-        api_key: Incomplete | None = ...,
-        partial: bool = ...,
-        stripe_version: Incomplete | None = ...,
-        stripe_account: Incomplete | None = ...,
-        last_response: Incomplete | None = ...,
+        api_key: Incomplete | None = None,
+        partial: bool = False,
+        stripe_version: Incomplete | None = None,
+        stripe_account: Incomplete | None = None,
+        last_response: Incomplete | None = None,
     ) -> None: ...
     @classmethod
     def api_base(cls) -> None: ...
-    def request(self, method, url, params: Incomplete | None = ..., headers: Incomplete | None = ...): ...
-    def request_stream(self, method, url, params: Incomplete | None = ..., headers: Incomplete | None = ...): ...
+    def request(self, method, url, params: Incomplete | None = None, headers: Incomplete | None = None): ...
+    def request_stream(self, method, url, params: Incomplete | None = None, headers: Incomplete | None = None): ...
     def to_dict(self): ...
     def to_dict_recursive(self): ...
     @property
     def stripe_id(self): ...
     def serialize(self, previous): ...
     def __copy__(self) -> StripeObject: ...
     def __deepcopy__(self, memo: Any) -> StripeObject: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/util.pyi` & `types-stripe-3.5.2.9/stripe-stubs/util.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 def logfmt(props): ...
 
 class class_method_variant:
     class_method_name: Any
     def __init__(self, class_method_name) -> None: ...
     method: Any
     def __call__(self, method): ...
-    def __get__(self, obj, objtype: Incomplete | None = ...): ...
+    def __get__(self, obj, objtype: Incomplete | None = None): ...
 
 @overload
 def populate_headers(idempotency_key: None) -> None: ...
 @overload
 def populate_headers(idempotency_key: str) -> dict[str, str]: ...
 
 _RespType: TypeAlias = dict[Any, Any] | StripeObject | StripeResponse
 
 # undocumented
 @overload
 def convert_to_stripe_object(
     resp: list[Any],
-    api_key: Incomplete | None = ...,
-    stripe_version: Incomplete | None = ...,
-    stripe_account: Incomplete | None = ...,
+    api_key: Incomplete | None = None,
+    stripe_version: Incomplete | None = None,
+    stripe_account: Incomplete | None = None,
 ) -> list[Any]: ...
 @overload
 def convert_to_stripe_object(
     resp: _RespType,
-    api_key: Incomplete | None = ...,
-    stripe_version: Incomplete | None = ...,
-    stripe_account: Incomplete | None = ...,
+    api_key: Incomplete | None = None,
+    stripe_version: Incomplete | None = None,
+    stripe_account: Incomplete | None = None,
 ) -> StripeObject: ...
```

### Comparing `types-stripe-3.5.2.8/stripe-stubs/webhook.pyi` & `types-stripe-3.5.2.9/stripe-stubs/webhook.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from stripe import Event, error as error
 
 class Webhook:
     DEFAULT_TOLERANCE: int
     @staticmethod
     def construct_event(
-        payload: bytes | str, sig_header: str, secret: str, tolerance: int = ..., api_key: str | None = ...
+        payload: bytes | str, sig_header: str, secret: str, tolerance: int = 300, api_key: str | None = None
     ) -> Event: ...
 
 class WebhookSignature:
     EXPECTED_SCHEME: str
     @classmethod
-    def verify_header(cls, payload: bytes | str, header: str, secret: str, tolerance: int | None = ...) -> Literal[True]: ...
+    def verify_header(cls, payload: bytes | str, header: str, secret: str, tolerance: int | None = None) -> Literal[True]: ...
     @staticmethod
     def _compute_signature(payload: str, secret: str) -> str: ...
```

### Comparing `types-stripe-3.5.2.8/types_stripe.egg-info/PKG-INFO` & `types-stripe-3.5.2.9/types_stripe.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-stripe
-Version: 3.5.2.8
+Version: 3.5.2.9
 Summary: Typing stubs for stripe
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stripe.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `stripe`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/stripe. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b98f7307ba12b86a44a8499bab58ae87e768529`.
+This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
```

### Comparing `types-stripe-3.5.2.8/types_stripe.egg-info/SOURCES.txt` & `types-stripe-3.5.2.9/types_stripe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

