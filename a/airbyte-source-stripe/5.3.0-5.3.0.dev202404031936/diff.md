# Comparing `tmp/airbyte_source_stripe-5.3.0.tar.gz` & `tmp/airbyte_source_stripe-5.3.0.dev202404031936.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_stripe-5.3.0.tar", max compression
+gzip compressed data, was "airbyte_source_stripe-5.3.0.dev202404031936.tar", max compression
```

## Comparing `airbyte_source_stripe-5.3.0.tar` & `airbyte_source_stripe-5.3.0.dev202404031936.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     4496 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/README.md
--rw-r--r--   0        0        0      804 2024-03-16 00:07:32.333140 airbyte_source_stripe-5.3.0/pyproject.toml
--rw-r--r--   0        0        0      122 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/__init__.py
--rw-r--r--   0        0        0     6009 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/availability_strategy.py
--rw-r--r--   0        0        0     1595 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/run.py
--rw-r--r--   0        0        0    22080 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/accounts.json
--rw-r--r--   0        0        0     1778 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/application_fees.json
--rw-r--r--   0        0        0      801 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/application_fees_refunds.json
--rw-r--r--   0        0        0     6359 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/authorizations.json
--rw-r--r--   0        0        0      131 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1032 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/bank_accounts.json
--rw-r--r--   0        0        0      121 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/cardholders.json
--rw-r--r--   0        0        0      115 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/cards.json
--rw-r--r--   0        0        0    27559 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/charges.json
--rw-r--r--   0        0        0    14125 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/checkout_sessions.json
--rw-r--r--   0        0        0     6396 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/checkout_sessions_line_items.json
--rw-r--r--   0        0        0     1157 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/coupons.json
--rw-r--r--   0        0        0     9606 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/credit_notes.json
--rw-r--r--   0        0        0      899 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/customer_balance_transactions.json
--rw-r--r--   0        0        0      119 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/customers.json
--rw-r--r--   0        0        0     4255 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/disputes.json
--rw-r--r--   0        0        0      644 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/early_fraud_warnings.json
--rw-r--r--   0        0        0      897 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/events.json
--rw-r--r--   0        0        0     1043 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/external_account_bank_accounts.json
--rw-r--r--   0        0        0     1654 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/external_account_cards.json
--rw-r--r--   0        0        0      642 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/file_links.json
--rw-r--r--   0        0        0     1904 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/files.json
--rw-r--r--   0        0        0     3890 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/invoice_items.json
--rw-r--r--   0        0        0     5237 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/invoice_line_items.json
--rw-r--r--   0        0        0    13937 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/invoices.json
--rw-r--r--   0        0        0  3248217 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/openapi_spec.json
--rw-r--r--   0        0        0      125 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/payment_intents.json
--rw-r--r--   0        0        0      125 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/payment_methods.json
--rw-r--r--   0        0        0     3038 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/payouts.json
--rw-r--r--   0        0        0    10760 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/persons.json
--rw-r--r--   0        0        0     2099 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/plans.json
--rw-r--r--   0        0        0     1932 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/prices.json
--rw-r--r--   0        0        0     2080 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/products.json
--rw-r--r--   0        0        0     2201 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/promotion_codes.json
--rw-r--r--   0        0        0     1590 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/refunds.json
--rw-r--r--   0        0        0     1710 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/reviews.json
--rw-r--r--   0        0        0    13649 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/setup_attempts.json
--rw-r--r--   0        0        0      123 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/setup_intents.json
--rw-r--r--   0        0        0      392 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/address.json
--rw-r--r--   0        0        0     1486 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/balance_transactions.json
--rw-r--r--   0        0        0     2149 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/card.json
--rw-r--r--   0        0        0     2489 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/cardholder.json
--rw-r--r--   0        0        0    23837 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/customer.json
--rw-r--r--   0        0        0     2206 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/issuing_transaction_purchase_details.json
--rw-r--r--   0        0        0    26783 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/payment_intent.json
--rw-r--r--   0        0        0     6034 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/payment_method.json
--rw-r--r--   0        0        0      163 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/payment_method_configuration_details.json
--rw-r--r--   0        0        0     2109 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/price.json
--rw-r--r--   0        0        0     2024 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/setup_intent.json
--rw-r--r--   0        0        0      510 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/spending_controls.json
--rw-r--r--   0        0        0      940 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/tax_rate.json
--rw-r--r--   0        0        0       78 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/tax_rates.json
--rw-r--r--   0        0        0     1222 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/shipping_rates.json
--rw-r--r--   0        0        0     3769 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/subscription_items.json
--rw-r--r--   0        0        0     5505 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/subscription_schedule.json
--rw-r--r--   0        0        0    10700 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/subscriptions.json
--rw-r--r--   0        0        0     1286 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/top_ups.json
--rw-r--r--   0        0        0     1957 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/transactions.json
--rw-r--r--   0        0        0      809 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/transfer_reversals.json
--rw-r--r--   0        0        0     1999 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/transfers.json
--rw-r--r--   0        0        0      716 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/schemas/usage_records.json
--rw-r--r--   0        0        0    25674 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/source.py
--rw-r--r--   0        0        0     3043 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/spec.yaml
--rw-r--r--   0        0        0     1861 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/stream_helpers.py
--rw-r--r--   0        0        0    37125 2024-03-15 20:25:52.000000 airbyte_source_stripe-5.3.0/source_stripe/streams.py
--rw-r--r--   0        0        0     5264 1970-01-01 00:00:00.000000 airbyte_source_stripe-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4496 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/README.md
+-rw-r--r--   0        0        0      820 2024-04-03 19:36:18.098208 airbyte_source_stripe-5.3.0.dev202404031936/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/__init__.py
+-rw-r--r--   0        0        0     6009 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/availability_strategy.py
+-rw-r--r--   0        0        0     1595 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/run.py
+-rw-r--r--   0        0        0    22080 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/accounts.json
+-rw-r--r--   0        0        0     1778 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/application_fees.json
+-rw-r--r--   0        0        0      801 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/application_fees_refunds.json
+-rw-r--r--   0        0        0     6359 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/authorizations.json
+-rw-r--r--   0        0        0      131 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1032 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/bank_accounts.json
+-rw-r--r--   0        0        0      121 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/cardholders.json
+-rw-r--r--   0        0        0      115 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/cards.json
+-rw-r--r--   0        0        0    27559 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/charges.json
+-rw-r--r--   0        0        0    14125 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/checkout_sessions.json
+-rw-r--r--   0        0        0     6396 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/checkout_sessions_line_items.json
+-rw-r--r--   0        0        0     1157 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/coupons.json
+-rw-r--r--   0        0        0     9606 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/credit_notes.json
+-rw-r--r--   0        0        0      899 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/customer_balance_transactions.json
+-rw-r--r--   0        0        0      119 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/customers.json
+-rw-r--r--   0        0        0     4255 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/disputes.json
+-rw-r--r--   0        0        0      644 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/early_fraud_warnings.json
+-rw-r--r--   0        0        0      897 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/events.json
+-rw-r--r--   0        0        0     1043 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/external_account_bank_accounts.json
+-rw-r--r--   0        0        0     1654 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/external_account_cards.json
+-rw-r--r--   0        0        0      642 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/file_links.json
+-rw-r--r--   0        0        0     1904 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/files.json
+-rw-r--r--   0        0        0     3890 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoice_items.json
+-rw-r--r--   0        0        0     5237 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoice_line_items.json
+-rw-r--r--   0        0        0    13937 2024-04-03 19:32:17.686677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoices.json
+-rw-r--r--   0        0        0  3248217 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/openapi_spec.json
+-rw-r--r--   0        0        0      125 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/payment_intents.json
+-rw-r--r--   0        0        0      125 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/payment_methods.json
+-rw-r--r--   0        0        0     3038 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/payouts.json
+-rw-r--r--   0        0        0    10760 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/persons.json
+-rw-r--r--   0        0        0     2099 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/plans.json
+-rw-r--r--   0        0        0     1932 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/prices.json
+-rw-r--r--   0        0        0     2080 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/products.json
+-rw-r--r--   0        0        0     2201 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/promotion_codes.json
+-rw-r--r--   0        0        0     1590 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/refunds.json
+-rw-r--r--   0        0        0     1710 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/reviews.json
+-rw-r--r--   0        0        0    13649 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/setup_attempts.json
+-rw-r--r--   0        0        0      123 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/setup_intents.json
+-rw-r--r--   0        0        0      392 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/address.json
+-rw-r--r--   0        0        0     1486 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/balance_transactions.json
+-rw-r--r--   0        0        0     2149 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/card.json
+-rw-r--r--   0        0        0     2489 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/cardholder.json
+-rw-r--r--   0        0        0    23837 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/customer.json
+-rw-r--r--   0        0        0     2206 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/issuing_transaction_purchase_details.json
+-rw-r--r--   0        0        0    26783 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/payment_intent.json
+-rw-r--r--   0        0        0     6034 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/payment_method.json
+-rw-r--r--   0        0        0      163 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/payment_method_configuration_details.json
+-rw-r--r--   0        0        0     2109 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/price.json
+-rw-r--r--   0        0        0     2024 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/setup_intent.json
+-rw-r--r--   0        0        0      510 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/spending_controls.json
+-rw-r--r--   0        0        0      940 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/tax_rate.json
+-rw-r--r--   0        0        0       78 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/tax_rates.json
+-rw-r--r--   0        0        0     1222 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shipping_rates.json
+-rw-r--r--   0        0        0     3769 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscription_items.json
+-rw-r--r--   0        0        0     5505 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscription_schedule.json
+-rw-r--r--   0        0        0    10700 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscriptions.json
+-rw-r--r--   0        0        0     1286 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/top_ups.json
+-rw-r--r--   0        0        0     1957 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transactions.json
+-rw-r--r--   0        0        0      809 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transfer_reversals.json
+-rw-r--r--   0        0        0     1999 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transfers.json
+-rw-r--r--   0        0        0      716 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/usage_records.json
+-rw-r--r--   0        0        0    25674 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/source.py
+-rw-r--r--   0        0        0     3043 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/spec.yaml
+-rw-r--r--   0        0        0     1861 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/stream_helpers.py
+-rw-r--r--   0        0        0    37125 2024-04-03 19:32:17.694677 airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/streams.py
+-rw-r--r--   0        0        0     5280 1970-01-01 00:00:00.000000 airbyte_source_stripe-5.3.0.dev202404031936/PKG-INFO
```

### Comparing `airbyte_source_stripe-5.3.0/README.md` & `airbyte_source_stripe-5.3.0.dev202404031936/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/pyproject.toml` & `airbyte_source_stripe-5.3.0.dev202404031936/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "5.3.0"
+version = "5.3.0.dev202404031936"
 name = "airbyte-source-stripe"
 description = "Source implementation for Stripe."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "Elv2"
 readme = "README.md"
```

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/availability_strategy.py` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/run.py` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/accounts.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/application_fees.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/application_fees.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/application_fees_refunds.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/application_fees_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/authorizations.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/authorizations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/bank_accounts.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/bank_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/charges.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/charges.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/checkout_sessions.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/checkout_sessions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/checkout_sessions_line_items.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/checkout_sessions_line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/coupons.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/coupons.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/credit_notes.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/credit_notes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/customer_balance_transactions.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/customer_balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/disputes.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/early_fraud_warnings.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/early_fraud_warnings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/events.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/events.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/external_account_bank_accounts.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/external_account_bank_accounts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/external_account_cards.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/external_account_cards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/file_links.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/file_links.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/files.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/files.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/invoice_items.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoice_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/invoice_line_items.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoice_line_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/invoices.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/openapi_spec.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/openapi_spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/payouts.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/payouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/persons.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/persons.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/plans.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/plans.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/prices.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/prices.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/products.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/promotion_codes.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/promotion_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/refunds.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/reviews.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/reviews.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/setup_attempts.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/setup_attempts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/balance_transactions.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/card.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/card.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/cardholder.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/cardholder.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/customer.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/customer.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/issuing_transaction_purchase_details.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/issuing_transaction_purchase_details.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/payment_intent.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/payment_intent.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/payment_method.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/payment_method.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/price.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/price.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/setup_intent.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/setup_intent.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shared/tax_rate.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shared/tax_rate.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/shipping_rates.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/shipping_rates.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/subscription_items.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscription_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/subscription_schedule.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscription_schedule.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/subscriptions.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/subscriptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/top_ups.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/top_ups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/transactions.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/transfer_reversals.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transfer_reversals.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/transfers.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/transfers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/schemas/usage_records.json` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/schemas/usage_records.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/source.py` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/spec.yaml` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/stream_helpers.py` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/stream_helpers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/source_stripe/streams.py` & `airbyte_source_stripe-5.3.0.dev202404031936/source_stripe/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_stripe-5.3.0/PKG-INFO` & `airbyte_source_stripe-5.3.0.dev202404031936/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-stripe
-Version: 5.3.0
+Version: 5.3.0.dev202404031936
 Summary: Source implementation for Stripe.
 Home-page: https://airbyte.com
 License: Elv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

