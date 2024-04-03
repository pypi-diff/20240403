# Comparing `tmp/postfinancecheckout-4.2.0.tar.gz` & `tmp/postfinancecheckout-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancecheckout-4.2.0.tar", last modified: Thu Jan 25 14:59:51 2024, max compression
+gzip compressed data, was "postfinancecheckout-5.0.0.tar", last modified: Wed Apr  3 17:09:53 2024, max compression
```

## Comparing `postfinancecheckout-4.2.0.tar` & `postfinancecheckout-5.0.0.tar`

### file list

```diff
@@ -1,422 +1,423 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.072661 postfinancecheckout-4.2.0/postfinancecheckout/
--rw-r--r--   0 runner    (1001) docker     (127)    34382 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.084661 postfinancecheckout-4.2.0/postfinancecheckout/api/
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23816 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/analytics_query_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22675 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/application_user_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/bank_account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/card_processing_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/charge_attempt_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/charge_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_level_payment_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_level_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31007 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/condition_type_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/country_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/country_state_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/currency_bank_account_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/currency_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29549 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/customer_address_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    33478 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/customer_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/customer_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/delivery_indication_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/document_template_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/document_template_type_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/external_transfer_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26260 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/human_user_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/internal_transfer_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23004 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reconciliation_record_invoice_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25169 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reconciliation_record_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22210 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reimbursement_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/label_description_group_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/label_description_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/language_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/legal_organization_form_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/manual_task_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_connector_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_connector_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_link_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_brand_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_processor_configuration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_processor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_till_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_transaction_summary_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/permission_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/refund_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28785 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/refund_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/refund_recovery_bank_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34776 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/refund_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_recurring_order_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscriber_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_product_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31281 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_suspension_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22307 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/space_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/static_value_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46905 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/token_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/token_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28993 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_completion_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_iframe_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29124 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_invoice_comment_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    40575 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_invoice_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_lightbox_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17314 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_line_item_version_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_mobile_sdk_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_payment_page_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    80373 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_terminal_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_void_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/user_account_role_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/user_space_role_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/web_app_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_encryption_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_listener_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_url_service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26113 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/encryption_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/postfinancecheckout/models/
--rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_account_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_application_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_address_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_human_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_payment_link_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_refund_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)    16919 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_shopify_subscription_product_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_space_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_invoice_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)    20178 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_pending.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_webhook_listener_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_webhook_url_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/account_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/account_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/account_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19096 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/address_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query_execution_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query_result_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_schema_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_schema_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/application_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_create_with_mac_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/authenticated_card_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/authenticated_card_data_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    15797 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_flow_direction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/card_authentication_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/card_authentication_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/card_cryptogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/card_cryptogram_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/card_cryptogram_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/cardholder_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/cardholder_authentication_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)    21380 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_attempt_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_attempt_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_payment_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/charge_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/client_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/client_error_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/completion_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/completion_line_item_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/condition_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/connector_invocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/connector_invocation_stage.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/creation_entity_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/criteria_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/currency_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_postal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customer_postal_address_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/customers_presence.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/data_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/delivery_indication.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/delivery_indication_decision_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/delivery_indication_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/document_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/document_template_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/document_template_type_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_export_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_filter_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_order_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_order_by_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/external_transfer_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/failure_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/failure_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/feature_category.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/gender.py
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/human_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/human_user_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/human_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/internal_transfer_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_invoice_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_rejection_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reimbursement.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reimbursement_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reimbursement_with_refund_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/legal_organization_form.py
--rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_attribute_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_reduction_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/localized_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_action_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/one_click_payment_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_adjustment_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)    16324 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_contract_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_contract_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_information_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_information_hash_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_initiation_advice_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_initiation_advice_file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    20275 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_address_handling_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_protection_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_primary_risk_taker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_processor_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration_version_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_dcc_transaction_sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location_version_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_receipt_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_sum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_summary_fetch_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/recurring_indicator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24283 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_recovery_bank_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/refund_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_terminal_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_terminal_transaction_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/resource_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/resource_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_address_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_address_format_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_country.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_country_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/rest_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/role_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/sales_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/server_error.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_additional_line_item_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_integration_payment_app_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_integration_subscription_app_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_recurring_order.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_recurring_order_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_recurring_order_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_address_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_billing_interval_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_creation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_billing_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_tax_line.py
--rw-r--r--   0 runner    (1001) docker     (127)    27878 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_pricing_option.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension_initiator.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_update_addresses_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    24539 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version_item_price_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_weekday.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_tax_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space_address_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/space_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/static_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tax_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tenant_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/terminal_receipt_fetch_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/terminal_receipt_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    19146 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token_version_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/token_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tokenization_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tokenized_card_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/tokenized_card_data_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    63417 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_aware_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    24689 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_environment_selection_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_group_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_replacement.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_line_item_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_line_item_version_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_line_item_version_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_pending.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_user_interface_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_void.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_void_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_void_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/two_factor_authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/user_account_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/user_space_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/wallet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/web_app_confirmation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/web_app_confirmation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_encryption_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/postfinancecheckout/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-01-25 14:59:51.000000 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22272 2024-01-25 14:59:51.000000 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 14:59:51.000000 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-01-25 14:59:51.000000 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-25 14:59:51.000000 postfinancecheckout-4.2.0/postfinancecheckout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 14:59:51.132661 postfinancecheckout-4.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_transaction_completion_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_transaction_iframe_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_transaction_lightbox_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_transaction_payment_page_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13825 2024-01-25 14:59:35.000000 postfinancecheckout-4.2.0/test/test_transaction_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.934881 postfinancecheckout-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-03 17:09:53.934881 postfinancecheckout-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5367 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.866881 postfinancecheckout-5.0.0/postfinancecheckout/
+-rw-r--r--   0 runner    (1001) docker     (127)    34382 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.878881 postfinancecheckout-5.0.0/postfinancecheckout/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22369 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23816 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/analytics_query_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22675 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/application_user_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/bank_account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/card_processing_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12652 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/charge_attempt_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/charge_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12855 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_level_payment_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16974 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_level_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31007 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/condition_type_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/country_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7205 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/country_state_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12743 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/currency_bank_account_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/currency_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29549 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/customer_address_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33478 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/customer_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/customer_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21661 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/delivery_indication_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12694 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/document_template_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7112 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/document_template_type_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/external_transfer_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26260 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/human_user_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12918 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/internal_transfer_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23004 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reconciliation_record_invoice_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25169 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reconciliation_record_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22210 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reimbursement_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/label_description_group_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/label_description_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/language_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/legal_organization_form_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/manual_task_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_connector_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_connector_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_link_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_brand_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7031 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_processor_configuration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_processor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12405 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_till_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17337 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_transaction_summary_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/permission_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/refund_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29218 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/refund_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/refund_recovery_bank_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34776 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/refund_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_recurring_order_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscriber_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21933 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_product_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31281 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21518 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_suspension_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12841 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12722 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22307 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/space_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/static_value_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46905 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/token_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17092 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/token_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29426 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31194 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_completion_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_iframe_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29557 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_invoice_comment_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40575 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_invoice_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_lightbox_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17314 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_line_item_version_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_mobile_sdk_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_payment_page_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80373 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_terminal_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21302 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_void_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13201 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/user_account_role_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/user_space_role_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/web_app_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_encryption_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_listener_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25419 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_url_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26356 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8545 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/encryption_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.930881 postfinancecheckout-5.0.0/postfinancecheckout/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    18601 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_account_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4062 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_application_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_address_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_human_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_payment_link_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_refund_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16919 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_shopify_subscription_product_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_space_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_invoice_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20178 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_pending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_webhook_listener_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_webhook_url_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/account_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/account_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/account_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19096 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/address_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12454 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query_execution_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query_result_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_schema_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_schema_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/application_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_create_with_mac_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/authenticated_card_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/authenticated_card_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16622 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_flow_direction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/card_authentication_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/card_authentication_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/card_cryptogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/card_cryptogram_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/card_cryptogram_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/cardholder_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/cardholder_authentication_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21380 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_attempt_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_attempt_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8390 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_configuration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/charge_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/client_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/client_error_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/completion_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/completion_line_item_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/condition_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/connector_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/connector_invocation_stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/creation_entity_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/criteria_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5874 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/currency_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10100 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7550 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8846 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20258 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customer_postal_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/customers_presence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/data_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10848 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/delivery_indication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/delivery_indication_decision_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/delivery_indication_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9844 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/document_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/document_template_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/document_template_type_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_filter_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_order_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_order_by_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/external_transfer_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/failure_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/failure_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/feature_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/gender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/human_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/human_user_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/human_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/internal_transfer_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6194 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_invoice_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_rejection_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reimbursement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reimbursement_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reimbursement_with_refund_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/legal_organization_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18658 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_attribute_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9524 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_reduction_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/localized_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8177 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_action_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/one_click_payment_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_adjustment_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12289 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_contract_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_contract_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_information_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_information_hash_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_initiation_advice_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_initiation_advice_file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20275 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_address_handling_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_protection_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_primary_risk_taker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_processor_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12362 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14186 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7778 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_dcc_transaction_sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_receipt_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_sum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9759 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_summary_fetch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/recurring_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24283 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7096 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_recovery_bank_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/refund_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_terminal_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_terminal_transaction_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/resource_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/resource_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_address_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_address_format_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_country_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/rest_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7371 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/role_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/sales_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/server_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_additional_line_item_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_integration_payment_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_integration_subscription_app_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_recurring_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_recurring_order_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_recurring_order_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15120 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20480 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_billing_interval_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15014 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_creation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_billing_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5444 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_tax_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27878 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_pricing_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension_initiator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_update_addresses_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24539 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5449 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version_item_price_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_weekday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_tax_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17704 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14673 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space_address_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/space_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/static_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tax_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tenant_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/terminal_receipt_fetch_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/terminal_receipt_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13760 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19146 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/token_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tokenization_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tokenized_card_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/tokenized_card_data_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63417 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_aware_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24689 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_environment_selection_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_group_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_replacement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16354 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_line_item_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_line_item_version_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_line_item_version_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_pending.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_user_interface_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_void.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_void_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_void_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/two_factor_authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/user_account_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/user_space_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/wallet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/web_app_confirmation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5748 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/web_app_confirmation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_encryption_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6223 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11239 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/postfinancecheckout/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.934881 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6241 2024-04-03 17:09:53.000000 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22312 2024-04-03 17:09:53.000000 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:09:53.000000 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 17:09:53.000000 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 17:09:53.000000 postfinancecheckout-5.0.0/postfinancecheckout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:09:53.934881 postfinancecheckout-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:09:53.930881 postfinancecheckout-5.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     7728 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_transaction_completion_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_transaction_iframe_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_transaction_lightbox_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_transaction_payment_page_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_transaction_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-03 17:09:36.000000 postfinancecheckout-5.0.0/test/test_webhook_encryption_service.py
```

### Comparing `postfinancecheckout-4.2.0/LICENSE` & `postfinancecheckout-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/PKG-INFO` & `postfinancecheckout-5.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfinancecheckout
-Version: 4.2.0
+Version: 5.0.0
 Summary: SDK that allows you to access PostFinance Checkout
 Author: Wallee AG
 License: Apache-2.0
 Keywords: postfinancecheckout,Payment,Payment Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,15 +41,15 @@
 ## Installation
 
 ### pip3 install (recommended)
 ```sh
 pip3 install --upgrade postfinancecheckout
 ```
 
-### pip3 install from source via github
+### pip3 install from source via GitHub
 
 ```sh
 pip3 install git+http://github.com/pfpayments/python-sdk.git
 ```
 (you may need to run `pip3` with root permission: `sudo pip3 install git+http://github.com/pfpayments/python-sdk.git` )
 
 ### install from source via Setuptools
@@ -69,15 +69,14 @@
 You can also optionally set `default_headers` to set some headers that will be sent to all requests
 
 ### Configuring a Service
 
 ```python
 from postfinancecheckout import Configuration
 from postfinancecheckout.api import TransactionServiceApi, TransactionPaymentPageServiceApi
-from postfinancecheckout.models import LineItem, LineItemType, TransactionCreate
 
 space_id = 405
 
 # default_headers is an optional param, that represents headers sent to all requests
 config = Configuration(
     user_id=512,
     api_secret='FKrO76r5VwJtBrqZawBspljbBNOxp5veKQQkOnZxucQ=',
```

### Comparing `postfinancecheckout-4.2.0/README.md` & `postfinancecheckout-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ## Installation
 
 ### pip3 install (recommended)
 ```sh
 pip3 install --upgrade postfinancecheckout
 ```
 
-### pip3 install from source via github
+### pip3 install from source via GitHub
 
 ```sh
 pip3 install git+http://github.com/pfpayments/python-sdk.git
 ```
 (you may need to run `pip3` with root permission: `sudo pip3 install git+http://github.com/pfpayments/python-sdk.git` )
 
 ### install from source via Setuptools
@@ -45,15 +45,14 @@
 You can also optionally set `default_headers` to set some headers that will be sent to all requests
 
 ### Configuring a Service
 
 ```python
 from postfinancecheckout import Configuration
 from postfinancecheckout.api import TransactionServiceApi, TransactionPaymentPageServiceApi
-from postfinancecheckout.models import LineItem, LineItemType, TransactionCreate
 
 space_id = 405
 
 # default_headers is an optional param, that represents headers sent to all requests
 config = Configuration(
     user_id=512,
     api_secret='FKrO76r5VwJtBrqZawBspljbBNOxp5veKQQkOnZxucQ=',
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/__init__.py` & `postfinancecheckout-5.0.0/postfinancecheckout/__init__.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/__init__.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/__init__.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/account_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/account_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/analytics_query_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/analytics_query_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/application_user_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/application_user_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/bank_account_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/bank_account_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/card_processing_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/card_processing_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/charge_attempt_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/charge_attempt_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/charge_bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/charge_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_level_payment_link_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_level_payment_link_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_level_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_level_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/charge_flow_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/charge_flow_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain;charset=utf-8'])
+            ['text/plain;charset=utf-8', 'application/json'])
 
         # Authentication setting
         auth_settings = []
 
         return self.api_client.call_api(
             '/charge-flow/fetch-charge-flow-payment-page-url', 'GET',
             path_params,
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/condition_type_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/condition_type_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/country_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/country_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/country_state_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/country_state_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/currency_bank_account_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/currency_bank_account_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/currency_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/currency_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/customer_address_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/customer_address_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/customer_comment_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/customer_comment_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/customer_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/customer_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/delivery_indication_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/delivery_indication_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/document_template_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/document_template_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/document_template_type_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/document_template_type_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/external_transfer_bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/external_transfer_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/human_user_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/human_user_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
         local_var_files = {}
 
         body_params = None
         if 'request' in params:
             body_params = params['request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json;charset=utf-8', 'text/csv'])
+            ['text/csv', 'application/json;charset=utf-8'])
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json;charset=utf-8'])
 
         # Authentication setting
         auth_settings = []
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/internal_transfer_bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/internal_transfer_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reconciliation_record_invoice_link_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reconciliation_record_invoice_link_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reconciliation_record_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reconciliation_record_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/invoice_reimbursement_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/invoice_reimbursement_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/label_description_group_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/label_description_group_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/label_description_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/label_description_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/language_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/language_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/legal_organization_form_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/legal_organization_form_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/manual_task_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/manual_task_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_connector_configuration_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_connector_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_connector_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_connector_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_link_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_link_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_brand_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_brand_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_configuration_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_method_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_method_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_processor_configuration_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_processor_configuration_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_processor_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_processor_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_till_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_till_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/payment_terminal_transaction_summary_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/payment_terminal_transaction_summary_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/permission_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/permission_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/refund_bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/refund_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/refund_comment_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/refund_comment_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param RefundCommentCreate entity:  (required)
+        :param RefundCommentCreate entity: The comment object which should be created. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -157,15 +157,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param RefundCommentCreate entity:  (required)
+        :param RefundCommentCreate entity: The comment object which should be created. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
@@ -305,23 +305,23 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'space_id' in params:
             query_params.append(('spaceId', params['space_id']))
-        if 'id' in params:
-            query_params.append(('id', params['id']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'id' in params:
+            body_params = params['id']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json;charset=utf-8'])
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json;charset=utf-8'])
@@ -353,15 +353,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -379,15 +379,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -464,15 +464,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -490,15 +490,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -575,15 +575,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -601,15 +601,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -686,15 +686,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param RefundCommentActive entity:  (required)
+        :param RefundCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -712,15 +712,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param RefundCommentActive entity:  (required)
+        :param RefundCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: RefundComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/refund_recovery_bank_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/refund_recovery_bank_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/refund_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/refund_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_recurring_order_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_recurring_order_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscriber_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscriber_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_product_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_product_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_suspension_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_suspension_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_subscription_version_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_subscription_version_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/shopify_transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/shopify_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/space_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/space_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/static_value_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/static_value_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/token_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/token_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/token_version_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/token_version_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_comment_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_comment_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionCommentCreate entity:  (required)
+        :param TransactionCommentCreate entity: The comment object which should be created. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -157,15 +157,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionCommentCreate entity:  (required)
+        :param TransactionCommentCreate entity: The comment object which should be created. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
@@ -305,23 +305,23 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'space_id' in params:
             query_params.append(('spaceId', params['space_id']))
-        if 'id' in params:
-            query_params.append(('id', params['id']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'id' in params:
+            body_params = params['id']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json;charset=utf-8'])
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json;charset=utf-8'])
@@ -353,15 +353,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -379,15 +379,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -464,15 +464,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -490,15 +490,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -575,15 +575,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -601,15 +601,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -686,15 +686,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionCommentActive entity:  (required)
+        :param TransactionCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -712,15 +712,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionCommentActive entity:  (required)
+        :param TransactionCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: TransactionComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_completion_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_completion_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_iframe_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_iframe_service_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain;charset=utf-8'])
+            ['text/plain;charset=utf-8', 'application/json'])
 
         # Authentication setting
         auth_settings = []
 
         return self.api_client.call_api(
             '/transaction-iframe/javascript-url', 'GET',
             path_params,
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_invoice_comment_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_invoice_comment_service_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionInvoiceCommentCreate entity:  (required)
+        :param TransactionInvoiceCommentCreate entity: The comment object which should be created. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -157,15 +157,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.create_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionInvoiceCommentCreate entity:  (required)
+        :param TransactionInvoiceCommentCreate entity: The comment object which should be created. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
@@ -305,23 +305,23 @@
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
         if 'space_id' in params:
             query_params.append(('spaceId', params['space_id']))
-        if 'id' in params:
-            query_params.append(('id', params['id']))
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'id' in params:
+            body_params = params['id']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json;charset=utf-8'])
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json;charset=utf-8'])
@@ -353,15 +353,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -379,15 +379,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.pin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to pin to the top. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -464,15 +464,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -490,15 +490,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.read_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment which should be returned. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -575,15 +575,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -601,15 +601,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.unpin_with_http_info(space_id, id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param int id:  (required)
+        :param int id: The id of the comment to unpin. (required)
         :return: None
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'id']
         all_params.append('async_req')
@@ -686,15 +686,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionInvoiceCommentActive entity:  (required)
+        :param TransactionInvoiceCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         
         kwargs['request_timeout'] = self.api_client.configuration.request_timeout
@@ -712,15 +712,15 @@
         asynchronous HTTP request, please pass async_req=True.
         
         >>> thread = api.update_with_http_info(space_id, entity, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param int space_id:  (required)
-        :param TransactionInvoiceCommentActive entity:  (required)
+        :param TransactionInvoiceCommentActive entity: The comment object with the properties which should be updated. (required)
         :return: TransactionInvoiceComment
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['space_id', 'entity']
         all_params.append('async_req')
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_invoice_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_invoice_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_lightbox_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_lightbox_service_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain;charset=utf-8'])
+            ['text/plain;charset=utf-8', 'application/json'])
 
         # Authentication setting
         auth_settings = []
 
         return self.api_client.call_api(
             '/transaction-lightbox/javascript-url', 'GET',
             path_params,
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_line_item_version_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_line_item_version_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_mobile_sdk_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_mobile_sdk_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain;charset=utf-8'])
+            ['text/plain;charset=utf-8', 'application/json'])
 
         # Authentication setting
         auth_settings = []
 
         return self.api_client.call_api(
             '/transaction-mobile-sdk/payment-form-url', 'GET',
             path_params,
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_payment_page_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_payment_page_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json', 'text/plain;charset=utf-8'])
+            ['text/plain;charset=utf-8', 'application/json'])
 
         # Authentication setting
         auth_settings = []
 
         return self.api_client.call_api(
             '/transaction-payment-page/payment-page-url', 'GET',
             path_params,
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         local_var_files = {}
 
         body_params = None
         if 'request' in params:
             body_params = params['request']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json;charset=utf-8', 'text/csv'])
+            ['text/csv', 'application/json;charset=utf-8'])
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json;charset=utf-8'])
 
         # Authentication setting
         auth_settings = []
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_terminal_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_terminal_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/transaction_void_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/transaction_void_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/user_account_role_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/user_account_role_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/user_space_role_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/user_space_role_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/web_app_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/web_app_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_encryption_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_encryption_service_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,18 +130,18 @@
         matcher = pattern.match(signature_header)
 
         if matcher:
             signature_algorithm = matcher.group(1)
             public_key_id = matcher.group(2)
             content_signature = matcher.group(3)
 
-            public_key = WebhookEncryptionServiceApi.read(self, public_key_id)
+            public_key_response = WebhookEncryptionServiceApi.read(self, public_key_id)
 
-            if public_key.public_key is None:
+            if public_key_response is None or public_key_response.public_key is None:
                 raise ValueError(f"Could not find public key with id {public_key_id}")
 
-            return EncryptionUtil.is_content_valid(content_to_verify, content_signature, public_key.public_key,
+            return EncryptionUtil.is_content_valid(content_to_verify, content_signature, public_key_response.public_key,
                                                    signature_algorithm)
         else:
             raise ValueError(
                 "Invalid webhook signature header. Expected format: 'algorithm=<algorithm>, keyId=<keyId>, "
                 "signature=<signature>'")
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_listener_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_listener_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api/webhook_url_service_api.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api/webhook_url_service_api.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/api_client.py` & `postfinancecheckout-5.0.0/postfinancecheckout/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     postfinancecheckout
 
     Python SDK
 
-    OpenAPI spec version: 4.2.0
+    OpenAPI spec version: 5.0.0
     
 """
 
 from __future__ import absolute_import
 
 import time
 import hashlib
@@ -21,14 +21,15 @@
 from multiprocessing.pool import ThreadPool
 import os
 import re
 import tempfile
 from enum import Enum
 import six
 import platform
+
 from six.moves.urllib.parse import quote
 from dateutil.parser import parse as date_util_parse
 import sys
 
 
 from postfinancecheckout.configuration import Configuration
 import postfinancecheckout.models
@@ -63,15 +64,15 @@
         for name, value in configuration.default_headers.items():
             self.default_headers[name] = value
 
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'postfinancecheckout/4.2.0/python'
+        self.user_agent = 'postfinancecheckout/5.0.0/python'
 
     def __del__(self):
         if self._pool is not None:
             self._pool.close()
             self._pool.join()
 
     @property
@@ -102,15 +103,15 @@
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
 
         # predefined default headers
         default_headers = {
-            'x-meta-sdk-version': '4.2.0',
+            'x-meta-sdk-version': '5.0.0',
             'x-meta-sdk-language': 'python',
             'x-meta-sdk-provider': 'PostFinance Checkout',
             'x-meta-sdk-language-version': platform.python_version()
         }
 
         header_params.update(self.default_headers)
         header_params.update(default_headers)
@@ -171,14 +172,18 @@
         if _preload_content:
             # deserialize response data
             if response_type:
                 return_data = self.deserialize(response_data, response_type)
             else:
                 return_data = None
 
+        if response_type is not None and hasattr(postfinancecheckout.models, response_type):
+            if all(value is None for value in return_data.__dict__.values()):
+                return_data = None
+
         if _return_http_data_only:
             return (return_data)
         else:
             return (return_data, response_data.status,
                     response_data.getheaders())
 
     def sanitize_for_serialization(self, obj):
@@ -447,15 +452,15 @@
 
         if files:
             for k, v in six.iteritems(files):
                 if not v:
                     continue
                 file_names = v if type(v) is list else [v]
                 for n in file_names:
-                    with open(n, 'rb') as f:
+                    with open(n, 'rb', encoding="utf8") as f:
                         filename = os.path.basename(f.name)
                         filedata = f.read()
                         mimetype = (mimetypes.guess_type(filename)[0] or
                                     'application/octet-stream')
                         params.append(
                             tuple([k, tuple([filename, filedata, mimetype])]))
 
@@ -532,15 +537,15 @@
 
         content_disposition = response.getheader("Content-Disposition")
         if content_disposition:
             filename = re.search(r'filename=[\'"]?([^\'"\s]+)[\'"]?',
                                  content_disposition).group(1)
             path = os.path.join(os.path.dirname(path), filename)
 
-        with open(path, "wb") as f:
+        with open(path, "wb", encoding="utf8") as f:
             f.write(response.data)
 
         return path
 
     def __deserialize_primitive(self, data, klass):
         """Deserializes string to primitive type.
 
@@ -553,15 +558,15 @@
             return klass(data)
         except UnicodeEncodeError:
             return six.text_type(data)
         except TypeError:
             return data
 
     def __deserialize_object(self, value):
-        """Return a original value.
+        """Return an original value.
 
         :return: object.
         """
         return value
 
     # TODO remove when the lowest supported Python version is 3.11+ . Then - also remove "python_dateutil" dependency from pip installs
     # https://stackoverflow.com/questions/55542280
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,19 +33,19 @@
         # dict to store API prefix (e.g. Bearer)
         self.api_key_prefix = {}
         # function to refresh API key if expired
         self.refresh_api_key_hook = None
         # Username for HTTP basic authentication
         self.username = ""
         # api secret for MAC authentication
-        self._api_secret=api_secret
+        self._api_secret = api_secret
         # user id for MAC authentication
-        self._user_id=user_id
+        self._user_id = user_id
         # version for MAC authentication
-        self._mac_version=mac_version
+        self._mac_version = mac_version
         # Password for HTTP basic authentication
         self.password = ""
 
         # Logging Settings
         self.logger = {"package_logger": logging.getLogger("postfinancecheckout"), "urllib3_logger": logging.getLogger("urllib3")}
         # Log format
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
@@ -258,10 +258,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 4.2.0\n"\
-               "SDK Package Version: 4.2.0".\
+               "Version of the API: 5.0.0\n"\
+               "SDK Package Version: 5.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/encryption_util.py` & `postfinancecheckout-5.0.0/postfinancecheckout/encryption_util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
             return False
 
     @staticmethod
     def _get_algorithm_class(algorithm):
         switch = {
             'SHA256withECDSA': ec.ECDSA,
         }
-        return switch.get(algorithm, None)
+        return switch.get(algorithm, None)
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/__init__.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/__init__.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_account_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_account_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_application_user_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_application_user_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_address_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_address_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_customer_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_customer_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_human_user_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_human_user_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_payment_link_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_payment_link_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_refund_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_refund_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_shopify_subscription_product_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_shopify_subscription_product_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_space_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_space_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_token_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_token_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_invoice_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_invoice_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_transaction_pending.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_transaction_pending.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_webhook_listener_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_webhook_listener_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,41 +5,67 @@
 
 
 
 class AbstractWebhookListenerUpdate:
 
     swagger_types = {
     
+        'enable_payload_signature_and_state': 'bool',
         'entity_states': 'list[str]',
         'name': 'str',
         'notify_every_change': 'bool',
         'state': 'CreationEntityState',
     }
 
     attribute_map = {
-        'entity_states': 'entityStates','name': 'name','notify_every_change': 'notifyEveryChange','state': 'state',
+        'enable_payload_signature_and_state': 'enablePayloadSignatureAndState','entity_states': 'entityStates','name': 'name','notify_every_change': 'notifyEveryChange','state': 'state',
     }
 
     
+    _enable_payload_signature_and_state = None
     _entity_states = None
     _name = None
     _notify_every_change = None
     _state = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
+        self.enable_payload_signature_and_state = kwargs.get('enable_payload_signature_and_state', None)
         self.entity_states = kwargs.get('entity_states', None)
         self.name = kwargs.get('name', None)
         self.notify_every_change = kwargs.get('notify_every_change', None)
         self.state = kwargs.get('state', None)
         
 
     
     @property
+    def enable_payload_signature_and_state(self):
+        """Gets the enable_payload_signature_and_state of this AbstractWebhookListenerUpdate.
+
+            Whether signature header and state property are enabled in webhook payload.
+
+        :return: The enable_payload_signature_and_state of this AbstractWebhookListenerUpdate.
+        :rtype: bool
+        """
+        return self._enable_payload_signature_and_state
+
+    @enable_payload_signature_and_state.setter
+    def enable_payload_signature_and_state(self, enable_payload_signature_and_state):
+        """Sets the enable_payload_signature_and_state of this AbstractWebhookListenerUpdate.
+
+            Whether signature header and state property are enabled in webhook payload.
+
+        :param enable_payload_signature_and_state: The enable_payload_signature_and_state of this AbstractWebhookListenerUpdate.
+        :type: bool
+        """
+
+        self._enable_payload_signature_and_state = enable_payload_signature_and_state
+    
+    @property
     def entity_states(self):
         """Gets the entity_states of this AbstractWebhookListenerUpdate.
 
             The entity's target states that are to be monitored.
 
         :return: The entity_states of this AbstractWebhookListenerUpdate.
         :rtype: list[str]
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/abstract_webhook_url_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/abstract_webhook_url_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/account.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/account.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/account_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/account_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/account_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/account_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/address_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/address_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query_execution.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query_execution.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_query_result_batch.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_query_result_batch.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_schema_column.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_schema_column.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/analytics_schema_table.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/analytics_schema_table.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/application_user.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/application_user.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_create_with_mac_key.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_create_with_mac_key.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/application_user_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/application_user_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/authenticated_card_data.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/authenticated_card_data.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/authenticated_card_data_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/authenticated_card_data_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/bank_account_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/bank_account_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,39 +13,41 @@
         'created_by': 'int',
         'created_on': 'datetime',
         'currency_bank_account': 'CurrencyBankAccount',
         'external_id': 'str',
         'flow_direction': 'BankTransactionFlowDirection',
         'id': 'int',
         'linked_space_id': 'int',
+        'payment_date': 'datetime',
         'planned_purge_date': 'datetime',
         'posting_amount': 'float',
         'reference': 'str',
         'source': 'int',
         'state': 'BankTransactionState',
         'total_adjustment_amount_including_tax': 'float',
         'type': 'int',
         'value_amount': 'float',
         'value_date': 'datetime',
         'version': 'int',
     }
 
     attribute_map = {
-        'adjustments': 'adjustments','created_by': 'createdBy','created_on': 'createdOn','currency_bank_account': 'currencyBankAccount','external_id': 'externalId','flow_direction': 'flowDirection','id': 'id','linked_space_id': 'linkedSpaceId','planned_purge_date': 'plannedPurgeDate','posting_amount': 'postingAmount','reference': 'reference','source': 'source','state': 'state','total_adjustment_amount_including_tax': 'totalAdjustmentAmountIncludingTax','type': 'type','value_amount': 'valueAmount','value_date': 'valueDate','version': 'version',
+        'adjustments': 'adjustments','created_by': 'createdBy','created_on': 'createdOn','currency_bank_account': 'currencyBankAccount','external_id': 'externalId','flow_direction': 'flowDirection','id': 'id','linked_space_id': 'linkedSpaceId','payment_date': 'paymentDate','planned_purge_date': 'plannedPurgeDate','posting_amount': 'postingAmount','reference': 'reference','source': 'source','state': 'state','total_adjustment_amount_including_tax': 'totalAdjustmentAmountIncludingTax','type': 'type','value_amount': 'valueAmount','value_date': 'valueDate','version': 'version',
     }
 
     
     _adjustments = None
     _created_by = None
     _created_on = None
     _currency_bank_account = None
     _external_id = None
     _flow_direction = None
     _id = None
     _linked_space_id = None
+    _payment_date = None
     _planned_purge_date = None
     _posting_amount = None
     _reference = None
     _source = None
     _state = None
     _total_adjustment_amount_including_tax = None
     _type = None
@@ -60,14 +62,15 @@
         self.created_by = kwargs.get('created_by', None)
         self.created_on = kwargs.get('created_on', None)
         self.currency_bank_account = kwargs.get('currency_bank_account', None)
         self.external_id = kwargs.get('external_id', None)
         self.flow_direction = kwargs.get('flow_direction', None)
         self.id = kwargs.get('id', None)
         self.linked_space_id = kwargs.get('linked_space_id', None)
+        self.payment_date = kwargs.get('payment_date', None)
         self.planned_purge_date = kwargs.get('planned_purge_date', None)
         self.posting_amount = kwargs.get('posting_amount', None)
         self.reference = kwargs.get('reference', None)
         self.source = kwargs.get('source', None)
         self.state = kwargs.get('state', None)
         self.total_adjustment_amount_including_tax = kwargs.get('total_adjustment_amount_including_tax', None)
         self.type = kwargs.get('type', None)
@@ -262,14 +265,37 @@
         :param linked_space_id: The linked_space_id of this BankTransaction.
         :type: int
         """
 
         self._linked_space_id = linked_space_id
     
     @property
+    def payment_date(self):
+        """Gets the payment_date of this BankTransaction.
+
+            The payment date describes the date when the transaction was made.
+
+        :return: The payment_date of this BankTransaction.
+        :rtype: datetime
+        """
+        return self._payment_date
+
+    @payment_date.setter
+    def payment_date(self, payment_date):
+        """Sets the payment_date of this BankTransaction.
+
+            The payment date describes the date when the transaction was made.
+
+        :param payment_date: The payment_date of this BankTransaction.
+        :type: datetime
+        """
+
+        self._payment_date = payment_date
+    
+    @property
     def planned_purge_date(self):
         """Gets the planned_purge_date of this BankTransaction.
 
             The date and time when the object is planned to be permanently removed. If the value is empty, the object will not be removed.
 
         :return: The planned_purge_date of this BankTransaction.
         :rtype: datetime
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_source.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_source.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/bank_transaction_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/bank_transaction_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/card_cryptogram.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/card_cryptogram.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/card_cryptogram_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/card_cryptogram_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/cardholder_authentication.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/cardholder_authentication.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/cardholder_authentication_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/cardholder_authentication_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_attempt.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_attempt.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_configuration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_configuration_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_configuration_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/charge_flow_level_payment_link.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/charge_flow_level_payment_link.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/client_error.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/client_error.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/completion_line_item.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/completion_line_item.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/completion_line_item_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/completion_line_item_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/condition.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/condition.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/condition_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/condition_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/connector_invocation.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/connector_invocation.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/criteria_operator.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/criteria_operator.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/currency_bank_account.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/currency_bank_account.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_address_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_address_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_comment_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_comment_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_postal_address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_postal_address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/customer_postal_address_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/customer_postal_address_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/delivery_indication.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/delivery_indication.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/delivery_indication_decision_reason.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/delivery_indication_decision_reason.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/document_template.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/document_template.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/document_template_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/document_template_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/document_template_type_group.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/document_template_type_group.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/entity_export_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/entity_export_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_filter.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_filter.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/entity_query_order_by.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/entity_query_order_by.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/external_transfer_bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/external_transfer_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/failure_reason.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/failure_reason.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/feature.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/feature.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/feature_category.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/feature_category.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/human_user.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/human_user.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/human_user_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/human_user_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/human_user_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/human_user_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/internal_transfer_bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/internal_transfer_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_invoice_link.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_invoice_link.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reconciliation_record_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reconciliation_record_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reimbursement.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reimbursement.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/invoice_reimbursement_with_refund_reference.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/invoice_reimbursement_with_refund_reference.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/label.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/label.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor_group.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor_group.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/label_descriptor_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/label_descriptor_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/legal_organization_form.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/legal_organization_form.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_attribute.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_attribute.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_attribute_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_attribute_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_reduction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_reduction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/line_item_reduction_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/line_item_reduction_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/localized_string.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/localized_string.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_action.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_action.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/manual_task_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/manual_task_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_adjustment.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_adjustment.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_adjustment_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_adjustment_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,35 +11,37 @@
     
         'applicable_for_transaction_processing': 'bool',
         'conditions': 'list[int]',
         'connector': 'int',
         'enabled_sales_channels': 'list[SalesChannel]',
         'enabled_space_views': 'list[int]',
         'id': 'int',
+        'image_path': 'str',
         'linked_space_id': 'int',
         'name': 'str',
         'payment_method_configuration': 'PaymentMethodConfiguration',
         'planned_purge_date': 'datetime',
         'priority': 'int',
         'processor_configuration': 'PaymentProcessorConfiguration',
         'state': 'CreationEntityState',
         'version': 'int',
     }
 
     attribute_map = {
-        'applicable_for_transaction_processing': 'applicableForTransactionProcessing','conditions': 'conditions','connector': 'connector','enabled_sales_channels': 'enabledSalesChannels','enabled_space_views': 'enabledSpaceViews','id': 'id','linked_space_id': 'linkedSpaceId','name': 'name','payment_method_configuration': 'paymentMethodConfiguration','planned_purge_date': 'plannedPurgeDate','priority': 'priority','processor_configuration': 'processorConfiguration','state': 'state','version': 'version',
+        'applicable_for_transaction_processing': 'applicableForTransactionProcessing','conditions': 'conditions','connector': 'connector','enabled_sales_channels': 'enabledSalesChannels','enabled_space_views': 'enabledSpaceViews','id': 'id','image_path': 'imagePath','linked_space_id': 'linkedSpaceId','name': 'name','payment_method_configuration': 'paymentMethodConfiguration','planned_purge_date': 'plannedPurgeDate','priority': 'priority','processor_configuration': 'processorConfiguration','state': 'state','version': 'version',
     }
 
     
     _applicable_for_transaction_processing = None
     _conditions = None
     _connector = None
     _enabled_sales_channels = None
     _enabled_space_views = None
     _id = None
+    _image_path = None
     _linked_space_id = None
     _name = None
     _payment_method_configuration = None
     _planned_purge_date = None
     _priority = None
     _processor_configuration = None
     _state = None
@@ -50,14 +52,15 @@
         
         self.applicable_for_transaction_processing = kwargs.get('applicable_for_transaction_processing', None)
         self.conditions = kwargs.get('conditions', None)
         self.connector = kwargs.get('connector', None)
         self.enabled_sales_channels = kwargs.get('enabled_sales_channels', None)
         self.enabled_space_views = kwargs.get('enabled_space_views', None)
         self.id = kwargs.get('id', None)
+        self.image_path = kwargs.get('image_path', None)
         self.linked_space_id = kwargs.get('linked_space_id', None)
         self.name = kwargs.get('name', None)
         self.payment_method_configuration = kwargs.get('payment_method_configuration', None)
         self.planned_purge_date = kwargs.get('planned_purge_date', None)
         self.priority = kwargs.get('priority', None)
         self.processor_configuration = kwargs.get('processor_configuration', None)
         self.state = kwargs.get('state', None)
@@ -200,14 +203,37 @@
         :param id: The id of this PaymentConnectorConfiguration.
         :type: int
         """
 
         self._id = id
     
     @property
+    def image_path(self):
+        """Gets the image_path of this PaymentConnectorConfiguration.
+
+            
+
+        :return: The image_path of this PaymentConnectorConfiguration.
+        :rtype: str
+        """
+        return self._image_path
+
+    @image_path.setter
+    def image_path(self, image_path):
+        """Sets the image_path of this PaymentConnectorConfiguration.
+
+            
+
+        :param image_path: The image_path of this PaymentConnectorConfiguration.
+        :type: str
+        """
+
+        self._image_path = image_path
+    
+    @property
     def linked_space_id(self):
         """Gets the linked_space_id of this PaymentConnectorConfiguration.
 
             The ID of the space this object belongs to.
 
         :return: The linked_space_id of this PaymentConnectorConfiguration.
         :rtype: int
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_connector_feature.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_connector_feature.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_contract.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_contract.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_contract_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_contract_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_information_hash.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_information_hash.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_information_hash_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_information_hash_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_initiation_advice_file.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_initiation_advice_file.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_link_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_link_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method_brand.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method_brand.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_method_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_method_configuration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_processor.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_processor.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_processor_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_processor_configuration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_configuration_version.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_configuration_version.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_dcc_transaction_sum.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_dcc_transaction_sum.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_location_version.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_location_version.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_receipt_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_receipt_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_sum.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_sum.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_summary.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_transaction_summary_fetch_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_transaction_summary_fetch_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/payment_terminal_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/payment_terminal_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/permission.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/permission.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_comment_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_comment_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/refund_recovery_bank_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/refund_recovery_bank_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_document.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_document.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_terminal_receipt.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_terminal_receipt.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rendered_terminal_transaction_summary.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rendered_terminal_transaction_summary.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/resource_path.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/resource_path.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rest_address_format.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rest_address_format.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rest_country.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rest_country.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rest_country_state.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rest_country_state.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rest_currency.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rest_currency.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/rest_language.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/rest_language.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/role.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/role.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/sales_channel.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/sales_channel.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/scope.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/scope.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/server_error.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/server_error.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_integration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_integration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_recurring_order.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_recurring_order.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_recurring_order_update_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_recurring_order_update_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscriber_creation.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscriber_creation.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_address_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_address_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_creation_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_creation_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_billing_configuration.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_billing_configuration.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_item.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_item.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_model_tax_line.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_model_tax_line.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_product_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_product_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_suspension_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_suspension_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_update_addresses_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_update_addresses_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_update_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_update_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_subscription_version_item.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_subscription_version_item.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_tax_line.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_tax_line.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/shopify_transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/shopify_transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space_address.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space_address.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space_address_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space_address_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/space_view.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/space_view.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/static_value.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/static_value.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/tax.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/tax.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/tax_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/tax_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/tenant_database.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/tenant_database.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/terminal_receipt_fetch_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/terminal_receipt_fetch_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/token.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/token.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/token_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/token_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/token_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/token_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/token_version.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/token_version.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/token_version_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/token_version_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/tokenized_card_data.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/tokenized_card_data.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/tokenized_card_data_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/tokenized_card_data_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_aware_entity.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_aware_entity.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_comment_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_comment_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_completion_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_completion_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_group.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_group.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment_active.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment_active.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_comment_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_comment_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_invoice_replacement.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_invoice_replacement.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_line_item_version.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_line_item_version.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_line_item_version_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_line_item_version_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_pending.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_pending.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/transaction_void.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/transaction_void.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/two_factor_authentication_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/two_factor_authentication_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/user.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/user.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/user_account_role.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/user_account_role.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/user_space_role.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/user_space_role.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/wallet_type.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/wallet_type.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/web_app_confirmation_request.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/web_app_confirmation_request.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/web_app_confirmation_response.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/web_app_confirmation_response.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_encryption_public_key.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_encryption_public_key.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_identity.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_identity.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,32 +5,34 @@
 
 
 
 class WebhookListener:
 
     swagger_types = {
     
+        'enable_payload_signature_and_state': 'bool',
         'entity': 'int',
         'entity_states': 'list[str]',
         'id': 'int',
         'identity': 'WebhookIdentity',
         'linked_space_id': 'int',
         'name': 'str',
         'notify_every_change': 'bool',
         'planned_purge_date': 'datetime',
         'state': 'CreationEntityState',
         'url': 'WebhookUrl',
         'version': 'int',
     }
 
     attribute_map = {
-        'entity': 'entity','entity_states': 'entityStates','id': 'id','identity': 'identity','linked_space_id': 'linkedSpaceId','name': 'name','notify_every_change': 'notifyEveryChange','planned_purge_date': 'plannedPurgeDate','state': 'state','url': 'url','version': 'version',
+        'enable_payload_signature_and_state': 'enablePayloadSignatureAndState','entity': 'entity','entity_states': 'entityStates','id': 'id','identity': 'identity','linked_space_id': 'linkedSpaceId','name': 'name','notify_every_change': 'notifyEveryChange','planned_purge_date': 'plannedPurgeDate','state': 'state','url': 'url','version': 'version',
     }
 
     
+    _enable_payload_signature_and_state = None
     _entity = None
     _entity_states = None
     _id = None
     _identity = None
     _linked_space_id = None
     _name = None
     _notify_every_change = None
@@ -38,14 +40,15 @@
     _state = None
     _url = None
     _version = None
 
     def __init__(self, **kwargs):
         self.discriminator = None
         
+        self.enable_payload_signature_and_state = kwargs.get('enable_payload_signature_and_state', None)
         self.entity = kwargs.get('entity', None)
         self.entity_states = kwargs.get('entity_states', None)
         self.id = kwargs.get('id', None)
         self.identity = kwargs.get('identity', None)
         self.linked_space_id = kwargs.get('linked_space_id', None)
         self.name = kwargs.get('name', None)
         self.notify_every_change = kwargs.get('notify_every_change', None)
@@ -53,14 +56,37 @@
         self.state = kwargs.get('state', None)
         self.url = kwargs.get('url', None)
         self.version = kwargs.get('version', None)
         
 
     
     @property
+    def enable_payload_signature_and_state(self):
+        """Gets the enable_payload_signature_and_state of this WebhookListener.
+
+            Whether signature header and state property are enabled in webhook payload.
+
+        :return: The enable_payload_signature_and_state of this WebhookListener.
+        :rtype: bool
+        """
+        return self._enable_payload_signature_and_state
+
+    @enable_payload_signature_and_state.setter
+    def enable_payload_signature_and_state(self, enable_payload_signature_and_state):
+        """Sets the enable_payload_signature_and_state of this WebhookListener.
+
+            Whether signature header and state property are enabled in webhook payload.
+
+        :param enable_payload_signature_and_state: The enable_payload_signature_and_state of this WebhookListener.
+        :type: bool
+        """
+
+        self._enable_payload_signature_and_state = enable_payload_signature_and_state
+    
+    @property
     def entity(self):
         """Gets the entity of this WebhookListener.
 
             The entity that is to be monitored.
 
         :return: The entity of this WebhookListener.
         :rtype: int
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_entity.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_entity.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_listener_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_listener_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url_create.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url_create.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/models/webhook_url_update.py` & `postfinancecheckout-5.0.0/postfinancecheckout/models/webhook_url_update.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout/rest.py` & `postfinancecheckout-5.0.0/postfinancecheckout/rest.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout.egg-info/PKG-INFO` & `postfinancecheckout-5.0.0/postfinancecheckout.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfinancecheckout
-Version: 4.2.0
+Version: 5.0.0
 Summary: SDK that allows you to access PostFinance Checkout
 Author: Wallee AG
 License: Apache-2.0
 Keywords: postfinancecheckout,Payment,Payment Integration
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: Apache Software License
@@ -41,15 +41,15 @@
 ## Installation
 
 ### pip3 install (recommended)
 ```sh
 pip3 install --upgrade postfinancecheckout
 ```
 
-### pip3 install from source via github
+### pip3 install from source via GitHub
 
 ```sh
 pip3 install git+http://github.com/pfpayments/python-sdk.git
 ```
 (you may need to run `pip3` with root permission: `sudo pip3 install git+http://github.com/pfpayments/python-sdk.git` )
 
 ### install from source via Setuptools
@@ -69,15 +69,14 @@
 You can also optionally set `default_headers` to set some headers that will be sent to all requests
 
 ### Configuring a Service
 
 ```python
 from postfinancecheckout import Configuration
 from postfinancecheckout.api import TransactionServiceApi, TransactionPaymentPageServiceApi
-from postfinancecheckout.models import LineItem, LineItemType, TransactionCreate
 
 space_id = 405
 
 # default_headers is an optional param, that represents headers sent to all requests
 config = Configuration(
     user_id=512,
     api_secret='FKrO76r5VwJtBrqZawBspljbBNOxp5veKQQkOnZxucQ=',
```

### Comparing `postfinancecheckout-4.2.0/postfinancecheckout.egg-info/SOURCES.txt` & `postfinancecheckout-5.0.0/postfinancecheckout.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -407,8 +407,9 @@
 postfinancecheckout/models/webhook_url_create.py
 postfinancecheckout/models/webhook_url_update.py
 test/test_refund.py
 test/test_transaction_completion_service.py
 test/test_transaction_iframe_service.py
 test/test_transaction_lightbox_service.py
 test/test_transaction_payment_page_service.py
-test/test_transaction_service.py
+test/test_transaction_service.py
+test/test_webhook_encryption_service.py
```

### Comparing `postfinancecheckout-4.2.0/setup.py` & `postfinancecheckout-5.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # coding: utf-8
 
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 NAME = "postfinancecheckout"
-VERSION = "4.2.0"
+VERSION = "5.0.0"
 
 REQUIRES = [
     "certifi >= 14.05.14",
     "six >= 1.10",
     "python_dateutil >= 2.8.2",
     "setuptools >= 68.0.0",
     "urllib3 >= 2.0.7",
```

### Comparing `postfinancecheckout-4.2.0/test/test_refund.py` & `postfinancecheckout-5.0.0/test/test_refund.py`

 * *Files 9% similar despite different names*

```diff
@@ -80,16 +80,26 @@
 
         self.assertEqual(
             RefundState.SUCCESSFUL,
             refund.state,
             "State must be SUCCESSFUL",
         )
 
+    def test_read_not_found(self):
+        """read_not_found() should read not found refund as none"""
+
+        NOT_FOUND_REFUND_ID = 0
+
+        refund_read = self.refund_service.read(
+            space_id=SPACE_ID, id=NOT_FOUND_REFUND_ID)
+
+        self.assertIsNone(refund_read, "Return data must be None.")
+
     def test_read(self):
-        """read() should should fetch refund details"""
+        """read() should fetch refund details"""
 
         transaction = self.transaction_service.create(
             space_id=SPACE_ID, transaction=get_transaction_create())
 
         transaction_processed = self.card_processing_service.process(
             space_id=SPACE_ID,
             transaction_id=transaction.id,
@@ -117,14 +127,16 @@
             refund.state,
             "State must be SUCCESSFUL",
         )
 
         read_refund = self.refund_service.read(
             space_id=SPACE_ID, id=refund.id)
 
+        self.assertIsNotNone(read_refund, "Return data must not be None.")
+
         self.assertEqual(
             refund.id,
             read_refund.id,
             "Refund ids must match",
         )
 
     def test_search(self):
@@ -160,23 +172,24 @@
             refund.state,
             "State must be SUCCESSFUL",
         )
 
         criteria = EntityQuery(
             filter=EntityQueryFilter(
                 field_name="id",
-                value=transaction_completion.id,
+                value=refund.id,
                 type=EntityQueryFilterType.LEAF,
                 operator=CriteriaOperator.EQUALS
             )
         )
 
         refunds_found = self.refund_service.search(
             SPACE_ID, query=criteria)
 
+        self.assertEqual(1, len(refunds_found))
         for ref in refunds_found:
             self.assertEqual(
                 refund.id,
                 ref.id,
                 "Refund ids must match",
             )
```

### Comparing `postfinancecheckout-4.2.0/test/test_transaction_completion_service.py` & `postfinancecheckout-5.0.0/test/test_transaction_completion_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     EntityQueryFilterType,
     CriteriaOperator,
     EntityQuery,
     TransactionState,
     TransactionCompletionState
 )
 
+
 class TransactionCompletionServiceTest(unittest.TestCase):
     """TransactionCompletionServiceApi tests"""
 
     def setUp(self):
         self.transaction_service = TransactionServiceApi(API_CONFIG)
         self.transaction_completion_service = TransactionCompletionServiceApi(
             API_CONFIG)
@@ -122,14 +123,16 @@
 
         transaction_completion = self.transaction_completion_service.complete_online(
             space_id=SPACE_ID, id=transaction_processed.id)
 
         transaction_read = self.transaction_completion_service.read(
             space_id=SPACE_ID, id=transaction_completion.id)
 
+        self.assertIsNotNone(transaction_read, "Return data must not be None.")
+
         self.assertEqual(transaction_completion.id,
                          transaction_read.id, "Transaction ids must match", )
 
     def test_count(self):
         """count() should count transaction completions based on provided criteria"""
 
         transaction = self.transaction_service.create(
```

### Comparing `postfinancecheckout-4.2.0/test/test_transaction_iframe_service.py` & `postfinancecheckout-5.0.0/test/test_transaction_iframe_service.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/test/test_transaction_lightbox_service.py` & `postfinancecheckout-5.0.0/test/test_transaction_lightbox_service.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/test/test_transaction_payment_page_service.py` & `postfinancecheckout-5.0.0/test/test_transaction_payment_page_service.py`

 * *Files identical despite different names*

### Comparing `postfinancecheckout-4.2.0/test/test_transaction_service.py` & `postfinancecheckout-5.0.0/test/test_transaction_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,23 +151,35 @@
             id=transaction.id,
             integration_mode="payment_page",
         )
 
         self.assertTrue(len(payment_methods) > 0,
                         "Payment methods should be configured for a given transaction in test space", )
 
+    def test_read_not_found(self):
+        """read_not_found() should read not found transaction as none"""
+
+        NOT_FOUND_TRANSACTION_ID = 0
+
+        transaction_read = self.transaction_service.read(
+            space_id=SPACE_ID, id=NOT_FOUND_TRANSACTION_ID)
+
+        self.assertIsNone(transaction_read, "Return data must be None.")
+
     def test_read(self):
         """read() should read transaction details"""
 
         transaction = self.transaction_service.create(
             space_id=SPACE_ID, transaction=get_transaction_create())
 
         transaction_read = self.transaction_service.read(
             space_id=SPACE_ID, id=transaction.id)
 
+        self.assertIsNotNone(transaction_read, "Return data must not be None.")
+
         self.assertEqual(transaction.id, transaction_read.id,
                          "Transaction ids should match")
 
         self.assertEqual(TransactionState.PENDING,
                          transaction_read.state, "State must be PENDING")
 
     def test_read_with_credentials_for_bad_creds(self):
@@ -191,14 +203,16 @@
 
         creds = self.transaction_service.create_transaction_credentials(
             space_id=SPACE_ID, id=transaction.id)
 
         transaction_read = self.transaction_service.read_with_credentials(
             credentials=creds)
 
+        self.assertIsNotNone(transaction_read, "Return data must not be None.")
+
         self.assertEqual(transaction.id, transaction_read.id,
                          "Transaction ids should match")
 
     def test_search(self):
         """search() should find transaction by id"""
 
         transaction = self.transaction_service.create(
@@ -235,15 +249,15 @@
         transaction = self.transaction_service.create(
             space_id=SPACE_ID, transaction=get_transaction_create())
 
         transaction_processed = self.transaction_service.process_without_user_interaction(
             space_id=SPACE_ID, id=transaction.id)
 
         self.assertEqual(
-            transaction.id, transaction_processed.id, "Transaction ids mush match"
+            transaction.id, transaction_processed.id, "Transaction ids must match"
         )
 
     def test_fetch_one_click_tokens_with_credentials_no_tokens(self):
         """fetch_one_click_tokens_with_credentials() should return one-click payment tokens (if any) for provided transaction"""
 
         transaction = self.transaction_service.create(
             space_id=SPACE_ID, transaction=get_transaction_create())
@@ -314,14 +328,16 @@
 
         self.assertTrue("securityToken" in payment_url2,
                         "URL must be of a proper format")
 
         transaction2_read = self.transaction_service.read(
             space_id=SPACE_ID, id=transaction2.id)
 
+        self.assertIsNotNone(transaction2_read, "Return data must not be None.")
+
         self.assertEqual(
             TransactionState.AUTHORIZED,
             transaction2_read.state,
             "State must be AUTHORIZED",
         )
 
         # cleanup - 2nd transaction
```

