# Comparing `tmp/merchantapi-2.5.0.tar.gz` & `tmp/merchantapi-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merchantapi-2.5.0.tar", last modified: Tue Aug  1 21:53:39 2023, max compression
+gzip compressed data, was "merchantapi-2.6.0.tar", last modified: Mon Mar 11 21:44:55 2024, max compression
```

## Comparing `merchantapi-2.5.0.tar` & `merchantapi-2.6.0.tar`

### file list

```diff
@@ -1,925 +1,954 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.625175 merchantapi-2.5.0/
--rw-r--r--   0 root         (0) root         (0)     2165 2020-08-14 21:03:21.000000 merchantapi-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       89 2020-08-14 21:03:21.000000 merchantapi-2.5.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     3576 2023-08-01 21:53:39.625175 merchantapi-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2548 2023-08-01 21:53:38.000000 merchantapi-2.5.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.134180 merchantapi-2.5.0/merchantapi/
--rw-r--r--   0 root         (0) root         (0)      236 2020-08-14 21:03:21.000000 merchantapi-2.5.0/merchantapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8125 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/abstract.py
--rw-r--r--   0 root         (0) root         (0)    10877 2022-10-06 22:50:41.000000 merchantapi-2.5.0/merchantapi/authenticator.py
--rw-r--r--   0 root         (0) root         (0)    14390 2022-10-06 22:50:41.000000 merchantapi-2.5.0/merchantapi/client.py
--rw-r--r--   0 root         (0) root         (0)    30650 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/listquery.py
--rw-r--r--   0 root         (0) root         (0)     2876 2022-10-06 22:50:41.000000 merchantapi-2.5.0/merchantapi/logging.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.210179 merchantapi-2.5.0/merchantapi/model/
--rw-r--r--   0 root         (0) root         (0)     7433 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/model/all_order_payment.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/attribute_template.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/attribute_template_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-01-23 17:59:44.000000 merchantapi-2.5.0/merchantapi/model/attribute_template_option.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/attribute_template_product.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group_business_account.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group_category.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group_customer.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group_product.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/availability_group_shipping_method.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch_css_resource.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch_css_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      539 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch_javascript_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch_property_version.py
--rw-r--r--   0 root         (0) root         (0)     2551 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/branch_template_version.py
--rw-r--r--   0 root         (0) root         (0)     1599 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/business_account.py
--rw-r--r--   0 root         (0) root         (0)      586 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/business_account_customer.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/category.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/category_product.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/changeset.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/changeset_change.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/changeset_css_resource.py
--rw-r--r--   0 root         (0) root         (0)      506 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/changeset_css_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/changeset_javascript_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/changeset_property_version.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/changeset_template_version.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/copy_page_rule.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/copy_page_rules_settings.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/copy_product_rule.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/copy_product_rules_custom_field.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/copy_product_rules_module.py
--rw-r--r--   0 root         (0) root         (0)     1736 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/coupon.py
--rw-r--r--   0 root         (0) root         (0)      559 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/coupon_customer.py
--rw-r--r--   0 root         (0) root         (0)      572 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/coupon_price_group.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/css_resource.py
--rw-r--r--   0 root         (0) root         (0)      481 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/css_resource_attribute.py
--rw-r--r--   0 root         (0) root         (0)     6019 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/css_resource_change.py
--rw-r--r--   0 root         (0) root         (0)     5043 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/css_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/css_resource_version_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1632 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/custom_field_values.py
--rw-r--r--   0 root         (0) root         (0)     6761 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_address.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_address_list.py
--rw-r--r--   0 root         (0) root         (0)     1527 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_credit_history.py
--rw-r--r--   0 root         (0) root         (0)     2744 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_payment_card.py
--rw-r--r--   0 root         (0) root         (0)      578 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_price_group.py
--rw-r--r--   0 root         (0) root         (0)     7533 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/customer_subscription.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/discount_module_capabilities.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/image_type.py
--rw-r--r--   0 root         (0) root         (0)     2719 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/javascript_resource.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/javascript_resource_attribute.py
--rw-r--r--   0 root         (0) root         (0)     7145 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/javascript_resource_change.py
--rw-r--r--   0 root         (0) root         (0)     5176 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/javascript_resource_version.py
--rw-r--r--   0 root         (0) root         (0)      523 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/javascript_resource_version_attribute.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/kit_part.py
--rw-r--r--   0 root         (0) root         (0)      888 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/merchant_version.py
--rw-r--r--   0 root         (0) root         (0)     1435 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/module.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/module_change.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/note.py
--rw-r--r--   0 root         (0) root         (0)    16787 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_charge.py
--rw-r--r--   0 root         (0) root         (0)     1135 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_coupon.py
--rw-r--r--   0 root         (0) root         (0)     1728 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/order_custom_field.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_discount_total.py
--rw-r--r--   0 root         (0) root         (0)     9782 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/order_item.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_item_discount.py
--rw-r--r--   0 root         (0) root         (0)     5337 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_item_option.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_item_option_discount.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_item_subscription.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_note.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_part.py
--rw-r--r--   0 root         (0) root         (0)     3419 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/order_payment.py
--rw-r--r--   0 root         (0) root         (0)     1740 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_payment_authorize.py
--rw-r--r--   0 root         (0) root         (0)      476 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_payment_card.py
--rw-r--r--   0 root         (0) root         (0)     1731 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_payment_total.py
--rw-r--r--   0 root         (0) root         (0)      569 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_price_group.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_product.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_product_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_return.py
--rw-r--r--   0 root         (0) root         (0)     3404 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_shipment.py
--rw-r--r--   0 root         (0) root         (0)     2136 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_shipment_update.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_total.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/order_total_and_item.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/model/page.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/payment_card_type.py
--rw-r--r--   0 root         (0) root         (0)     3105 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/payment_method.py
--rw-r--r--   0 root         (0) root         (0)     5054 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group.py
--rw-r--r--   0 root         (0) root         (0)      614 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group_business_account.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group_category.py
--rw-r--r--   0 root         (0) root         (0)      571 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group_customer.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group_exclusion.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/price_group_product.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/print_queue.py
--rw-r--r--   0 root         (0) root         (0)     1750 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/print_queue_job.py
--rw-r--r--   0 root         (0) root         (0)    11554 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/product.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_and_subscription_term.py
--rw-r--r--   0 root         (0) root         (0)     4175 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_attribute.py
--rw-r--r--   0 root         (0) root         (0)     4763 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_attribute_list_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2312 2023-01-23 18:14:28.000000 merchantapi-2.5.0/merchantapi/model/product_attribute_list_option.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_attribute_list_template.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_image_data.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_inventory_adjustment.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_inventory_settings.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/model/product_kit.py
--rw-r--r--   0 root         (0) root         (0)      942 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_kit_part.py
--rw-r--r--   0 root         (0) root         (0)     2261 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_option.py
--rw-r--r--   0 root         (0) root         (0)      705 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_shipping_method.py
--rw-r--r--   0 root         (0) root         (0)     2120 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_shipping_rules.py
--rw-r--r--   0 root         (0) root         (0)     1964 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/product_subscription_settings.py
--rw-r--r--   0 root         (0) root         (0)     3084 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/model/product_subscription_term.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_subscription_term_date.py
--rw-r--r--   0 root         (0) root         (0)     3286 2023-01-23 17:59:16.000000 merchantapi-2.5.0/merchantapi/model/product_variant.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-01-23 17:59:16.000000 merchantapi-2.5.0/merchantapi/model/product_variant_attribute.py
--rw-r--r--   0 root         (0) root         (0)      980 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_variant_dimension.py
--rw-r--r--   0 root         (0) root         (0)     2664 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_variant_exclusion.py
--rw-r--r--   0 root         (0) root         (0)     2604 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_variant_limit.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/product_variant_part.py
--rw-r--r--   0 root         (0) root         (0)     5608 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/property_change.py
--rw-r--r--   0 root         (0) root         (0)     4669 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/property_version.py
--rw-r--r--   0 root         (0) root         (0)      904 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/provision_message.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/received_return.py
--rw-r--r--   0 root         (0) root         (0)     2598 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/model/related_product.py
--rw-r--r--   0 root         (0) root         (0)     1014 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/resource_attribute.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/model/resource_group.py
--rw-r--r--   0 root         (0) root         (0)     2520 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/resource_group_change.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-01-23 17:59:44.000000 merchantapi-2.5.0/merchantapi/model/split_order_item.py
--rw-r--r--   0 root         (0) root         (0)     5781 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/store.py
--rw-r--r--   0 root         (0) root         (0)     4957 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1409 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/subscription_attribute.py
--rw-r--r--   0 root         (0) root         (0)      943 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/subscription_option.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/subscription_shipping_method.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/template_change.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/uri.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/uri_detail.py
--rw-r--r--   0 root         (0) root         (0)     3581 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/variable_value.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/variant_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/model/variant_part.py
--rw-r--r--   0 root         (0) root         (0)     1760 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/model/version_settings.py
--rw-r--r--   0 root         (0) root         (0)    11905 2020-08-14 21:03:21.000000 merchantapi-2.5.0/merchantapi/multicall.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.342178 merchantapi-2.5.0/merchantapi/request/
--rw-r--r--   0 root         (0) root         (0)    16359 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/request/allorderpaymentlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4512 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_copylinkedtemplate.py
--rw-r--r--   0 root         (0) root         (0)     4734 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_copytemplate.py
--rw-r--r--   0 root         (0) root         (0)     4620 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_delete.py
--rw-r--r--   0 root         (0) root         (0)     6395 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_insert.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_load_code.py
--rw-r--r--   0 root         (0) root         (0)     8650 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attribute_update.py
--rw-r--r--   0 root         (0) root         (0)     3812 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributeandoptionlist_load_product.py
--rw-r--r--   0 root         (0) root         (0)     3696 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplate_delete.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplate_insert.py
--rw-r--r--   0 root         (0) root         (0)     4344 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplate_update.py
--rw-r--r--   0 root         (0) root         (0)     5864 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_delete.py
--rw-r--r--   0 root         (0) root         (0)     7585 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_insert.py
--rw-r--r--   0 root         (0) root         (0)     9930 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_update.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateattributelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplatelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     7811 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateoption_delete.py
--rw-r--r--   0 root         (0) root         (0)     8360 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateoption_insert.py
--rw-r--r--   0 root         (0) root         (0)     8596 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateoption_set_default.py
--rw-r--r--   0 root         (0) root         (0)    10367 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateoption_update.py
--rw-r--r--   0 root         (0) root         (0)     6066 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateoptionlist_load_attribute.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4816 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/attributetemplateproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroup_delete.py
--rw-r--r--   0 root         (0) root         (0)     2668 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroup_insert.py
--rw-r--r--   0 root         (0) root         (0)     4179 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroup_update.py
--rw-r--r--   0 root         (0) root         (0)     5557 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupbusinessaccount_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4762 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupbusinessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5657 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4622 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4622 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5753 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygrouppaymentmethod_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     6064 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4602 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5188 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupshippingmethod_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/availabilitygroupshippingmethodlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branch_copy.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branch_create.py
--rw-r--r--   0 root         (0) root         (0)     2473 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branch_delete.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branch_setprimary.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branch_update.py
--rw-r--r--   0 root         (0) root         (0)     4239 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchcssresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4351 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchjavascriptresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4257 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchpropertyversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/branchtemplateversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccount_insert.py
--rw-r--r--   0 root         (0) root         (0)     4258 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccount_update.py
--rw-r--r--   0 root         (0) root         (0)     5582 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccountcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4337 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccountcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccountlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1639 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/businessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/category_delete.py
--rw-r--r--   0 root         (0) root         (0)     5847 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/category_insert.py
--rw-r--r--   0 root         (0) root         (0)     6927 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/category_update.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categorylist_load_parent.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/categorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5350 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4049 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryuri_insert.py
--rw-r--r--   0 root         (0) root         (0)     3988 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryuri_redirect.py
--rw-r--r--   0 root         (0) root         (0)     2993 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryuri_update.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     3433 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/categoryurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)    15292 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/changeset_create.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/changesetchangelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2721 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesetcssresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesetjavascriptresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3159 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesetlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3421 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesetlist_merge.py
--rw-r--r--   0 root         (0) root         (0)     2783 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesetpropertyversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/changesettemplateversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4377 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/childcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5310 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypagerules_insert.py
--rw-r--r--   0 root         (0) root         (0)     6728 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypagerules_update.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypageruleslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypageruleslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypagerulessettings_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3690 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copypagerulessettingslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)    10348 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrules_insert.py
--rw-r--r--   0 root         (0) root         (0)    11892 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrules_update.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrulescustomfield_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4278 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrulescustomfieldlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2523 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductruleslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1491 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductruleslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3954 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrulesmodule_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/copyproductrulesmodulelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5419 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/coupon_insert.py
--rw-r--r--   0 root         (0) root         (0)     6387 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/coupon_update.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3860 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1641 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4461 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponpricegroup_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3971 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/couponpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3438 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/request/cssresource_delete.py
--rw-r--r--   0 root         (0) root         (0)     7037 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/cssresource_insert.py
--rw-r--r--   0 root         (0) root         (0)     8064 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/cssresource_update.py
--rw-r--r--   0 root         (0) root         (0)     1609 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/cssresourcelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2980 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customer_delete.py
--rw-r--r--   0 root         (0) root         (0)    20053 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/customer_insert.py
--rw-r--r--   0 root         (0) root         (0)    21188 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/customer_update.py
--rw-r--r--   0 root         (0) root         (0)     4110 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddress_delete.py
--rw-r--r--   0 root         (0) root         (0)     7779 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddress_insert.py
--rw-r--r--   0 root         (0) root         (0)     9527 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddress_update.py
--rw-r--r--   0 root         (0) root         (0)     3241 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddress_update_residential.py
--rw-r--r--   0 root         (0) root         (0)     4141 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddresslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customeraddresslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customercredithistory_delete.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customercredithistory_insert.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customercredithistorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2401 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     8073 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customerpaymentcard_register.py
--rw-r--r--   0 root         (0) root         (0)     3728 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customerpaymentcardlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/customerpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4278 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/customersubscriptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3178 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/feeduri_insert.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/feeduri_update.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/feedurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/feedurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/imagetypelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)    11654 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/inventoryproductsettings_update.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/request/javascriptresource_delete.py
--rw-r--r--   0 root         (0) root         (0)     8143 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/javascriptresource_insert.py
--rw-r--r--   0 root         (0) root         (0)     9959 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/javascriptresource_update.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/javascriptresourcelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/mivamerchantversion.py
--rw-r--r--   0 root         (0) root         (0)     2688 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/module.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/note_delete.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/note_insert.py
--rw-r--r--   0 root         (0) root         (0)     2215 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/note_update.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/notelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3146 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/option_delete.py
--rw-r--r--   0 root         (0) root         (0)     6830 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/option_insert.py
--rw-r--r--   0 root         (0) root         (0)     4822 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/option_load_code.py
--rw-r--r--   0 root         (0) root         (0)     3676 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/option_set_default.py
--rw-r--r--   0 root         (0) root         (0)     7929 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/option_update.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/optionlist_load_attribute.py
--rw-r--r--   0 root         (0) root         (0)     3689 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/order_authorize.py
--rw-r--r--   0 root         (0) root         (0)    19746 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/order_create.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/order_create_fromorder.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/order_delete.py
--rw-r--r--   0 root         (0) root         (0)    13752 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/order_update_customer_information.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/ordercoupon_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     2858 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/ordercouponlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1326 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/ordercustomfieldlist_load.py
--rw-r--r--   0 root         (0) root         (0)     2869 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/ordercustomfields_update.py
--rw-r--r--   0 root         (0) root         (0)     5562 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/orderitem_add.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitem_split.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/orderitem_update.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_backorder.py
--rw-r--r--   0 root         (0) root         (0)     3070 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_cancel.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_createreturn.py
--rw-r--r--   0 root         (0) root         (0)     2823 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_createshipment.py
--rw-r--r--   0 root         (0) root         (0)     2704 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderitemlist_removefromshipment.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/orderlist_archive.py
--rw-r--r--   0 root         (0) root         (0)     4234 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/orderlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderpayment_capture.py
--rw-r--r--   0 root         (0) root         (0)     2440 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderpayment_refund.py
--rw-r--r--   0 root         (0) root         (0)     2416 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderpayment_void.py
--rw-r--r--   0 root         (0) root         (0)     3489 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderpricegroup_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/orderpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/orderreturnlist_received.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/ordershipmentlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3263 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/ordershipmentlist_update.py
--rw-r--r--   0 root         (0) root         (0)     7376 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/request/page_copy.py
--rw-r--r--   0 root         (0) root         (0)     2770 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/request/page_delete.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/page_insert.py
--rw-r--r--   0 root         (0) root         (0)     6067 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/page_update.py
--rw-r--r--   0 root         (0) root         (0)     3256 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/pagelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3792 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pageuri_insert.py
--rw-r--r--   0 root         (0) root         (0)     3908 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pageuri_redirect.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pageuri_update.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pageurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     2814 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pageurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1984 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/paymentmethodlist_load.py
--rw-r--r--   0 root         (0) root         (0)     3152 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroup_delete.py
--rw-r--r--   0 root         (0) root         (0)    15796 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/pricegroup_insert.py
--rw-r--r--   0 root         (0) root         (0)    18126 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/pricegroup_update.py
--rw-r--r--   0 root         (0) root         (0)     5567 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupbusinessaccount_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4300 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupbusinessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5340 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4160 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3734 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5320 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupexcludedcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupexcludedcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5667 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupexcludedproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupexcludedproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5281 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3716 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     5302 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupqualifyingproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/pricegroupqualifyingproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/printqueuejob_delete.py
--rw-r--r--   0 root         (0) root         (0)     5003 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/printqueuejob_insert.py
--rw-r--r--   0 root         (0) root         (0)     2196 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/printqueuejob_status.py
--rw-r--r--   0 root         (0) root         (0)     3802 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/printqueuejoblist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/printqueuelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     6277 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/product_copy.py
--rw-r--r--   0 root         (0) root         (0)     3385 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/product_delete.py
--rw-r--r--   0 root         (0) root         (0)    10424 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/product_insert.py
--rw-r--r--   0 root         (0) root         (0)    11502 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/product_update.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productandsubscriptiontermlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productattributeandoptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productimage_add.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productimage_delete.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productimage_update_type.py
--rw-r--r--   0 root         (0) root         (0)     3685 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productkit_generate_variants.py
--rw-r--r--   0 root         (0) root         (0)     5884 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/productkit_update_parts.py
--rw-r--r--   0 root         (0) root         (0)     3029 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productkit_variant_count.py
--rw-r--r--   0 root         (0) root         (0)     3219 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productkitlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/productlist_adjust_inventory.py
--rw-r--r--   0 root         (0) root         (0)     2445 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/request/productlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productsubscriptiontermlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4005 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/producturi_insert.py
--rw-r--r--   0 root         (0) root         (0)     3968 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/producturi_redirect.py
--rw-r--r--   0 root         (0) root         (0)     2977 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/producturi_update.py
--rw-r--r--   0 root         (0) root         (0)     2122 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/producturilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     3272 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/producturilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     3692 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productvariant_generate.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productvariant_generate_delimiter.py
--rw-r--r--   0 root         (0) root         (0)     6104 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/productvariant_insert.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/productvariant_update.py
--rw-r--r--   0 root         (0) root         (0)     4016 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productvariantlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     7486 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/productvariantlist_load_product.py
--rw-r--r--   0 root         (0) root         (0)     3330 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/productvariantlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/provision_domain.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/provision_store.py
--rw-r--r--   0 root         (0) root         (0)     5167 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/relatedproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/relatedproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/request_builder.py
--rw-r--r--   0 root         (0) root         (0)     3764 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/resourcegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/store_load.py
--rw-r--r--   0 root         (0) root         (0)     1745 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/storelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     9931 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/subscription_insert.py
--rw-r--r--   0 root         (0) root         (0)    10781 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/subscription_update.py
--rw-r--r--   0 root         (0) root         (0)    10730 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/subscriptionandorderitem_add.py
--rw-r--r--   0 root         (0) root         (0)    11762 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/subscriptionandorderitem_update.py
--rw-r--r--   0 root         (0) root         (0)     2362 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/subscriptionlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/subscriptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)    10739 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/request/subscriptionshippingmethodlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1902 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/uri_delete.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/uri_insert.py
--rw-r--r--   0 root         (0) root         (0)     3738 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/uri_update.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/urilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/request/urilist_load_query.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.489176 merchantapi-2.5.0/merchantapi/response/
--rw-r--r--   0 root         (0) root         (0)    16359 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/response/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/allorderpaymentlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_copylinkedtemplate.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_copytemplate.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_delete.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_insert.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_load_code.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attribute_update.py
--rw-r--r--   0 root         (0) root         (0)     1273 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributeandoptionlist_load_product.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplate_delete.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplate_insert.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplate_update.py
--rw-r--r--   0 root         (0) root         (0)      868 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_delete.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_insert.py
--rw-r--r--   0 root         (0) root         (0)      868 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_update.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateattributelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplatelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateoption_delete.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateoption_insert.py
--rw-r--r--   0 root         (0) root         (0)      874 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateoption_set_default.py
--rw-r--r--   0 root         (0) root         (0)      856 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateoption_update.py
--rw-r--r--   0 root         (0) root         (0)     1428 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateoptionlist_load_attribute.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/attributetemplateproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroup_delete.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroup_insert.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroup_update.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupbusinessaccount_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1588 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupbusinessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygrouppaymentmethod_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      922 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupshippingmethod_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/availabilitygroupshippingmethodlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1061 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branch_copy.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branch_create.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branch_delete.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branch_setprimary.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branch_update.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branchcssresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/branchjavascriptresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branchlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branchlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branchpropertyversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/branchtemplateversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccount_insert.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccount_update.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccountcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccountcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccountlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/businessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/category_delete.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/category_insert.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/category_update.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categorylist_load_parent.py
--rw-r--r--   0 root         (0) root         (0)     1410 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1059 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryuri_insert.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryuri_redirect.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryuri_update.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/categoryurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changeset_create.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesetchangelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1566 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesetcssresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/changesetjavascriptresourceversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesetlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesetlist_merge.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesetpropertyversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/changesettemplateversionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1412 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/childcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1116 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypagerules_insert.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypagerules_update.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypageruleslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypageruleslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      882 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypagerulessettings_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1516 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copypagerulessettingslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrules_insert.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrules_update.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrulescustomfield_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrulescustomfieldlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      844 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductruleslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductruleslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrulesmodule_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1526 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/copyproductrulesmodulelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/coupon_insert.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/coupon_update.py
--rw-r--r--   0 root         (0) root         (0)      854 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1392 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponpricegroup_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/couponpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/cssresource_delete.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/cssresource_insert.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/cssresource_update.py
--rw-r--r--   0 root         (0) root         (0)     1434 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/cssresourcelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customer_delete.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customer_insert.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customer_update.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddress_delete.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddress_insert.py
--rw-r--r--   0 root         (0) root         (0)      824 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddress_update.py
--rw-r--r--   0 root         (0) root         (0)      870 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddress_update_residential.py
--rw-r--r--   0 root         (0) root         (0)      840 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddresslist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1468 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customeraddresslist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      848 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customercredithistory_delete.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customercredithistory_insert.py
--rw-r--r--   0 root         (0) root         (0)     1514 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customercredithistorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customerpaymentcard_register.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customerpaymentcardlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customerpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/customersubscriptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/feeduri_insert.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/feeduri_update.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/feedurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/feedurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1418 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/imagetypelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      860 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/inventoryproductsettings_update.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/javascriptresource_delete.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/javascriptresource_insert.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/javascriptresource_update.py
--rw-r--r--   0 root         (0) root         (0)     1490 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/javascriptresourcelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/mivamerchantversion.py
--rw-r--r--   0 root         (0) root         (0)      762 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/module.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/note_delete.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/note_insert.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/note_update.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/notelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/option_delete.py
--rw-r--r--   0 root         (0) root         (0)     1091 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/option_insert.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/option_load_code.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/option_set_default.py
--rw-r--r--   0 root         (0) root         (0)      788 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/option_update.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/optionlist_load_attribute.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/order_authorize.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/order_create.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/order_create_fromorder.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/order_delete.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/order_update_customer_information.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordercoupon_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1416 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordercouponlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordercustomfieldlist_load.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordercustomfields_update.py
--rw-r--r--   0 root         (0) root         (0)     1115 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitem_add.py
--rw-r--r--   0 root         (0) root         (0)     1106 2023-01-23 17:59:44.000000 merchantapi-2.5.0/merchantapi/response/orderitem_split.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitem_update.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_backorder.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_cancel.py
--rw-r--r--   0 root         (0) root         (0)     1133 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_createreturn.py
--rw-r--r--   0 root         (0) root         (0)     1151 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_createshipment.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_delete.py
--rw-r--r--   0 root         (0) root         (0)      864 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderitemlist_removefromshipment.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/response/orderlist_archive.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderpayment_capture.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderpayment_refund.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderpayment_void.py
--rw-r--r--   0 root         (0) root         (0)      858 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderpricegroup_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderpricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/orderreturnlist_received.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordershipmentlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/ordershipmentlist_update.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/page_copy.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/page_delete.py
--rw-r--r--   0 root         (0) root         (0)     1036 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/page_insert.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-01-24 22:24:13.000000 merchantapi-2.5.0/merchantapi/response/page_update.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/pagelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pageuri_insert.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pageuri_redirect.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pageuri_update.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pageurilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pageurilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/paymentmethodlist_load.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroup_delete.py
--rw-r--r--   0 root         (0) root         (0)     1092 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroup_insert.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroup_update.py
--rw-r--r--   0 root         (0) root         (0)      898 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupbusinessaccount_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupbusinessaccountlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      870 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      870 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupcustomer_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1474 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupcustomerlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      902 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupexcludedcategory_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1508 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupexcludedcategorylist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupexcludedproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupexcludedproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupqualifyingproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1506 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/pricegroupqualifyingproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/printqueuejob_delete.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/printqueuejob_insert.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/printqueuejob_status.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/printqueuejoblist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/printqueuelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-03-23 19:33:43.000000 merchantapi-2.5.0/merchantapi/response/product_copy.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/product_delete.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/product_insert.py
--rw-r--r--   0 root         (0) root         (0)      792 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/product_update.py
--rw-r--r--   0 root         (0) root         (0)     1540 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productandsubscriptiontermlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productattributeandoptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productimage_add.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productimage_delete.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productimage_update_type.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productkit_generate_variants.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productkit_update_parts.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productkit_variant_count.py
--rw-r--r--   0 root         (0) root         (0)     1426 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productkitlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productlist_adjust_inventory.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1532 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productsubscriptiontermlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/producturi_insert.py
--rw-r--r--   0 root         (0) root         (0)     1374 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/producturi_redirect.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/producturi_update.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/producturilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/producturilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariant_generate.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariant_generate_delimiter.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariant_insert.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariant_update.py
--rw-r--r--   0 root         (0) root         (0)      985 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariantlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariantlist_load_product.py
--rw-r--r--   0 root         (0) root         (0)     1458 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/productvariantlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/provision_domain.py
--rw-r--r--   0 root         (0) root         (0)     1195 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/provision_store.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/relatedproduct_update_assigned.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/relatedproductlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/request_builder.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/resourcegrouplist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/store_load.py
--rw-r--r--   0 root         (0) root         (0)     1384 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/storelist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscription_insert.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscription_update.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscriptionandorderitem_add.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscriptionandorderitem_update.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscriptionlist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscriptionlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/subscriptionshippingmethodlist_load_query.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/uri_delete.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/uri_insert.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/uri_update.py
--rw-r--r--   0 root         (0) root         (0)     1137 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/urilist_delete.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-01-19 18:57:56.000000 merchantapi-2.5.0/merchantapi/response/urilist_load_query.py
--rw-r--r--   0 root         (0) root         (0)     8727 2020-09-11 20:12:22.000000 merchantapi-2.5.0/merchantapi/sshagent.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-08-01 21:53:38.000000 merchantapi-2.5.0/merchantapi/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.135180 merchantapi-2.5.0/merchantapi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3576 2023-08-01 21:53:39.000000 merchantapi-2.5.0/merchantapi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    41392 2023-08-01 21:53:39.000000 merchantapi-2.5.0/merchantapi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-08-01 21:53:39.000000 merchantapi-2.5.0/merchantapi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2020-08-14 21:03:23.000000 merchantapi-2.5.0/merchantapi.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-08-01 21:53:39.000000 merchantapi-2.5.0/merchantapi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-08-01 21:53:39.000000 merchantapi-2.5.0/merchantapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-08-01 21:53:39.626175 merchantapi-2.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      911 2022-10-06 22:50:41.000000 merchantapi-2.5.0/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-08-01 21:53:39.625175 merchantapi-2.5.0/tests/
--rw-r--r--   0 root         (0) root         (0)      294 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1542 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/allorderpaymentlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      896 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_copylinkedtemplate_test.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_copytemplate_test.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_insert_test.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_load_code_test.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attribute_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributeandoptionlist_load_product_test.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplate_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1303 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplate_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplate_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1058 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateattribute_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1920 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateattribute_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1716 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateattribute_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1095 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateattributelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplatelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateoption_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateoption_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateoption_set_default_test.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateoption_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateoptionlist_load_attribute_test.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1173 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/attributetemplateproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroup_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1390 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroup_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1147 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroup_update_test.py
--rw-r--r--   0 root         (0) root         (0)     3516 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupbusinessaccount_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1461 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupbusinessaccountlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupcategory_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1397 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupcategorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     3188 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupcustomer_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupcustomerlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1183 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygrouppaymentmethod_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     3198 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupshippingmethod_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/availabilitygroupshippingmethodlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1327 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branch_copy_test.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branch_create_test.py
--rw-r--r--   0 root         (0) root         (0)     1132 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branch_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      986 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branch_setprimary_test.py
--rw-r--r--   0 root         (0) root         (0)     1000 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branch_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchcssresourceversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1305 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchjavascriptresourceversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchpropertyversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/branchtemplateversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccount_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccount_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccountcustomer_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1873 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccountcustomerlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1475 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccountlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      956 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/businessaccountlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/category_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     4192 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/category_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/category_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categorylist_load_parent_test.py
--rw-r--r--   0 root         (0) root         (0)     4623 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/categorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryuri_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1494 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryuri_redirect_test.py
--rw-r--r--   0 root         (0) root         (0)     1232 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryuri_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryurilist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1100 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/categoryurilist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2801 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/changeset_create_test.py
--rw-r--r--   0 root         (0) root         (0)     3839 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/changesetchangelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/changesetcssresourceversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/changesetjavascriptresourceversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      889 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/changesetlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2896 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/changesetlist_merge_test.py
--rw-r--r--   0 root         (0) root         (0)     1628 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/changesetpropertyversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/changesettemplateversionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/childcategorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)    18003 2022-10-06 22:50:41.000000 merchantapi-2.5.0/tests/client.py
--rw-r--r--   0 root         (0) root         (0)     1829 2020-08-14 21:03:21.000000 merchantapi-2.5.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypagerules_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypagerules_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypageruleslist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypageruleslist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypagerulessettings_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     3044 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copypagerulessettingslist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     3239 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrules_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     2859 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrules_update_test.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrulescustomfield_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrulescustomfieldlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1623 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductruleslist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      918 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductruleslist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2412 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrulesmodule_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/copyproductrulesmodulelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/coupon_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1039 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/coupon_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponcustomer_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponcustomerlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1098 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2953 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponpricegroup_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/couponpricegrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      613 2020-08-14 21:03:21.000000 merchantapi-2.5.0/tests/credentials.py.dist
--rw-r--r--   0 root         (0) root         (0)      878 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/cssresource_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     8818 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/cssresource_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/cssresource_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/cssresourcelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1138 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customer_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     8633 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customer_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customer_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddress_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     2760 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddress_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1429 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddress_update_residential_test.py
--rw-r--r--   0 root         (0) root         (0)     2764 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddress_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddresslist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customeraddresslist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customercredithistory_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customercredithistory_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customercredithistorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     4205 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customerlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1801 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customerpaymentcard_register_test.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customerpaymentcardlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customerpricegrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     3566 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/customersubscriptionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/feeduri_insert_test.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/feeduri_update_test.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/feedurilist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/feedurilist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)    34519 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/helper.py
--rw-r--r--   0 root         (0) root         (0)      900 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/imagetypelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/inventoryproductsettings_update_test.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/javascriptresource_delete_test.py
--rw-r--r--   0 root         (0) root         (0)    11011 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/javascriptresource_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/javascriptresource_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/javascriptresourcelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     8889 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/listquery.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/mivamerchantversion_test.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/module_test.py
--rw-r--r--   0 root         (0) root         (0)     3888 2020-09-11 20:12:22.000000 merchantapi-2.5.0/tests/multicall.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/note_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/note_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1453 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/note_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1449 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/notelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/option_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/option_insert_test.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/option_load_code_test.py
--rw-r--r--   0 root         (0) root         (0)     1347 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/option_set_default_test.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/option_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1101 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/optionlist_load_attribute_test.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/order_create_fromorder_test.py
--rw-r--r--   0 root         (0) root         (0)     7869 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/order_create_test.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/order_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/order_update_customer_information_test.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordercoupon_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1251 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordercouponlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordercustomfieldlist_load_test.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordercustomfields_update_test.py
--rw-r--r--   0 root         (0) root         (0)     5396 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitem_add_test.py
--rw-r--r--   0 root         (0) root         (0)     1333 2023-01-23 17:59:44.000000 merchantapi-2.5.0/tests/orderitem_split_test.py
--rw-r--r--   0 root         (0) root         (0)     2505 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitem_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_backorder_test.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_cancel_test.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_createreturn_test.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_createshipment_test.py
--rw-r--r--   0 root         (0) root         (0)     1708 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderitemlist_removefromshipment_test.py
--rw-r--r--   0 root         (0) root         (0)     1220 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/orderlist_archive_test.py
--rw-r--r--   0 root         (0) root         (0)     9388 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/orderlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2863 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderpricegroup_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/orderpricegrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1436 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordershipmentlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/ordershipmentlist_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/page_copy_test.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/page_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/page_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1351 2023-01-24 22:24:13.000000 merchantapi-2.5.0/tests/page_update_test.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/pagelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pageuri_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1342 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pageuri_redirect_test.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pageuri_update_test.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pageurilist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pageurilist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/paymentmethodlist_load_test.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroup_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     3853 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/pricegroup_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/pricegroup_update_test.py
--rw-r--r--   0 root         (0) root         (0)     2011 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupbusinessaccount_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1191 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupbusinessaccountlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupcategory_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupcategorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupcustomer_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupcustomerlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2016 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupexcludedcategory_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1192 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupexcludedcategorylist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupexcludedproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1181 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupexcludedproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2940 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupqualifyingproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1199 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/pricegroupqualifyingproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/printqueuejob_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/printqueuejob_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/printqueuejob_status_test.py
--rw-r--r--   0 root         (0) root         (0)     1386 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/printqueuejoblist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/printqueuelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/product_copy_test.py
--rw-r--r--   0 root         (0) root         (0)     2132 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/product_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/product_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/product_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productandsubscriptiontermlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productattributeandoptionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1848 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productimage_add_test.py
--rw-r--r--   0 root         (0) root         (0)     1193 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productimage_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1647 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productimage_update_type_test.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productkit_generate_variants_test.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productkit_update_parts_test.py
--rw-r--r--   0 root         (0) root         (0)      859 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productkit_variant_count_test.py
--rw-r--r--   0 root         (0) root         (0)      915 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productkitlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productlist_adjust_inventory_test.py
--rw-r--r--   0 root         (0) root         (0)     8918 2023-03-23 19:33:43.000000 merchantapi-2.5.0/tests/productlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productsubscriptiontermlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/producturi_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/producturi_redirect_test.py
--rw-r--r--   0 root         (0) root         (0)     1217 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/producturi_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/producturilist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1078 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/producturilist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productvariant_generate_delimiter_test.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productvariant_generate_test.py
--rw-r--r--   0 root         (0) root         (0)     3550 2023-01-23 17:59:16.000000 merchantapi-2.5.0/tests/productvariant_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     1813 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productvariant_update_test.py
--rw-r--r--   0 root         (0) root         (0)     1218 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productvariantlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1610 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/productvariantlist_load_product_test.py
--rw-r--r--   0 root         (0) root         (0)     1424 2023-01-23 17:59:16.000000 merchantapi-2.5.0/tests/productvariantlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2244 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/relatedproduct_update_assigned_test.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/relatedproductlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1960 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/request_builder_test.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/resourcegrouplist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-08-01 21:53:38.000000 merchantapi-2.5.0/tests/store_load_test.py
--rw-r--r--   0 root         (0) root         (0)      796 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/storelist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     3643 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscription_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     2488 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscription_update_test.py
--rw-r--r--   0 root         (0) root         (0)     4546 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscriptionandorderitem_add_test.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscriptionandorderitem_update_test.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscriptionlist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscriptionlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1842 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/subscriptionshippingmethodlist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/uri_delete_test.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/uri_insert_test.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/uri_update_test.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/urilist_delete_test.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/urilist_load_query_test.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-01-19 18:57:56.000000 merchantapi-2.5.0/tests/version_settings_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:55.568964 merchantapi-2.6.0/
+-rw-r-----   0 root         (0) root         (0)     2165 2020-08-14 17:25:38.000000 merchantapi-2.6.0/LICENSE
+-rw-r-----   0 root         (0) root         (0)       89 2020-08-14 17:25:38.000000 merchantapi-2.6.0/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-03-11 21:44:55.568964 merchantapi-2.6.0/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)     2548 2024-03-11 21:44:54.000000 merchantapi-2.6.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:54.965966 merchantapi-2.6.0/merchantapi/
+-rw-r-----   0 root         (0) root         (0)      236 2020-08-14 17:25:38.000000 merchantapi-2.6.0/merchantapi/__init__.py
+-rw-r-----   0 root         (0) root         (0)     8125 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/abstract.py
+-rw-r-----   0 root         (0) root         (0)    10877 2020-10-22 22:38:21.000000 merchantapi-2.6.0/merchantapi/authenticator.py
+-rw-r-----   0 root         (0) root         (0)    14390 2022-03-18 21:44:51.000000 merchantapi-2.6.0/merchantapi/client.py
+-rw-r-----   0 root         (0) root         (0)    30650 2023-06-14 21:26:20.000000 merchantapi-2.6.0/merchantapi/listquery.py
+-rw-r-----   0 root         (0) root         (0)     2876 2022-03-18 21:44:51.000000 merchantapi-2.6.0/merchantapi/logging.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:55.050966 merchantapi-2.6.0/merchantapi/model/
+-rw-r-----   0 root         (0) root         (0)     7704 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1125 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/all_order_payment.py
+-rw-r-----   0 root         (0) root         (0)      885 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/attribute_template.py
+-rw-r-----   0 root         (0) root         (0)     3405 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/attribute_template_attribute.py
+-rw-r-----   0 root         (0) root         (0)     2179 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/attribute_template_option.py
+-rw-r-----   0 root         (0) root         (0)      586 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/attribute_template_product.py
+-rw-r-----   0 root         (0) root         (0)      785 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group.py
+-rw-r-----   0 root         (0) root         (0)      635 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group_business_account.py
+-rw-r-----   0 root         (0) root         (0)      592 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group_category.py
+-rw-r-----   0 root         (0) root         (0)      592 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group_customer.py
+-rw-r-----   0 root         (0) root         (0)      586 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group_product.py
+-rw-r-----   0 root         (0) root         (0)      986 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/availability_group_shipping_method.py
+-rw-r-----   0 root         (0) root         (0)     1488 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch.py
+-rw-r-----   0 root         (0) root         (0)      454 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch_css_resource.py
+-rw-r-----   0 root         (0) root         (0)      497 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch_css_resource_version.py
+-rw-r-----   0 root         (0) root         (0)     1840 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/branch_item_version.py
+-rw-r-----   0 root         (0) root         (0)      539 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch_javascript_resource_version.py
+-rw-r-----   0 root         (0) root         (0)     3246 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/branch_page_version.py
+-rw-r-----   0 root         (0) root         (0)      478 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch_property_version.py
+-rw-r-----   0 root         (0) root         (0)     2551 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/branch_template_version.py
+-rw-r-----   0 root         (0) root         (0)     1599 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/business_account.py
+-rw-r-----   0 root         (0) root         (0)      586 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/business_account_customer.py
+-rw-r-----   0 root         (0) root         (0)     3654 2023-07-05 18:33:00.000000 merchantapi-2.6.0/merchantapi/model/category.py
+-rw-r-----   0 root         (0) root         (0)      559 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/category_product.py
+-rw-r-----   0 root         (0) root         (0)     1487 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/changeset.py
+-rw-r-----   0 root         (0) root         (0)     1501 2023-07-11 16:53:38.000000 merchantapi-2.6.0/merchantapi/model/changeset_change.py
+-rw-r-----   0 root         (0) root         (0)      463 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/changeset_css_resource.py
+-rw-r-----   0 root         (0) root         (0)      506 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/changeset_css_resource_version.py
+-rw-r-----   0 root         (0) root         (0)     1849 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/changeset_item_version.py
+-rw-r-----   0 root         (0) root         (0)      548 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/changeset_javascript_resource_version.py
+-rw-r-----   0 root         (0) root         (0)      487 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/changeset_property_version.py
+-rw-r-----   0 root         (0) root         (0)     2560 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/changeset_template_version.py
+-rw-r-----   0 root         (0) root         (0)     1779 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/copy_page_rule.py
+-rw-r-----   0 root         (0) root         (0)     1383 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/copy_page_rules_settings.py
+-rw-r-----   0 root         (0) root         (0)     2895 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/copy_product_rule.py
+-rw-r-----   0 root         (0) root         (0)     1561 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/copy_product_rules_custom_field.py
+-rw-r-----   0 root         (0) root         (0)     1298 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/copy_product_rules_module.py
+-rw-r-----   0 root         (0) root         (0)     1736 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/coupon.py
+-rw-r-----   0 root         (0) root         (0)      602 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/coupon_business_account.py
+-rw-r-----   0 root         (0) root         (0)      559 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/coupon_customer.py
+-rw-r-----   0 root         (0) root         (0)      572 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/coupon_price_group.py
+-rw-r-----   0 root         (0) root         (0)     2642 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/css_resource.py
+-rw-r-----   0 root         (0) root         (0)      481 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/css_resource_attribute.py
+-rw-r-----   0 root         (0) root         (0)     6019 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/css_resource_change.py
+-rw-r-----   0 root         (0) root         (0)     5043 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/css_resource_version.py
+-rw-r-----   0 root         (0) root         (0)      502 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/css_resource_version_attribute.py
+-rw-r-----   0 root         (0) root         (0)     1632 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/custom_field_values.py
+-rw-r-----   0 root         (0) root         (0)     6761 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer.py
+-rw-r-----   0 root         (0) root         (0)     2216 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_address.py
+-rw-r-----   0 root         (0) root         (0)     1576 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_address_list.py
+-rw-r-----   0 root         (0) root         (0)     1527 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_credit_history.py
+-rw-r-----   0 root         (0) root         (0)     2744 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_payment_card.py
+-rw-r-----   0 root         (0) root         (0)      578 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_price_group.py
+-rw-r-----   0 root         (0) root         (0)     7533 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/customer_subscription.py
+-rw-r-----   0 root         (0) root         (0)     1214 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/discount_module_capabilities.py
+-rw-r-----   0 root         (0) root         (0)      750 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/image_type.py
+-rw-r-----   0 root         (0) root         (0)     2719 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/javascript_resource.py
+-rw-r-----   0 root         (0) root         (0)      502 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/javascript_resource_attribute.py
+-rw-r-----   0 root         (0) root         (0)     7145 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/javascript_resource_change.py
+-rw-r-----   0 root         (0) root         (0)     5176 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/javascript_resource_version.py
+-rw-r-----   0 root         (0) root         (0)      523 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/javascript_resource_version_attribute.py
+-rw-r-----   0 root         (0) root         (0)      992 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/kit_part.py
+-rw-r-----   0 root         (0) root         (0)      888 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/merchant_version.py
+-rw-r-----   0 root         (0) root         (0)     1553 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/module.py
+-rw-r-----   0 root         (0) root         (0)     2103 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/model/module_change.py
+-rw-r-----   0 root         (0) root         (0)     1623 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/note.py
+-rw-r-----   0 root         (0) root         (0)    16787 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order.py
+-rw-r-----   0 root         (0) root         (0)     2862 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_charge.py
+-rw-r-----   0 root         (0) root         (0)     1135 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_coupon.py
+-rw-r-----   0 root         (0) root         (0)     1728 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/order_custom_field.py
+-rw-r-----   0 root         (0) root         (0)     1033 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_discount_total.py
+-rw-r-----   0 root         (0) root         (0)     9782 2023-07-05 18:33:00.000000 merchantapi-2.6.0/merchantapi/model/order_item.py
+-rw-r-----   0 root         (0) root         (0)     1169 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_item_discount.py
+-rw-r-----   0 root         (0) root         (0)     5337 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_item_option.py
+-rw-r-----   0 root         (0) root         (0)     1452 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_item_option_discount.py
+-rw-r-----   0 root         (0) root         (0)     1465 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_item_subscription.py
+-rw-r-----   0 root         (0) root         (0)      408 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_note.py
+-rw-r-----   0 root         (0) root         (0)     1110 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_part.py
+-rw-r-----   0 root         (0) root         (0)     3419 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/order_payment.py
+-rw-r-----   0 root         (0) root         (0)     1740 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_payment_authorize.py
+-rw-r-----   0 root         (0) root         (0)      476 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_payment_card.py
+-rw-r-----   0 root         (0) root         (0)     1731 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_payment_total.py
+-rw-r-----   0 root         (0) root         (0)      569 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_price_group.py
+-rw-r-----   0 root         (0) root         (0)     3972 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_product.py
+-rw-r-----   0 root         (0) root         (0)     1409 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_product_attribute.py
+-rw-r-----   0 root         (0) root         (0)     1242 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_return.py
+-rw-r-----   0 root         (0) root         (0)     3404 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_shipment.py
+-rw-r-----   0 root         (0) root         (0)     2136 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_shipment_update.py
+-rw-r-----   0 root         (0) root         (0)      683 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_total.py
+-rw-r-----   0 root         (0) root         (0)     1096 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/order_total_and_item.py
+-rw-r-----   0 root         (0) root         (0)     4095 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/page.py
+-rw-r-----   0 root         (0) root         (0)      991 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/payment_card_type.py
+-rw-r-----   0 root         (0) root         (0)     3105 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/payment_method.py
+-rw-r-----   0 root         (0) root         (0)     5054 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group.py
+-rw-r-----   0 root         (0) root         (0)      614 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group_business_account.py
+-rw-r-----   0 root         (0) root         (0)      571 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group_category.py
+-rw-r-----   0 root         (0) root         (0)      571 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group_customer.py
+-rw-r-----   0 root         (0) root         (0)     1137 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group_exclusion.py
+-rw-r-----   0 root         (0) root         (0)      565 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/price_group_product.py
+-rw-r-----   0 root         (0) root         (0)      647 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/print_queue.py
+-rw-r-----   0 root         (0) root         (0)     1750 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/print_queue_job.py
+-rw-r-----   0 root         (0) root         (0)    11669 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/product.py
+-rw-r-----   0 root         (0) root         (0)     1520 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_and_subscription_term.py
+-rw-r-----   0 root         (0) root         (0)     4175 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_attribute.py
+-rw-r-----   0 root         (0) root         (0)     4763 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_attribute_list_attribute.py
+-rw-r-----   0 root         (0) root         (0)     2312 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_attribute_list_option.py
+-rw-r-----   0 root         (0) root         (0)      925 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_attribute_list_template.py
+-rw-r-----   0 root         (0) root         (0)     1594 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_image_data.py
+-rw-r-----   0 root         (0) root         (0)     1906 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_inventory_adjustment.py
+-rw-r-----   0 root         (0) root         (0)     2458 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_inventory_settings.py
+-rw-r-----   0 root         (0) root         (0)     2450 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_kit.py
+-rw-r-----   0 root         (0) root         (0)      942 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_kit_part.py
+-rw-r-----   0 root         (0) root         (0)     2261 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_option.py
+-rw-r-----   0 root         (0) root         (0)      705 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_shipping_method.py
+-rw-r-----   0 root         (0) root         (0)     2120 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_shipping_rules.py
+-rw-r-----   0 root         (0) root         (0)     1964 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/product_subscription_settings.py
+-rw-r-----   0 root         (0) root         (0)     3084 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/product_subscription_term.py
+-rw-r-----   0 root         (0) root         (0)      860 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_subscription_term_date.py
+-rw-r-----   0 root         (0) root         (0)     3286 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant.py
+-rw-r-----   0 root         (0) root         (0)     1106 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant_attribute.py
+-rw-r-----   0 root         (0) root         (0)      980 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant_dimension.py
+-rw-r-----   0 root         (0) root         (0)     2664 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant_exclusion.py
+-rw-r-----   0 root         (0) root         (0)     2604 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant_limit.py
+-rw-r-----   0 root         (0) root         (0)     1193 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/product_variant_part.py
+-rw-r-----   0 root         (0) root         (0)     5608 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/property_change.py
+-rw-r-----   0 root         (0) root         (0)     4669 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/property_version.py
+-rw-r-----   0 root         (0) root         (0)      904 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/provision_message.py
+-rw-r-----   0 root         (0) root         (0)     1131 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/received_return.py
+-rw-r-----   0 root         (0) root         (0)     2598 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/related_product.py
+-rw-r-----   0 root         (0) root         (0)     1014 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/resource_attribute.py
+-rw-r-----   0 root         (0) root         (0)     2705 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/model/resource_group.py
+-rw-r-----   0 root         (0) root         (0)     2520 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/resource_group_change.py
+-rw-r-----   0 root         (0) root         (0)     1138 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/shipping_rule_method.py
+-rw-r-----   0 root         (0) root         (0)     1741 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/split_order_item.py
+-rw-r-----   0 root         (0) root         (0)     5781 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/model/store.py
+-rw-r-----   0 root         (0) root         (0)     4957 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/subscription.py
+-rw-r-----   0 root         (0) root         (0)     1409 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/subscription_attribute.py
+-rw-r-----   0 root         (0) root         (0)      943 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/subscription_option.py
+-rw-r-----   0 root         (0) root         (0)     1577 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/subscription_shipping_method.py
+-rw-r-----   0 root         (0) root         (0)     2656 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/template_change.py
+-rw-r-----   0 root         (0) root         (0)     4375 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/model/uri.py
+-rw-r-----   0 root         (0) root         (0)      740 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/uri_detail.py
+-rw-r-----   0 root         (0) root         (0)     3581 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/model/variable_value.py
+-rw-r-----   0 root         (0) root         (0)     2659 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/variant_attribute.py
+-rw-r-----   0 root         (0) root         (0)     1331 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/model/variant_part.py
+-rw-r-----   0 root         (0) root         (0)     1760 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/model/version_settings.py
+-rw-r-----   0 root         (0) root         (0)    11905 2020-08-14 17:25:38.000000 merchantapi-2.6.0/merchantapi/multicall.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:55.210965 merchantapi-2.6.0/merchantapi/request/
+-rw-r-----   0 root         (0) root         (0)    16951 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/__init__.py
+-rw-r-----   0 root         (0) root         (0)     2401 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/allorderpaymentlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4512 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_copylinkedtemplate.py
+-rw-r-----   0 root         (0) root         (0)     4734 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_copytemplate.py
+-rw-r-----   0 root         (0) root         (0)     4620 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_delete.py
+-rw-r-----   0 root         (0) root         (0)     6395 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_insert.py
+-rw-r-----   0 root         (0) root         (0)     3725 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_load_code.py
+-rw-r-----   0 root         (0) root         (0)     8650 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attribute_update.py
+-rw-r-----   0 root         (0) root         (0)     3812 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributeandoptionlist_load_product.py
+-rw-r-----   0 root         (0) root         (0)     3696 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplate_delete.py
+-rw-r-----   0 root         (0) root         (0)     2112 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplate_insert.py
+-rw-r-----   0 root         (0) root         (0)     4344 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplate_update.py
+-rw-r-----   0 root         (0) root         (0)     5864 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_delete.py
+-rw-r-----   0 root         (0) root         (0)     7585 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_insert.py
+-rw-r-----   0 root         (0) root         (0)     9930 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_update.py
+-rw-r-----   0 root         (0) root         (0)     4613 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateattributelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1567 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplatelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     7811 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateoption_delete.py
+-rw-r-----   0 root         (0) root         (0)     8360 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateoption_insert.py
+-rw-r-----   0 root         (0) root         (0)     8596 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateoption_set_default.py
+-rw-r-----   0 root         (0) root         (0)    10367 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateoption_update.py
+-rw-r-----   0 root         (0) root         (0)     6066 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateoptionlist_load_attribute.py
+-rw-r-----   0 root         (0) root         (0)     5707 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4816 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/attributetemplateproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3482 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroup_delete.py
+-rw-r-----   0 root         (0) root         (0)     2668 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroup_insert.py
+-rw-r-----   0 root         (0) root         (0)     4179 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroup_update.py
+-rw-r-----   0 root         (0) root         (0)     5557 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4762 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5657 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4622 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5707 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4622 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1515 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5753 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygrouppaymentmethod_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     6064 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4602 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5188 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupshippingmethod_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4772 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/availabilitygroupshippingmethodlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2883 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branch_copy.py
+-rw-r-----   0 root         (0) root         (0)     3431 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branch_create.py
+-rw-r-----   0 root         (0) root         (0)     2473 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branch_delete.py
+-rw-r-----   0 root         (0) root         (0)     2962 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branch_setprimary.py
+-rw-r-----   0 root         (0) root         (0)     3256 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branch_update.py
+-rw-r-----   0 root         (0) root         (0)     4239 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchcssresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3772 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/branchitemversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4351 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchjavascriptresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2146 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1517 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4008 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/branchpageversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4257 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchpropertyversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4094 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/branchtemplateversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2653 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccount_insert.py
+-rw-r-----   0 root         (0) root         (0)     4258 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccount_update.py
+-rw-r-----   0 root         (0) root         (0)     5582 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccountcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4337 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccountcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2486 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccountlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1639 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/businessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2965 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/category_delete.py
+-rw-r-----   0 root         (0) root         (0)     5847 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/category_insert.py
+-rw-r-----   0 root         (0) root         (0)     6927 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/category_update.py
+-rw-r-----   0 root         (0) root         (0)     2005 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categorylist_load_parent.py
+-rw-r-----   0 root         (0) root         (0)     1929 2023-07-05 18:33:00.000000 merchantapi-2.6.0/merchantapi/request/categorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5350 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4049 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4076 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryuri_insert.py
+-rw-r-----   0 root         (0) root         (0)     3988 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryuri_redirect.py
+-rw-r-----   0 root         (0) root         (0)     2993 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryuri_update.py
+-rw-r-----   0 root         (0) root         (0)     2134 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     3433 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/categoryurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)    15292 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/changeset_create.py
+-rw-r-----   0 root         (0) root         (0)     2493 2023-07-11 16:53:38.000000 merchantapi-2.6.0/merchantapi/request/changesetchangelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2721 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesetcssresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2522 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/changesetitemversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2791 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesetjavascriptresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3159 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesetlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3421 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesetlist_merge.py
+-rw-r-----   0 root         (0) root         (0)     2783 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesetpropertyversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2690 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/changesettemplateversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4377 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/childcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5310 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypagerules_insert.py
+-rw-r-----   0 root         (0) root         (0)     6728 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypagerules_update.py
+-rw-r-----   0 root         (0) root         (0)     2415 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypageruleslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1681 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypageruleslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3800 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypagerulessettings_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3690 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copypagerulessettingslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)    10348 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrules_insert.py
+-rw-r-----   0 root         (0) root         (0)    11892 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrules_update.py
+-rw-r-----   0 root         (0) root         (0)     4454 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrulescustomfield_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4278 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrulescustomfieldlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2523 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductruleslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1491 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductruleslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3954 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrulesmodule_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4134 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/copyproductrulesmodulelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5419 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/coupon_insert.py
+-rw-r-----   0 root         (0) root         (0)     6387 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/coupon_update.py
+-rw-r-----   0 root         (0) root         (0)     5322 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/couponbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4296 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/couponbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4926 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3860 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2146 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1641 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4461 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponpricegroup_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3971 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/couponpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3438 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/cssresource_delete.py
+-rw-r-----   0 root         (0) root         (0)     7037 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/cssresource_insert.py
+-rw-r-----   0 root         (0) root         (0)     8064 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/cssresource_update.py
+-rw-r-----   0 root         (0) root         (0)     1609 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/cssresourcelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2980 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customer_delete.py
+-rw-r-----   0 root         (0) root         (0)    20053 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/customer_insert.py
+-rw-r-----   0 root         (0) root         (0)    21188 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/customer_update.py
+-rw-r-----   0 root         (0) root         (0)     4110 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddress_delete.py
+-rw-r-----   0 root         (0) root         (0)     7779 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddress_insert.py
+-rw-r-----   0 root         (0) root         (0)     9527 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddress_update.py
+-rw-r-----   0 root         (0) root         (0)     3241 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddress_update_residential.py
+-rw-r-----   0 root         (0) root         (0)     4141 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddresslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     3627 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customeraddresslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2359 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customercredithistory_delete.py
+-rw-r-----   0 root         (0) root         (0)     4485 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customercredithistory_insert.py
+-rw-r-----   0 root         (0) root         (0)     3585 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customercredithistorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2401 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     8073 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customerpaymentcard_register.py
+-rw-r-----   0 root         (0) root         (0)     3728 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customerpaymentcardlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4124 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/customerpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4278 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/customersubscriptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3178 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/feeduri_insert.py
+-rw-r-----   0 root         (0) root         (0)     2929 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/feeduri_update.py
+-rw-r-----   0 root         (0) root         (0)     2086 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/feedurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     2375 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/feedurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1408 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/imagetypelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)    11654 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/inventoryproductsettings_update.py
+-rw-r-----   0 root         (0) root         (0)     3949 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/javascriptresource_delete.py
+-rw-r-----   0 root         (0) root         (0)     8143 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/javascriptresource_insert.py
+-rw-r-----   0 root         (0) root         (0)     9959 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/javascriptresource_update.py
+-rw-r-----   0 root         (0) root         (0)     1665 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/javascriptresourcelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1341 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/mivamerchantversion.py
+-rw-r-----   0 root         (0) root         (0)     2688 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/module.py
+-rw-r-----   0 root         (0) root         (0)     1821 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/note_delete.py
+-rw-r-----   0 root         (0) root         (0)     2869 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/note_insert.py
+-rw-r-----   0 root         (0) root         (0)     2215 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/note_update.py
+-rw-r-----   0 root         (0) root         (0)     1635 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/notelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3146 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/option_delete.py
+-rw-r-----   0 root         (0) root         (0)     6830 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/option_insert.py
+-rw-r-----   0 root         (0) root         (0)     4822 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/option_load_code.py
+-rw-r-----   0 root         (0) root         (0)     3676 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/option_set_default.py
+-rw-r-----   0 root         (0) root         (0)     7929 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/option_update.py
+-rw-r-----   0 root         (0) root         (0)     4975 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/optionlist_load_attribute.py
+-rw-r-----   0 root         (0) root         (0)     3689 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/order_authorize.py
+-rw-r-----   0 root         (0) root         (0)    19746 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/order_create.py
+-rw-r-----   0 root         (0) root         (0)     2001 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/order_create_fromorder.py
+-rw-r-----   0 root         (0) root         (0)     1851 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/order_delete.py
+-rw-r-----   0 root         (0) root         (0)    13752 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/order_update_customer_information.py
+-rw-r-----   0 root         (0) root         (0)     3739 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/ordercoupon_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     2858 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/ordercouponlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1326 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/ordercustomfieldlist_load.py
+-rw-r-----   0 root         (0) root         (0)     2869 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/ordercustomfields_update.py
+-rw-r-----   0 root         (0) root         (0)     5562 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/orderitem_add.py
+-rw-r-----   0 root         (0) root         (0)     2772 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitem_split.py
+-rw-r-----   0 root         (0) root         (0)     6546 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/orderitem_update.py
+-rw-r-----   0 root         (0) root         (0)     3256 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_backorder.py
+-rw-r-----   0 root         (0) root         (0)     3070 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_cancel.py
+-rw-r-----   0 root         (0) root         (0)     2845 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_createreturn.py
+-rw-r-----   0 root         (0) root         (0)     2823 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_createshipment.py
+-rw-r-----   0 root         (0) root         (0)     2704 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     2929 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderitemlist_removefromshipment.py
+-rw-r-----   0 root         (0) root         (0)     3213 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/orderlist_archive.py
+-rw-r-----   0 root         (0) root         (0)     4234 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/orderlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2452 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderpayment_capture.py
+-rw-r-----   0 root         (0) root         (0)     2440 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderpayment_refund.py
+-rw-r-----   0 root         (0) root         (0)     2416 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderpayment_void.py
+-rw-r-----   0 root         (0) root         (0)     3489 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderpricegroup_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     2972 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/orderpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2996 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/orderreturnlist_received.py
+-rw-r-----   0 root         (0) root         (0)     3739 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/ordershipmentlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3263 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/ordershipmentlist_update.py
+-rw-r-----   0 root         (0) root         (0)     7376 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/page_copy.py
+-rw-r-----   0 root         (0) root         (0)     6212 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/page_copy_branch.py
+-rw-r-----   0 root         (0) root         (0)     3967 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/page_delete.py
+-rw-r-----   0 root         (0) root         (0)     6927 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/page_insert.py
+-rw-r-----   0 root         (0) root         (0)     7264 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/page_update.py
+-rw-r-----   0 root         (0) root         (0)     3256 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/pagelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3792 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pageuri_insert.py
+-rw-r-----   0 root         (0) root         (0)     3908 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pageuri_redirect.py
+-rw-r-----   0 root         (0) root         (0)     2929 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pageuri_update.py
+-rw-r-----   0 root         (0) root         (0)     2086 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pageurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     2814 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pageurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1984 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/paymentmethodlist_load.py
+-rw-r-----   0 root         (0) root         (0)     3152 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroup_delete.py
+-rw-r-----   0 root         (0) root         (0)    15796 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/pricegroup_insert.py
+-rw-r-----   0 root         (0) root         (0)    18126 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/pricegroup_update.py
+-rw-r-----   0 root         (0) root         (0)     5567 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4300 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5340 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4160 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4682 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3734 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5320 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupexcludedcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4304 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupexcludedcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5667 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupexcludedproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4284 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupexcludedproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2141 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5281 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3716 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5302 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupqualifyingproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     4320 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/pricegroupqualifyingproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     2196 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/printqueuejob_delete.py
+-rw-r-----   0 root         (0) root         (0)     5003 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/printqueuejob_insert.py
+-rw-r-----   0 root         (0) root         (0)     2196 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/printqueuejob_status.py
+-rw-r-----   0 root         (0) root         (0)     3802 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/printqueuejoblist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1507 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/printqueuelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     6277 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/product_copy.py
+-rw-r-----   0 root         (0) root         (0)     3385 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/product_delete.py
+-rw-r-----   0 root         (0) root         (0)    10424 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/product_insert.py
+-rw-r-----   0 root         (0) root         (0)    11502 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/product_update.py
+-rw-r-----   0 root         (0) root         (0)     1494 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productandsubscriptiontermlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3966 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productattributeandoptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4162 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productimage_add.py
+-rw-r-----   0 root         (0) root         (0)     2107 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productimage_delete.py
+-rw-r-----   0 root         (0) root         (0)     2363 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productimage_update_type.py
+-rw-r-----   0 root         (0) root         (0)     3685 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productkit_generate_variants.py
+-rw-r-----   0 root         (0) root         (0)     5884 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/productkit_update_parts.py
+-rw-r-----   0 root         (0) root         (0)     3029 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productkit_variant_count.py
+-rw-r-----   0 root         (0) root         (0)     3219 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productkitlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3542 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/productlist_adjust_inventory.py
+-rw-r-----   0 root         (0) root         (0)     2445 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/request/productlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     7678 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/productshippingrules_update.py
+-rw-r-----   0 root         (0) root         (0)     3531 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productsubscriptiontermlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4005 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/producturi_insert.py
+-rw-r-----   0 root         (0) root         (0)     3968 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/producturi_redirect.py
+-rw-r-----   0 root         (0) root         (0)     2977 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/producturi_update.py
+-rw-r-----   0 root         (0) root         (0)     2122 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/producturilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     3272 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/producturilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     3692 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productvariant_generate.py
+-rw-r-----   0 root         (0) root         (0)     2080 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productvariant_generate_delimiter.py
+-rw-r-----   0 root         (0) root         (0)     6104 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/productvariant_insert.py
+-rw-r-----   0 root         (0) root         (0)     6546 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/productvariant_update.py
+-rw-r-----   0 root         (0) root         (0)     4016 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productvariantlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     7486 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/productvariantlist_load_product.py
+-rw-r-----   0 root         (0) root         (0)     3330 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/productvariantlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     5617 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/request/productvariantpricing_update.py
+-rw-r-----   0 root         (0) root         (0)     1742 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/provision_domain.py
+-rw-r-----   0 root         (0) root         (0)     1674 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/provision_store.py
+-rw-r-----   0 root         (0) root         (0)     5167 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/relatedproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     3980 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/relatedproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     4952 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/request_builder.py
+-rw-r-----   0 root         (0) root         (0)     3764 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/resourcegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1206 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/store_load.py
+-rw-r-----   0 root         (0) root         (0)     1745 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/storelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     9931 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/subscription_insert.py
+-rw-r-----   0 root         (0) root         (0)    10781 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/subscription_update.py
+-rw-r-----   0 root         (0) root         (0)    10730 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/subscriptionandorderitem_add.py
+-rw-r-----   0 root         (0) root         (0)    11762 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/subscriptionandorderitem_update.py
+-rw-r-----   0 root         (0) root         (0)     2362 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/subscriptionlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     3429 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/subscriptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)    10739 2023-07-17 20:14:29.000000 merchantapi-2.6.0/merchantapi/request/subscriptionshippingmethodlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1902 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/uri_delete.py
+-rw-r-----   0 root         (0) root         (0)     3246 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/uri_insert.py
+-rw-r-----   0 root         (0) root         (0)     3738 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/uri_update.py
+-rw-r-----   0 root         (0) root         (0)     2096 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/urilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1871 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/request/urilist_load_query.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:55.375964 merchantapi-2.6.0/merchantapi/response/
+-rw-r-----   0 root         (0) root         (0)    16951 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1450 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/allorderpaymentlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      848 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_copylinkedtemplate.py
+-rw-r-----   0 root         (0) root         (0)      824 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_copytemplate.py
+-rw-r-----   0 root         (0) root         (0)      800 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_delete.py
+-rw-r-----   0 root         (0) root         (0)     1118 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_insert.py
+-rw-r-----   0 root         (0) root         (0)     1128 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_load_code.py
+-rw-r-----   0 root         (0) root         (0)      800 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attribute_update.py
+-rw-r-----   0 root         (0) root         (0)     1273 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributeandoptionlist_load_product.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplate_delete.py
+-rw-r-----   0 root         (0) root         (0)     1155 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplate_insert.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplate_update.py
+-rw-r-----   0 root         (0) root         (0)      868 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_delete.py
+-rw-r-----   0 root         (0) root         (0)     1238 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_insert.py
+-rw-r-----   0 root         (0) root         (0)      868 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_update.py
+-rw-r-----   0 root         (0) root         (0)     1556 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateattributelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1482 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplatelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      856 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateoption_delete.py
+-rw-r-----   0 root         (0) root         (0)     1211 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateoption_insert.py
+-rw-r-----   0 root         (0) root         (0)      874 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateoption_set_default.py
+-rw-r-----   0 root         (0) root         (0)      856 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateoption_update.py
+-rw-r-----   0 root         (0) root         (0)     1428 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateoptionlist_load_attribute.py
+-rw-r-----   0 root         (0) root         (0)      894 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1522 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/attributetemplateproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroup_delete.py
+-rw-r-----   0 root         (0) root         (0)     1155 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroup_insert.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroup_update.py
+-rw-r-----   0 root         (0) root         (0)      926 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1588 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      898 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1532 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      898 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1530 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1482 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      918 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygrouppaymentmethod_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)      894 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1522 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      922 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupshippingmethod_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1598 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/availabilitygroupshippingmethodlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1061 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branch_copy.py
+-rw-r-----   0 root         (0) root         (0)     1054 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branch_create.py
+-rw-r-----   0 root         (0) root         (0)      788 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branch_delete.py
+-rw-r-----   0 root         (0) root         (0)      804 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branch_setprimary.py
+-rw-r-----   0 root         (0) root         (0)      788 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branch_update.py
+-rw-r-----   0 root         (0) root         (0)     1542 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branchcssresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1484 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/branchitemversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1761 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/branchjavascriptresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      953 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branchlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1394 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branchlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1484 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/branchpageversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1516 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branchpropertyversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1516 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/branchtemplateversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1137 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccount_insert.py
+-rw-r-----   0 root         (0) root         (0)      824 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccount_update.py
+-rw-r-----   0 root         (0) root         (0)      890 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccountcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1514 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccountcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      989 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccountlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1466 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/businessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      796 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/category_delete.py
+-rw-r-----   0 root         (0) root         (0)     1072 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/category_insert.py
+-rw-r-----   0 root         (0) root         (0)      796 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/category_update.py
+-rw-r-----   0 root         (0) root         (0)     1197 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categorylist_load_parent.py
+-rw-r-----   0 root         (0) root         (0)     1410 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      858 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1448 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1059 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryuri_insert.py
+-rw-r-----   0 root         (0) root         (0)     1378 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryuri_redirect.py
+-rw-r-----   0 root         (0) root         (0)      808 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryuri_update.py
+-rw-r-----   0 root         (0) root         (0)     1169 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1400 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/categoryurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1081 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changeset_create.py
+-rw-r-----   0 root         (0) root         (0)     1466 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesetchangelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1566 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesetcssresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1508 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/changesetitemversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1794 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/changesetjavascriptresourceversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1416 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesetlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1093 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesetlist_merge.py
+-rw-r-----   0 root         (0) root         (0)     1540 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesetpropertyversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1540 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/changesettemplateversionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1412 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/childcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1116 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypagerules_insert.py
+-rw-r-----   0 root         (0) root         (0)      816 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypagerules_update.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypageruleslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1448 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypageruleslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      882 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypagerulessettings_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1516 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copypagerulessettingslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1143 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrules_insert.py
+-rw-r-----   0 root         (0) root         (0)      828 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrules_update.py
+-rw-r-----   0 root         (0) root         (0)      906 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrulescustomfield_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1568 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrulescustomfieldlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      844 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductruleslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1472 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductruleslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      886 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrulesmodule_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1526 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/copyproductrulesmodulelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1054 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/coupon_insert.py
+-rw-r-----   0 root         (0) root         (0)      788 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/coupon_update.py
+-rw-r-----   0 root         (0) root         (0)      882 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/couponbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1516 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/couponbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      854 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1440 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      953 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1392 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      862 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponpricegroup_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1458 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/couponpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      808 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/cssresource_delete.py
+-rw-r-----   0 root         (0) root         (0)     1101 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/cssresource_insert.py
+-rw-r-----   0 root         (0) root         (0)      808 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/cssresource_update.py
+-rw-r-----   0 root         (0) root         (0)     1434 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/cssresourcelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      796 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customer_delete.py
+-rw-r-----   0 root         (0) root         (0)     1072 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customer_insert.py
+-rw-r-----   0 root         (0) root         (0)      796 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customer_update.py
+-rw-r-----   0 root         (0) root         (0)      824 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddress_delete.py
+-rw-r-----   0 root         (0) root         (0)     1137 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddress_insert.py
+-rw-r-----   0 root         (0) root         (0)      824 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddress_update.py
+-rw-r-----   0 root         (0) root         (0)      870 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddress_update_residential.py
+-rw-r-----   0 root         (0) root         (0)      840 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddresslist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1468 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customeraddresslist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      848 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customercredithistory_delete.py
+-rw-r-----   0 root         (0) root         (0)     1193 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customercredithistory_insert.py
+-rw-r-----   0 root         (0) root         (0)     1514 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customercredithistorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1408 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1183 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customerpaymentcard_register.py
+-rw-r-----   0 root         (0) root         (0)     1500 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customerpaymentcardlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1474 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customerpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1488 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/customersubscriptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1043 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/feeduri_insert.py
+-rw-r-----   0 root         (0) root         (0)      792 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/feeduri_update.py
+-rw-r-----   0 root         (0) root         (0)     1153 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/feedurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1384 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/feedurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1418 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/imagetypelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      860 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/inventoryproductsettings_update.py
+-rw-r-----   0 root         (0) root         (0)      836 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/javascriptresource_delete.py
+-rw-r-----   0 root         (0) root         (0)     1164 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/javascriptresource_insert.py
+-rw-r-----   0 root         (0) root         (0)      836 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/javascriptresource_update.py
+-rw-r-----   0 root         (0) root         (0)     1490 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/javascriptresourcelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1127 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/mivamerchantversion.py
+-rw-r-----   0 root         (0) root         (0)      762 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/module.py
+-rw-r-----   0 root         (0) root         (0)      780 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/note_delete.py
+-rw-r-----   0 root         (0) root         (0)     1036 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/note_insert.py
+-rw-r-----   0 root         (0) root         (0)      780 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/note_update.py
+-rw-r-----   0 root         (0) root         (0)     1376 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/notelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      788 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/option_delete.py
+-rw-r-----   0 root         (0) root         (0)     1091 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/option_insert.py
+-rw-r-----   0 root         (0) root         (0)     1101 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/option_load_code.py
+-rw-r-----   0 root         (0) root         (0)      806 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/option_set_default.py
+-rw-r-----   0 root         (0) root         (0)      788 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/option_update.py
+-rw-r-----   0 root         (0) root         (0)     1221 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/optionlist_load_attribute.py
+-rw-r-----   0 root         (0) root         (0)     1141 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/order_authorize.py
+-rw-r-----   0 root         (0) root         (0)     1045 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/order_create.py
+-rw-r-----   0 root         (0) root         (0)     1083 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/order_create_fromorder.py
+-rw-r-----   0 root         (0) root         (0)      784 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/order_delete.py
+-rw-r-----   0 root         (0) root         (0)      864 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/order_update_customer_information.py
+-rw-r-----   0 root         (0) root         (0)      842 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordercoupon_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1416 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordercouponlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1237 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordercustomfieldlist_load.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordercustomfields_update.py
+-rw-r-----   0 root         (0) root         (0)     1115 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitem_add.py
+-rw-r-----   0 root         (0) root         (0)     1106 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitem_split.py
+-rw-r-----   0 root         (0) root         (0)     1088 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitem_update.py
+-rw-r-----   0 root         (0) root         (0)      828 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_backorder.py
+-rw-r-----   0 root         (0) root         (0)      816 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_cancel.py
+-rw-r-----   0 root         (0) root         (0)     1133 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_createreturn.py
+-rw-r-----   0 root         (0) root         (0)     1151 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_createshipment.py
+-rw-r-----   0 root         (0) root         (0)      816 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_delete.py
+-rw-r-----   0 root         (0) root         (0)      864 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderitemlist_removefromshipment.py
+-rw-r-----   0 root         (0) root         (0)      953 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/orderlist_archive.py
+-rw-r-----   0 root         (0) root         (0)     1384 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1141 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderpayment_capture.py
+-rw-r-----   0 root         (0) root         (0)     1137 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderpayment_refund.py
+-rw-r-----   0 root         (0) root         (0)     1129 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderpayment_void.py
+-rw-r-----   0 root         (0) root         (0)      858 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderpricegroup_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1450 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderpricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/orderreturnlist_received.py
+-rw-r-----   0 root         (0) root         (0)     1450 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordershipmentlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      832 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/ordershipmentlist_update.py
+-rw-r-----   0 root         (0) root         (0)     1028 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/page_copy.py
+-rw-r-----   0 root         (0) root         (0)     1054 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/page_copy_branch.py
+-rw-r-----   0 root         (0) root         (0)      780 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/page_delete.py
+-rw-r-----   0 root         (0) root         (0)     1036 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/page_insert.py
+-rw-r-----   0 root         (0) root         (0)      780 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/page_update.py
+-rw-r-----   0 root         (0) root         (0)     1376 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/pagelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1043 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pageuri_insert.py
+-rw-r-----   0 root         (0) root         (0)     1362 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pageuri_redirect.py
+-rw-r-----   0 root         (0) root         (0)      792 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pageuri_update.py
+-rw-r-----   0 root         (0) root         (0)     1153 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pageurilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1384 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pageurilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1211 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/paymentmethodlist_load.py
+-rw-r-----   0 root         (0) root         (0)      804 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroup_delete.py
+-rw-r-----   0 root         (0) root         (0)     1092 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroup_insert.py
+-rw-r-----   0 root         (0) root         (0)      804 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroup_update.py
+-rw-r-----   0 root         (0) root         (0)      898 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupbusinessaccount_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1532 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupbusinessaccountlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      870 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1476 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      870 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupcustomer_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1474 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupcustomerlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      902 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupexcludedcategory_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1508 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupexcludedcategorylist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1303 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupexcludedproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1498 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupexcludedproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1426 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      866 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1466 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      906 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupqualifyingproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1506 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/pricegroupqualifyingproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      816 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/printqueuejob_delete.py
+-rw-r-----   0 root         (0) root         (0)     1121 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/printqueuejob_insert.py
+-rw-r-----   0 root         (0) root         (0)      999 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/printqueuejob_status.py
+-rw-r-----   0 root         (0) root         (0)     1452 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/printqueuejoblist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1426 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/printqueuelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1453 2023-03-23 19:33:09.000000 merchantapi-2.6.0/merchantapi/response/product_copy.py
+-rw-r-----   0 root         (0) root         (0)      792 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/product_delete.py
+-rw-r-----   0 root         (0) root         (0)     1063 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/product_insert.py
+-rw-r-----   0 root         (0) root         (0)      792 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/product_update.py
+-rw-r-----   0 root         (0) root         (0)     1540 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productandsubscriptiontermlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1520 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productattributeandoptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1120 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productimage_add.py
+-rw-r-----   0 root         (0) root         (0)      812 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productimage_delete.py
+-rw-r-----   0 root         (0) root         (0)      830 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productimage_update_type.py
+-rw-r-----   0 root         (0) root         (0)      846 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productkit_generate_variants.py
+-rw-r-----   0 root         (0) root         (0)      826 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productkit_update_parts.py
+-rw-r-----   0 root         (0) root         (0)     1015 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productkit_variant_count.py
+-rw-r-----   0 root         (0) root         (0)     1426 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productkitlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      846 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productlist_adjust_inventory.py
+-rw-r-----   0 root         (0) root         (0)     1400 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      844 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/productshippingrules_update.py
+-rw-r-----   0 root         (0) root         (0)     1532 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productsubscriptiontermlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1055 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/producturi_insert.py
+-rw-r-----   0 root         (0) root         (0)     1374 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/producturi_redirect.py
+-rw-r-----   0 root         (0) root         (0)      804 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/producturi_update.py
+-rw-r-----   0 root         (0) root         (0)     1165 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/producturilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1396 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/producturilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      828 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariant_generate.py
+-rw-r-----   0 root         (0) root         (0)      940 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariant_generate_delimiter.py
+-rw-r-----   0 root         (0) root         (0)     1128 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariant_insert.py
+-rw-r-----   0 root         (0) root         (0)      820 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariant_update.py
+-rw-r-----   0 root         (0) root         (0)      985 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariantlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1249 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariantlist_load_product.py
+-rw-r-----   0 root         (0) root         (0)     1458 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/productvariantlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      848 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/response/productvariantpricing_update.py
+-rw-r-----   0 root         (0) root         (0)     1199 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/provision_domain.py
+-rw-r-----   0 root         (0) root         (0)     1195 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/provision_store.py
+-rw-r-----   0 root         (0) root         (0)     1245 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/relatedproduct_update_assigned.py
+-rw-r-----   0 root         (0) root         (0)     1440 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/relatedproductlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      425 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/request_builder.py
+-rw-r-----   0 root         (0) root         (0)     1450 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/resourcegrouplist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1037 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/store_load.py
+-rw-r-----   0 root         (0) root         (0)     1384 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/storelist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1108 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscription_insert.py
+-rw-r-----   0 root         (0) root         (0)     1108 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscription_update.py
+-rw-r-----   0 root         (0) root         (0)     1175 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscriptionandorderitem_add.py
+-rw-r-----   0 root         (0) root         (0)     1148 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscriptionandorderitem_update.py
+-rw-r-----   0 root         (0) root         (0)      828 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscriptionlist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1440 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscriptionlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     1556 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/subscriptionshippingmethodlist_load_query.py
+-rw-r-----   0 root         (0) root         (0)      776 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/uri_delete.py
+-rw-r-----   0 root         (0) root         (0)     1027 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/uri_insert.py
+-rw-r-----   0 root         (0) root         (0)      776 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/uri_update.py
+-rw-r-----   0 root         (0) root         (0)     1137 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/urilist_delete.py
+-rw-r-----   0 root         (0) root         (0)     1368 2023-01-24 22:23:48.000000 merchantapi-2.6.0/merchantapi/response/urilist_load_query.py
+-rw-r-----   0 root         (0) root         (0)     8727 2020-09-03 18:52:42.000000 merchantapi-2.6.0/merchantapi/sshagent.py
+-rw-r-----   0 root         (0) root         (0)      390 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:54.966966 merchantapi-2.6.0/merchantapi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3576 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    42846 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2020-08-14 17:25:40.000000 merchantapi-2.6.0/merchantapi.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-11 21:44:54.000000 merchantapi-2.6.0/merchantapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-11 21:44:55.568964 merchantapi-2.6.0/setup.cfg
+-rw-r-----   0 root         (0) root         (0)      911 2020-10-22 22:38:21.000000 merchantapi-2.6.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-11 21:44:55.567964 merchantapi-2.6.0/tests/
+-rw-r-----   0 root         (0) root         (0)      294 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1542 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/allorderpaymentlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      896 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_copylinkedtemplate_test.py
+-rw-r-----   0 root         (0) root         (0)     1027 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_copytemplate_test.py
+-rw-r-----   0 root         (0) root         (0)      915 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1367 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_insert_test.py
+-rw-r-----   0 root         (0) root         (0)      924 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_load_code_test.py
+-rw-r-----   0 root         (0) root         (0)     1030 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attribute_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1303 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributeandoptionlist_load_product_test.py
+-rw-r-----   0 root         (0) root         (0)      924 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplate_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1303 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplate_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1190 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplate_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1058 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateattribute_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1920 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateattribute_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1716 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateattribute_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1095 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateattributelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1023 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplatelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1113 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateoption_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1753 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateoption_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1386 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateoption_set_default_test.py
+-rw-r-----   0 root         (0) root         (0)     1492 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateoption_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1174 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateoptionlist_load_attribute_test.py
+-rw-r-----   0 root         (0) root         (0)     2984 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1173 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/attributetemplateproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1023 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroup_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1390 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroup_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1147 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroup_update_test.py
+-rw-r-----   0 root         (0) root         (0)     3516 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupbusinessaccount_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1461 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupbusinessaccountlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1950 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupcategory_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1397 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupcategorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     3188 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupcustomer_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1399 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupcustomerlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1183 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2761 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygrouppaymentmethod_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     3198 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1393 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2975 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupshippingmethod_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1438 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/availabilitygroupshippingmethodlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1327 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branch_copy_test.py
+-rw-r-----   0 root         (0) root         (0)      944 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branch_create_test.py
+-rw-r-----   0 root         (0) root         (0)     1132 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branch_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      986 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branch_setprimary_test.py
+-rw-r-----   0 root         (0) root         (0)     1000 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branch_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1242 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchcssresourceversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1438 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/branchitemversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1305 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchjavascriptresourceversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1197 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      809 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1377 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/branchpageversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1212 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchpropertyversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1031 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/branchtemplateversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1360 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccount_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1189 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccount_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1954 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccountcustomer_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1873 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccountcustomerlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1475 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccountlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      956 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/businessaccountlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1122 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/category_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     4192 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/category_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1199 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/category_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1346 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categorylist_load_parent_test.py
+-rw-r-----   0 root         (0) root         (0)     4623 2023-07-05 18:33:00.000000 merchantapi-2.6.0/tests/categorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2904 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1239 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1227 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryuri_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1494 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryuri_redirect_test.py
+-rw-r-----   0 root         (0) root         (0)     1232 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryuri_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1082 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryurilist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1100 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/categoryurilist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2801 2023-07-17 20:14:29.000000 merchantapi-2.6.0/tests/changeset_create_test.py
+-rw-r-----   0 root         (0) root         (0)     3839 2023-07-11 16:53:38.000000 merchantapi-2.6.0/tests/changesetchangelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2104 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/changesetcssresourceversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1933 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/changesetitemversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2417 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/changesetjavascriptresourceversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      889 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/changesetlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2896 2023-07-17 20:14:29.000000 merchantapi-2.6.0/tests/changesetlist_merge_test.py
+-rw-r-----   0 root         (0) root         (0)     1628 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/changesetpropertyversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1820 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/changesettemplateversionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2314 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/childcategorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)    18003 2020-10-22 22:38:21.000000 merchantapi-2.6.0/tests/client.py
+-rw-r-----   0 root         (0) root         (0)     1829 2020-08-14 17:25:38.000000 merchantapi-2.6.0/tests/conftest.py
+-rw-r-----   0 root         (0) root         (0)     1667 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypagerules_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1590 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypagerules_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1561 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypageruleslist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      892 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypageruleslist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2465 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypagerulessettings_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     3044 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copypagerulessettingslist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     3239 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrules_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2859 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrules_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2735 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrulescustomfield_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     3042 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrulescustomfieldlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1623 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductruleslist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      918 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductruleslist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2412 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrulesmodule_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     2431 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/copyproductrulesmodulelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     4473 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/coupon_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1039 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/coupon_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2908 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/couponbusinessaccountList_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1706 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/couponbusinessaccount_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1872 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponcustomer_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1108 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponcustomerlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1130 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1098 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2953 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponpricegroup_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1257 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/couponpricegrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      613 2020-08-14 17:25:38.000000 merchantapi-2.6.0/tests/credentials.py.dist
+-rw-r-----   0 root         (0) root         (0)      878 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/cssresource_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     8818 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/cssresource_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2332 2023-07-17 20:14:29.000000 merchantapi-2.6.0/tests/cssresource_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1004 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/cssresourcelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1138 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customer_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     8633 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customer_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     3169 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customer_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1221 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddress_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     2760 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddress_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1429 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddress_update_residential_test.py
+-rw-r-----   0 root         (0) root         (0)     2764 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddress_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1125 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddresslist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     2425 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customeraddresslist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1729 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customercredithistory_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1044 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customercredithistory_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1634 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customercredithistorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     4205 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customerlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1801 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customerpaymentcard_register_test.py
+-rw-r-----   0 root         (0) root         (0)     2244 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customerpaymentcardlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1601 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customerpricegrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     3566 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/customersubscriptionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1067 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/feeduri_insert_test.py
+-rw-r-----   0 root         (0) root         (0)      959 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/feeduri_update_test.py
+-rw-r-----   0 root         (0) root         (0)      974 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/feedurilist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      839 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/feedurilist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)    36953 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/helper.py
+-rw-r-----   0 root         (0) root         (0)      900 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/imagetypelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2355 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/inventoryproductsettings_update_test.py
+-rw-r-----   0 root         (0) root         (0)      955 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/javascriptresource_delete_test.py
+-rw-r-----   0 root         (0) root         (0)    11011 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/javascriptresource_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2578 2023-07-17 20:14:29.000000 merchantapi-2.6.0/tests/javascriptresource_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1081 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/javascriptresourcelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     8889 2023-06-14 21:26:20.000000 merchantapi-2.6.0/tests/listquery.py
+-rw-r-----   0 root         (0) root         (0)     1176 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/mivamerchantversion_test.py
+-rw-r-----   0 root         (0) root         (0)      693 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/module_test.py
+-rw-r-----   0 root         (0) root         (0)     3888 2020-09-03 18:52:42.000000 merchantapi-2.6.0/tests/multicall.py
+-rw-r-----   0 root         (0) root         (0)     1312 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/note_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     2334 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/note_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1453 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/note_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1449 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/notelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1119 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/option_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1752 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/option_insert_test.py
+-rw-r-----   0 root         (0) root         (0)      966 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/option_load_code_test.py
+-rw-r-----   0 root         (0) root         (0)     1347 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/option_set_default_test.py
+-rw-r-----   0 root         (0) root         (0)     1283 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/option_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1101 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/optionlist_load_attribute_test.py
+-rw-r-----   0 root         (0) root         (0)     1386 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/order_create_fromorder_test.py
+-rw-r-----   0 root         (0) root         (0)     7869 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/order_create_test.py
+-rw-r-----   0 root         (0) root         (0)     1042 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/order_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     3177 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/order_update_customer_information_test.py
+-rw-r-----   0 root         (0) root         (0)     2736 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordercoupon_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1251 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordercouponlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      996 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordercustomfieldlist_load_test.py
+-rw-r-----   0 root         (0) root         (0)     1159 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordercustomfields_update_test.py
+-rw-r-----   0 root         (0) root         (0)     5396 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitem_add_test.py
+-rw-r-----   0 root         (0) root         (0)     1333 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitem_split_test.py
+-rw-r-----   0 root         (0) root         (0)     2505 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitem_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1953 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_backorder_test.py
+-rw-r-----   0 root         (0) root         (0)     2129 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_cancel_test.py
+-rw-r-----   0 root         (0) root         (0)     3500 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_createreturn_test.py
+-rw-r-----   0 root         (0) root         (0)     1766 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_createshipment_test.py
+-rw-r-----   0 root         (0) root         (0)     1708 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1308 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderitemlist_removefromshipment_test.py
+-rw-r-----   0 root         (0) root         (0)     1220 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/orderlist_archive_test.py
+-rw-r-----   0 root         (0) root         (0)     9388 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/orderlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2863 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderpricegroup_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1283 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/orderpricegrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1436 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordershipmentlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      993 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/ordershipmentlist_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1918 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/page_copy_branch_test.py
+-rw-r-----   0 root         (0) root         (0)     1649 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/page_copy_test.py
+-rw-r-----   0 root         (0) root         (0)     1503 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/page_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     3286 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/page_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2556 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/page_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2361 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/pagelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1178 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pageuri_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1342 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pageuri_redirect_test.py
+-rw-r-----   0 root         (0) root         (0)     1026 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pageuri_update_test.py
+-rw-r-----   0 root         (0) root         (0)      974 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pageurilist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      839 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pageurilist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1420 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/paymentmethodlist_load_test.py
+-rw-r-----   0 root         (0) root         (0)      895 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroup_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     3853 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/pricegroup_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1440 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/pricegroup_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2011 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupbusinessaccount_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1191 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupbusinessaccountlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1841 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupcategory_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1117 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupcategorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2990 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupcustomer_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1386 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupcustomerlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2016 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupexcludedcategory_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1192 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupexcludedcategorylist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1991 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupexcludedproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1181 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupexcludedproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1225 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2940 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1340 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2033 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupqualifyingproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1199 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/pricegroupqualifyingproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1343 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/printqueuejob_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1270 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/printqueuejob_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1396 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/printqueuejob_status_test.py
+-rw-r-----   0 root         (0) root         (0)     1386 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/printqueuejoblist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)      859 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/printqueuelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2868 2023-03-23 19:33:09.000000 merchantapi-2.6.0/tests/product_copy_test.py
+-rw-r-----   0 root         (0) root         (0)     2132 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/product_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     4309 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/product_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2022 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/product_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1209 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productandsubscriptiontermlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1498 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productattributeandoptionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1848 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productimage_add_test.py
+-rw-r-----   0 root         (0) root         (0)     1193 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productimage_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1647 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productimage_update_type_test.py
+-rw-r-----   0 root         (0) root         (0)     1031 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productkit_generate_variants_test.py
+-rw-r-----   0 root         (0) root         (0)     1320 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productkit_update_parts_test.py
+-rw-r-----   0 root         (0) root         (0)      859 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productkit_variant_count_test.py
+-rw-r-----   0 root         (0) root         (0)      915 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productkitlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1033 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productlist_adjust_inventory_test.py
+-rw-r-----   0 root         (0) root         (0)     9492 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/productlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2131 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/productshippingrules_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1197 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productsubscriptiontermlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1212 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/producturi_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1469 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/producturi_redirect_test.py
+-rw-r-----   0 root         (0) root         (0)     1217 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/producturi_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1067 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/producturilist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1078 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/producturilist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1254 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariant_generate_delimiter_test.py
+-rw-r-----   0 root         (0) root         (0)     1149 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariant_generate_test.py
+-rw-r-----   0 root         (0) root         (0)     3550 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariant_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     1813 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariant_update_test.py
+-rw-r-----   0 root         (0) root         (0)     1218 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariantlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1610 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariantlist_load_product_test.py
+-rw-r-----   0 root         (0) root         (0)     1424 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/productvariantlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1441 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/productvariantpricing_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2244 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/relatedproduct_update_assigned_test.py
+-rw-r-----   0 root         (0) root         (0)     1117 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/relatedproductlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1960 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/request_builder_test.py
+-rw-r-----   0 root         (0) root         (0)     1781 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/resourcegrouplist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1070 2023-07-17 20:14:29.000000 merchantapi-2.6.0/tests/store_load_test.py
+-rw-r-----   0 root         (0) root         (0)      796 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/storelist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     3643 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscription_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     2488 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscription_update_test.py
+-rw-r-----   0 root         (0) root         (0)     4546 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscriptionandorderitem_add_test.py
+-rw-r-----   0 root         (0) root         (0)     3573 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscriptionandorderitem_update_test.py
+-rw-r-----   0 root         (0) root         (0)     2889 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscriptionlist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     1967 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscriptionlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1842 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/subscriptionshippingmethodlist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     1057 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/uri_delete_test.py
+-rw-r-----   0 root         (0) root         (0)     3541 2024-03-11 21:44:54.000000 merchantapi-2.6.0/tests/uri_insert_test.py
+-rw-r-----   0 root         (0) root         (0)     3598 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/uri_update_test.py
+-rw-r-----   0 root         (0) root         (0)      957 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/urilist_delete_test.py
+-rw-r-----   0 root         (0) root         (0)      753 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/urilist_load_query_test.py
+-rw-r-----   0 root         (0) root         (0)     2140 2023-01-24 22:23:48.000000 merchantapi-2.6.0/tests/version_settings_test.py
```

### Comparing `merchantapi-2.5.0/LICENSE` & `merchantapi-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/PKG-INFO` & `merchantapi-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merchantapi
-Version: 2.5.0
+Version: 2.6.0
 Summary: Miva Merchant JSON API SDK
 Home-page: https://www.miva.com
 Author: Miva, Inc.
 Author-email: support@miva.com
 License: Miva SDK License Agreement
 Description: # Miva Merchant API SDK for Python (3.x)
         
@@ -30,15 +30,15 @@
             
         *Note: On some operating systems the `pip` program may be named `pip3`*
         
         # Adding as a dependency in your packages
         
         You can also add it to your project's `requirements.txt` file:
         
-            merchantapi>=2.5.0
+            merchantapi>=2.6.0
             
         Then install
         
             pip install -r requirements.txt
             
         *Note: On some operating systems the `pip` program may be named `pip3`*
```

### Comparing `merchantapi-2.5.0/README.md` & `merchantapi-2.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     
 *Note: On some operating systems the `pip` program may be named `pip3`*
 
 # Adding as a dependency in your packages
 
 You can also add it to your project's `requirements.txt` file:
 
-    merchantapi>=2.5.0
+    merchantapi>=2.6.0
     
 Then install
 
     pip install -r requirements.txt
     
 *Note: On some operating systems the `pip` program may be named `pip3`*
```

### Comparing `merchantapi-2.5.0/merchantapi/abstract.py` & `merchantapi-2.6.0/merchantapi/abstract.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/authenticator.py` & `merchantapi-2.6.0/merchantapi/authenticator.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/client.py` & `merchantapi-2.6.0/merchantapi/client.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/listquery.py` & `merchantapi-2.6.0/merchantapi/listquery.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/logging.py` & `merchantapi-2.6.0/merchantapi/logging.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/__init__.py` & `merchantapi-2.6.0/merchantapi/model/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,18 @@
 from .module_change import ModuleChange
 from .copy_page_rule import CopyPageRule
 from .copy_page_rules_settings import CopyPageRulesSettings
 from .copy_product_rule import CopyProductRule
 from .copy_product_rules_module import CopyProductRulesModule
 from .copy_product_rules_custom_field import CopyProductRulesCustomField
 from .product_subscription_settings import ProductSubscriptionSettings
+from .branch_item_version import BranchItemVersion
+from .changeset_item_version import ChangesetItemVersion
+from .branch_page_version import BranchPageVersion
+from .shipping_rule_method import ShippingRuleMethod
 from .availability_group_customer import AvailabilityGroupCustomer
 from .availability_group_category import AvailabilityGroupCategory
 from .availability_group_product import AvailabilityGroupProduct
 from .availability_group_business_account import AvailabilityGroupBusinessAccount
 from .business_account_customer import BusinessAccountCustomer
 from .order_note import OrderNote
 from .category_product import CategoryProduct
@@ -143,7 +147,8 @@
 from .javascript_resource_attribute import JavaScriptResourceAttribute
 from .order_price_group import OrderPriceGroup
 from .branch_property_version import BranchPropertyVersion
 from .changeset_property_version import ChangesetPropertyVersion
 from .customer_subscription import CustomerSubscription
 from .product_and_subscription_term import ProductAndSubscriptionTerm
 from .all_order_payment import AllOrderPayment
+from .coupon_business_account import CouponBusinessAccount
```

### Comparing `merchantapi-2.5.0/merchantapi/model/all_order_payment.py` & `merchantapi-2.6.0/merchantapi/model/all_order_payment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/attribute_template.py` & `merchantapi-2.6.0/merchantapi/model/attribute_template.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/attribute_template_attribute.py` & `merchantapi-2.6.0/merchantapi/model/attribute_template_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/attribute_template_option.py` & `merchantapi-2.6.0/merchantapi/model/attribute_template_option.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/attribute_template_product.py` & `merchantapi-2.6.0/merchantapi/model/attribute_template_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group.py` & `merchantapi-2.6.0/merchantapi/model/availability_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group_business_account.py` & `merchantapi-2.6.0/merchantapi/model/availability_group_business_account.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group_category.py` & `merchantapi-2.6.0/merchantapi/model/availability_group_category.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group_customer.py` & `merchantapi-2.6.0/merchantapi/model/availability_group_customer.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group_product.py` & `merchantapi-2.6.0/merchantapi/model/availability_group_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/availability_group_shipping_method.py` & `merchantapi-2.6.0/merchantapi/model/availability_group_shipping_method.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/branch.py` & `merchantapi-2.6.0/merchantapi/model/branch.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/branch_javascript_resource_version.py` & `merchantapi-2.6.0/merchantapi/model/branch_javascript_resource_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/branch_template_version.py` & `merchantapi-2.6.0/merchantapi/model/branch_template_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/business_account.py` & `merchantapi-2.6.0/merchantapi/model/business_account.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/business_account_customer.py` & `merchantapi-2.6.0/merchantapi/model/business_account_customer.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/category.py` & `merchantapi-2.6.0/merchantapi/model/category.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/category_product.py` & `merchantapi-2.6.0/merchantapi/model/category_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/changeset.py` & `merchantapi-2.6.0/merchantapi/model/changeset.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/changeset_change.py` & `merchantapi-2.6.0/merchantapi/model/changeset_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/changeset_javascript_resource_version.py` & `merchantapi-2.6.0/merchantapi/model/changeset_javascript_resource_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/changeset_template_version.py` & `merchantapi-2.6.0/merchantapi/model/changeset_template_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/copy_page_rule.py` & `merchantapi-2.6.0/merchantapi/model/copy_page_rule.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/copy_page_rules_settings.py` & `merchantapi-2.6.0/merchantapi/model/copy_page_rules_settings.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/copy_product_rule.py` & `merchantapi-2.6.0/merchantapi/model/copy_product_rule.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/copy_product_rules_custom_field.py` & `merchantapi-2.6.0/merchantapi/model/copy_product_rules_custom_field.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/copy_product_rules_module.py` & `merchantapi-2.6.0/merchantapi/model/copy_product_rules_module.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/coupon.py` & `merchantapi-2.6.0/merchantapi/model/coupon.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/coupon_customer.py` & `merchantapi-2.6.0/merchantapi/model/coupon_customer.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/coupon_price_group.py` & `merchantapi-2.6.0/merchantapi/model/coupon_price_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/css_resource.py` & `merchantapi-2.6.0/merchantapi/model/css_resource.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/css_resource_change.py` & `merchantapi-2.6.0/merchantapi/model/css_resource_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/css_resource_version.py` & `merchantapi-2.6.0/merchantapi/model/css_resource_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/custom_field_values.py` & `merchantapi-2.6.0/merchantapi/model/custom_field_values.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer.py` & `merchantapi-2.6.0/merchantapi/model/customer.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_address.py` & `merchantapi-2.6.0/merchantapi/model/customer_address.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_address_list.py` & `merchantapi-2.6.0/merchantapi/model/customer_address_list.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_credit_history.py` & `merchantapi-2.6.0/merchantapi/model/customer_credit_history.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_payment_card.py` & `merchantapi-2.6.0/merchantapi/model/customer_payment_card.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_price_group.py` & `merchantapi-2.6.0/merchantapi/model/customer_price_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/customer_subscription.py` & `merchantapi-2.6.0/merchantapi/model/customer_subscription.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/discount_module_capabilities.py` & `merchantapi-2.6.0/merchantapi/model/discount_module_capabilities.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/image_type.py` & `merchantapi-2.6.0/merchantapi/model/image_type.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/javascript_resource.py` & `merchantapi-2.6.0/merchantapi/model/javascript_resource.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/javascript_resource_change.py` & `merchantapi-2.6.0/merchantapi/model/javascript_resource_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/javascript_resource_version.py` & `merchantapi-2.6.0/merchantapi/model/javascript_resource_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/javascript_resource_version_attribute.py` & `merchantapi-2.6.0/merchantapi/model/javascript_resource_version_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/kit_part.py` & `merchantapi-2.6.0/merchantapi/model/kit_part.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/merchant_version.py` & `merchantapi-2.6.0/merchantapi/model/merchant_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/module.py` & `merchantapi-2.6.0/merchantapi/model/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,7 +97,16 @@
 		"""
 		Get active.
 
 		:returns: bool
 		"""
 
 		return self.get_field('active', False)
+
+	def get_priority(self) -> int:
+		"""
+		Get priority.
+
+		:returns: int
+		"""
+
+		return self.get_field('priority', 0)
```

### Comparing `merchantapi-2.5.0/merchantapi/model/module_change.py` & `merchantapi-2.6.0/merchantapi/model/module_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/note.py` & `merchantapi-2.6.0/merchantapi/model/note.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order.py` & `merchantapi-2.6.0/merchantapi/model/order.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_charge.py` & `merchantapi-2.6.0/merchantapi/model/order_charge.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_coupon.py` & `merchantapi-2.6.0/merchantapi/model/order_coupon.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_custom_field.py` & `merchantapi-2.6.0/merchantapi/model/order_custom_field.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_discount_total.py` & `merchantapi-2.6.0/merchantapi/model/order_discount_total.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_item.py` & `merchantapi-2.6.0/merchantapi/model/order_item.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_item_discount.py` & `merchantapi-2.6.0/merchantapi/model/order_item_discount.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_item_option.py` & `merchantapi-2.6.0/merchantapi/model/order_item_option.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_item_option_discount.py` & `merchantapi-2.6.0/merchantapi/model/order_item_option_discount.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_item_subscription.py` & `merchantapi-2.6.0/merchantapi/model/order_item_subscription.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_part.py` & `merchantapi-2.6.0/merchantapi/model/order_part.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_payment.py` & `merchantapi-2.6.0/merchantapi/model/order_payment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_payment_authorize.py` & `merchantapi-2.6.0/merchantapi/model/order_payment_authorize.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_payment_total.py` & `merchantapi-2.6.0/merchantapi/model/order_payment_total.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_price_group.py` & `merchantapi-2.6.0/merchantapi/model/order_price_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_product.py` & `merchantapi-2.6.0/merchantapi/model/order_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_product_attribute.py` & `merchantapi-2.6.0/merchantapi/model/order_product_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_return.py` & `merchantapi-2.6.0/merchantapi/model/order_return.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_shipment.py` & `merchantapi-2.6.0/merchantapi/model/order_shipment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_shipment_update.py` & `merchantapi-2.6.0/merchantapi/model/order_shipment_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_total.py` & `merchantapi-2.6.0/merchantapi/model/order_total.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/order_total_and_item.py` & `merchantapi-2.6.0/merchantapi/model/order_total_and_item.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/page.py` & `merchantapi-2.6.0/merchantapi/model/page.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,14 +195,23 @@
 		Get CustomField_Values.
 
 		:returns: CustomFieldValues|None
 		"""
 
 		return self.get_field('CustomField_Values', None)
 
+	def get_version_id(self) -> int:
+		"""
+		Get version_id.
+
+		:returns: int
+		"""
+
+		return self.get_field('version_id', 0)
+
 	def to_dict(self) -> dict:
 		"""
 		Reduce the model to a dict.
 		"""
 
 		ret = self.copy()
```

### Comparing `merchantapi-2.5.0/merchantapi/model/payment_card_type.py` & `merchantapi-2.6.0/merchantapi/model/payment_card_type.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/payment_method.py` & `merchantapi-2.6.0/merchantapi/model/payment_method.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group.py` & `merchantapi-2.6.0/merchantapi/model/price_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group_business_account.py` & `merchantapi-2.6.0/merchantapi/model/price_group_business_account.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group_category.py` & `merchantapi-2.6.0/merchantapi/model/price_group_category.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group_customer.py` & `merchantapi-2.6.0/merchantapi/model/price_group_customer.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group_exclusion.py` & `merchantapi-2.6.0/merchantapi/model/price_group_exclusion.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/price_group_product.py` & `merchantapi-2.6.0/merchantapi/model/price_group_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/print_queue.py` & `merchantapi-2.6.0/merchantapi/model/print_queue.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/print_queue_job.py` & `merchantapi-2.6.0/merchantapi/model/print_queue_job.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product.py` & `merchantapi-2.6.0/merchantapi/model/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,23 @@
 		Get cancat_code.
 
 		:returns: string
 		"""
 
 		return self.get_field('cancat_code')
 
+	def get_page_id(self) -> int:
+		"""
+		Get page_id.
+
+		:returns: int
+		"""
+
+		return self.get_field('page_id', 0)
+
 	def get_page_code(self) -> str:
 		"""
 		Get page_code.
 
 		:returns: string
 		"""
```

### Comparing `merchantapi-2.5.0/merchantapi/model/product_and_subscription_term.py` & `merchantapi-2.6.0/merchantapi/model/product_and_subscription_term.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_attribute.py` & `merchantapi-2.6.0/merchantapi/model/product_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_attribute_list_attribute.py` & `merchantapi-2.6.0/merchantapi/model/product_attribute_list_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_attribute_list_option.py` & `merchantapi-2.6.0/merchantapi/model/product_attribute_list_option.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_attribute_list_template.py` & `merchantapi-2.6.0/merchantapi/model/product_attribute_list_template.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_image_data.py` & `merchantapi-2.6.0/merchantapi/model/product_image_data.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_inventory_adjustment.py` & `merchantapi-2.6.0/merchantapi/model/product_inventory_adjustment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_inventory_settings.py` & `merchantapi-2.6.0/merchantapi/model/product_inventory_settings.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_kit.py` & `merchantapi-2.6.0/merchantapi/model/product_kit.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_kit_part.py` & `merchantapi-2.6.0/merchantapi/model/product_kit_part.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_option.py` & `merchantapi-2.6.0/merchantapi/model/product_option.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_shipping_method.py` & `merchantapi-2.6.0/merchantapi/model/product_shipping_method.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_shipping_rules.py` & `merchantapi-2.6.0/merchantapi/model/product_shipping_rules.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_subscription_settings.py` & `merchantapi-2.6.0/merchantapi/model/product_subscription_settings.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_subscription_term.py` & `merchantapi-2.6.0/merchantapi/model/product_subscription_term.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_subscription_term_date.py` & `merchantapi-2.6.0/merchantapi/model/product_subscription_term_date.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant.py` & `merchantapi-2.6.0/merchantapi/model/product_variant.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant_attribute.py` & `merchantapi-2.6.0/merchantapi/model/product_variant_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant_dimension.py` & `merchantapi-2.6.0/merchantapi/model/product_variant_dimension.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant_exclusion.py` & `merchantapi-2.6.0/merchantapi/model/product_variant_exclusion.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant_limit.py` & `merchantapi-2.6.0/merchantapi/model/product_variant_limit.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/product_variant_part.py` & `merchantapi-2.6.0/merchantapi/model/product_variant_part.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/property_change.py` & `merchantapi-2.6.0/merchantapi/model/property_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/property_version.py` & `merchantapi-2.6.0/merchantapi/model/property_version.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/provision_message.py` & `merchantapi-2.6.0/merchantapi/model/provision_message.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/received_return.py` & `merchantapi-2.6.0/merchantapi/model/received_return.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/related_product.py` & `merchantapi-2.6.0/merchantapi/model/related_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/resource_attribute.py` & `merchantapi-2.6.0/merchantapi/model/resource_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/resource_group.py` & `merchantapi-2.6.0/merchantapi/model/resource_group.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/resource_group_change.py` & `merchantapi-2.6.0/merchantapi/model/resource_group_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/split_order_item.py` & `merchantapi-2.6.0/merchantapi/model/split_order_item.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/store.py` & `merchantapi-2.6.0/merchantapi/model/store.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/subscription.py` & `merchantapi-2.6.0/merchantapi/model/subscription.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/subscription_attribute.py` & `merchantapi-2.6.0/merchantapi/model/subscription_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/subscription_option.py` & `merchantapi-2.6.0/merchantapi/model/subscription_option.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/subscription_shipping_method.py` & `merchantapi-2.6.0/merchantapi/model/subscription_shipping_method.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/template_change.py` & `merchantapi-2.6.0/merchantapi/model/template_change.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/uri.py` & `merchantapi-2.6.0/merchantapi/model/uri.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,23 @@
 		Get page_id.
 
 		:returns: int
 		"""
 
 		return self.get_field('page_id', 0)
 
+	def get_page_code(self) -> str:
+		"""
+		Get page_code.
+
+		:returns: string
+		"""
+
+		return self.get_field('page_code')
+
 	def get_category_id(self) -> int:
 		"""
 		Get cat_id.
 
 		:returns: int
 		"""
```

### Comparing `merchantapi-2.5.0/merchantapi/model/uri_detail.py` & `merchantapi-2.6.0/merchantapi/model/uri_detail.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/variable_value.py` & `merchantapi-2.6.0/merchantapi/model/variable_value.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/variant_attribute.py` & `merchantapi-2.6.0/merchantapi/model/variant_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/variant_part.py` & `merchantapi-2.6.0/merchantapi/model/variant_part.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/model/version_settings.py` & `merchantapi-2.6.0/merchantapi/model/version_settings.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/multicall.py` & `merchantapi-2.6.0/merchantapi/multicall.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/__init__.py` & `merchantapi-2.6.0/merchantapi/request/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,22 @@
 from .copyproductruleslist_delete import CopyProductRulesListDelete
 from .copyproductruleslist_load_query import CopyProductRulesListLoadQuery
 from .copyproductrulesmodulelist_load_query import CopyProductRulesModuleListLoadQuery
 from .copyproductrulesmodule_update_assigned import CopyProductRulesModuleUpdateAssigned
 from .copyproductrulescustomfieldlist_load_query import CopyProductRulesCustomFieldListLoadQuery
 from .copyproductrulescustomfield_update_assigned import CopyProductRulesCustomFieldUpdateAssigned
 from .orderlist_archive import OrderListArchive
+from .page_copy_branch import PageCopyBranch
+from .branchitemversionlist_load_query import BranchItemVersionListLoadQuery
+from .changesetitemversionlist_load_query import ChangesetItemVersionListLoadQuery
+from .branchpageversionlist_load_query import BranchPageVersionListLoadQuery
+from .couponbusinessaccountlist_load_query import CouponBusinessAccountListLoadQuery
+from .couponbusinessaccount_update_assigned import CouponBusinessAccountUpdateAssigned
+from .productvariantpricing_update import ProductVariantPricingUpdate
+from .productshippingrules_update import ProductShippingRulesUpdate
 from .categoryproductlist_load_query import CategoryProductListLoadQuery
 from .couponpricegrouplist_load_query import CouponPriceGroupListLoadQuery
 from .pricegroupcustomerlist_load_query import PriceGroupCustomerListLoadQuery
 from .pricegroupproductlist_load_query import PriceGroupProductListLoadQuery
 from .customerpricegrouplist_load_query import CustomerPriceGroupListLoadQuery
 from .orderpricegrouplist_load_query import OrderPriceGroupListLoadQuery
 from .ordercouponlist_load_query import OrderCouponListLoadQuery
```

### Comparing `merchantapi-2.5.0/merchantapi/request/allorderpaymentlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/allorderpaymentlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_copylinkedtemplate.py` & `merchantapi-2.6.0/merchantapi/request/attribute_copylinkedtemplate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_copytemplate.py` & `merchantapi-2.6.0/merchantapi/request/attribute_copytemplate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_delete.py` & `merchantapi-2.6.0/merchantapi/request/attribute_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_insert.py` & `merchantapi-2.6.0/merchantapi/request/attribute_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_load_code.py` & `merchantapi-2.6.0/merchantapi/request/attribute_load_code.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attribute_update.py` & `merchantapi-2.6.0/merchantapi/request/attribute_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributeandoptionlist_load_product.py` & `merchantapi-2.6.0/merchantapi/request/attributeandoptionlist_load_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplate_delete.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplate_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplate_insert.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplate_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplate_update.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplate_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_delete.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_insert.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateattribute_update.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateattribute_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateattributelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateattributelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplatelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplatelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateoption_delete.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateoption_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateoption_insert.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateoption_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateoption_set_default.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateoption_set_default.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateoption_update.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateoption_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateoptionlist_load_attribute.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateoptionlist_load_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/attributetemplateproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/attributetemplateproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroup_delete.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroup_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroup_insert.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroup_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroup_update.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroup_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupbusinessaccount_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupbusinessaccount_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupbusinessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupbusinessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygrouppaymentmethod_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygrouppaymentmethod_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupshippingmethod_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupshippingmethod_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/availabilitygroupshippingmethodlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/availabilitygroupshippingmethodlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branch_copy.py` & `merchantapi-2.6.0/merchantapi/request/branch_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branch_create.py` & `merchantapi-2.6.0/merchantapi/request/branch_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branch_delete.py` & `merchantapi-2.6.0/merchantapi/request/branch_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branch_setprimary.py` & `merchantapi-2.6.0/merchantapi/request/branch_setprimary.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branch_update.py` & `merchantapi-2.6.0/merchantapi/request/branch_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchcssresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/branchcssresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchjavascriptresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/branchjavascriptresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/branchlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/branchlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchpropertyversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/branchpropertyversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/branchtemplateversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/branchtemplateversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccount_insert.py` & `merchantapi-2.6.0/merchantapi/request/businessaccount_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccount_update.py` & `merchantapi-2.6.0/merchantapi/request/businessaccount_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccountcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/businessaccountcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccountcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/businessaccountcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccountlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/businessaccountlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/businessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/businessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/category_delete.py` & `merchantapi-2.6.0/merchantapi/request/category_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/category_insert.py` & `merchantapi-2.6.0/merchantapi/request/category_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/category_update.py` & `merchantapi-2.6.0/merchantapi/request/category_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categorylist_load_parent.py` & `merchantapi-2.6.0/merchantapi/request/categorylist_load_parent.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/categorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/categoryproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/categoryproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryuri_insert.py` & `merchantapi-2.6.0/merchantapi/request/categoryuri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryuri_redirect.py` & `merchantapi-2.6.0/merchantapi/request/categoryuri_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryuri_update.py` & `merchantapi-2.6.0/merchantapi/request/categoryuri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryurilist_delete.py` & `merchantapi-2.6.0/merchantapi/request/categoryurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/categoryurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/categoryurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changeset_create.py` & `merchantapi-2.6.0/merchantapi/request/changeset_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetchangelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesetchangelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetcssresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesetcssresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetjavascriptresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesetjavascriptresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesetlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetlist_merge.py` & `merchantapi-2.6.0/merchantapi/request/changesetlist_merge.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesetpropertyversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesetpropertyversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/changesettemplateversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/changesettemplateversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/childcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/childcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypagerules_insert.py` & `merchantapi-2.6.0/merchantapi/request/copypagerules_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypagerules_update.py` & `merchantapi-2.6.0/merchantapi/request/copypagerules_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypageruleslist_delete.py` & `merchantapi-2.6.0/merchantapi/request/copypageruleslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypageruleslist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/copypageruleslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypagerulessettings_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/copypagerulessettings_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copypagerulessettingslist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/copypagerulessettingslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrules_insert.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrules_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrules_update.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrules_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrulescustomfield_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrulescustomfield_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrulescustomfieldlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrulescustomfieldlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductruleslist_delete.py` & `merchantapi-2.6.0/merchantapi/request/copyproductruleslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductruleslist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/copyproductruleslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrulesmodule_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrulesmodule_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/copyproductrulesmodulelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/copyproductrulesmodulelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/coupon_insert.py` & `merchantapi-2.6.0/merchantapi/request/coupon_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/coupon_update.py` & `merchantapi-2.6.0/merchantapi/request/coupon_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/couponcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/couponcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/couponlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/couponlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponpricegroup_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/couponpricegroup_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/couponpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/couponpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/cssresource_delete.py` & `merchantapi-2.6.0/merchantapi/request/cssresource_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/cssresource_insert.py` & `merchantapi-2.6.0/merchantapi/request/cssresource_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/cssresource_update.py` & `merchantapi-2.6.0/merchantapi/request/cssresource_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/cssresourcelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/cssresourcelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customer_delete.py` & `merchantapi-2.6.0/merchantapi/request/customer_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customer_insert.py` & `merchantapi-2.6.0/merchantapi/request/customer_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customer_update.py` & `merchantapi-2.6.0/merchantapi/request/customer_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddress_delete.py` & `merchantapi-2.6.0/merchantapi/request/customeraddress_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddress_insert.py` & `merchantapi-2.6.0/merchantapi/request/customeraddress_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddress_update.py` & `merchantapi-2.6.0/merchantapi/request/customeraddress_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddress_update_residential.py` & `merchantapi-2.6.0/merchantapi/request/customeraddress_update_residential.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddresslist_delete.py` & `merchantapi-2.6.0/merchantapi/request/customeraddresslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customeraddresslist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customeraddresslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customercredithistory_delete.py` & `merchantapi-2.6.0/merchantapi/request/customercredithistory_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customercredithistory_insert.py` & `merchantapi-2.6.0/merchantapi/request/customercredithistory_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customercredithistorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customercredithistorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customerpaymentcard_register.py` & `merchantapi-2.6.0/merchantapi/request/customerpaymentcard_register.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customerpaymentcardlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customerpaymentcardlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customerpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customerpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/customersubscriptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/customersubscriptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/feeduri_insert.py` & `merchantapi-2.6.0/merchantapi/request/feeduri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/feeduri_update.py` & `merchantapi-2.6.0/merchantapi/request/feeduri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/feedurilist_delete.py` & `merchantapi-2.6.0/merchantapi/request/feedurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/feedurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/feedurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/imagetypelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/imagetypelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/inventoryproductsettings_update.py` & `merchantapi-2.6.0/merchantapi/request/inventoryproductsettings_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/javascriptresource_delete.py` & `merchantapi-2.6.0/merchantapi/request/javascriptresource_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/javascriptresource_insert.py` & `merchantapi-2.6.0/merchantapi/request/javascriptresource_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/javascriptresource_update.py` & `merchantapi-2.6.0/merchantapi/request/javascriptresource_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/javascriptresourcelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/javascriptresourcelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/mivamerchantversion.py` & `merchantapi-2.6.0/merchantapi/request/mivamerchantversion.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/module.py` & `merchantapi-2.6.0/merchantapi/request/module.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/note_delete.py` & `merchantapi-2.6.0/merchantapi/request/note_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/note_insert.py` & `merchantapi-2.6.0/merchantapi/request/note_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/note_update.py` & `merchantapi-2.6.0/merchantapi/request/note_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/notelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/notelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/option_delete.py` & `merchantapi-2.6.0/merchantapi/request/option_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/option_insert.py` & `merchantapi-2.6.0/merchantapi/request/option_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/option_load_code.py` & `merchantapi-2.6.0/merchantapi/request/option_load_code.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/option_set_default.py` & `merchantapi-2.6.0/merchantapi/request/option_set_default.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/option_update.py` & `merchantapi-2.6.0/merchantapi/request/option_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/optionlist_load_attribute.py` & `merchantapi-2.6.0/merchantapi/request/optionlist_load_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/order_authorize.py` & `merchantapi-2.6.0/merchantapi/request/order_authorize.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/order_create.py` & `merchantapi-2.6.0/merchantapi/request/order_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/order_create_fromorder.py` & `merchantapi-2.6.0/merchantapi/request/order_create_fromorder.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/order_delete.py` & `merchantapi-2.6.0/merchantapi/request/order_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/order_update_customer_information.py` & `merchantapi-2.6.0/merchantapi/request/order_update_customer_information.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordercoupon_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/ordercoupon_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordercouponlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/ordercouponlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordercustomfieldlist_load.py` & `merchantapi-2.6.0/merchantapi/request/ordercustomfieldlist_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordercustomfields_update.py` & `merchantapi-2.6.0/merchantapi/request/ordercustomfields_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitem_add.py` & `merchantapi-2.6.0/merchantapi/request/orderitem_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitem_split.py` & `merchantapi-2.6.0/merchantapi/request/orderitem_split.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitem_update.py` & `merchantapi-2.6.0/merchantapi/request/orderitem_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_backorder.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_backorder.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_cancel.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_cancel.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_createreturn.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_createreturn.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_createshipment.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_createshipment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderitemlist_removefromshipment.py` & `merchantapi-2.6.0/merchantapi/request/orderitemlist_removefromshipment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderlist_archive.py` & `merchantapi-2.6.0/merchantapi/request/orderlist_archive.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/orderlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderpayment_capture.py` & `merchantapi-2.6.0/merchantapi/request/orderpayment_capture.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderpayment_refund.py` & `merchantapi-2.6.0/merchantapi/request/orderpayment_refund.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderpayment_void.py` & `merchantapi-2.6.0/merchantapi/request/orderpayment_void.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderpricegroup_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/orderpricegroup_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/orderpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/orderreturnlist_received.py` & `merchantapi-2.6.0/merchantapi/request/orderreturnlist_received.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordershipmentlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/ordershipmentlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/ordershipmentlist_update.py` & `merchantapi-2.6.0/merchantapi/request/ordershipmentlist_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/page_copy.py` & `merchantapi-2.6.0/merchantapi/request/page_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/page_delete.py` & `merchantapi-2.6.0/merchantapi/request/producturi_update.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,142 +2,161 @@
 This file is part of the MerchantAPI package.
 
 (c) Miva Inc <https://www.miva.com/>
 
 For the full copyright and license information, please view the LICENSE
 file that was distributed with this source code.
 
-Handles API Request Page_Delete. 
+Handles API Request ProductURI_Update. 
 Scope: Store.
-:see: https://docs.miva.com/json-api/functions/page_delete
+:see: https://docs.miva.com/json-api/functions/producturi_update
 """
 
 import merchantapi.abstract
 import merchantapi.model
 import merchantapi.response
 from merchantapi.client import BaseClient as Client
 from requests.models import Response as HttpResponse
 
 
-class PageDelete(merchantapi.abstract.Request):
-	def __init__(self, client: Client = None, page: merchantapi.model.Page = None):
+class ProductURIUpdate(merchantapi.abstract.Request):
+	def __init__(self, client: Client = None, uri: merchantapi.model.Uri = None):
 		"""
-		PageDelete Constructor.
+		ProductURIUpdate Constructor.
 
 		:param client: Client
-		:param page: Page
+		:param uri: Uri
 		"""
 
 		super().__init__(client)
-		self.page_id = None
-		self.edit_page = None
-		self.page_code = None
-		if isinstance(page, merchantapi.model.Page):
-			if page.get_id():
-				self.set_page_id(page.get_id())
-			elif page.get_code():
-				self.set_edit_page(page.get_code())
-			elif page.get_code():
-				self.set_page_code(page.get_code())
+		self.uri_id = None
+		self.uri = None
+		self.status = None
+		self.canonical = None
+		if isinstance(uri, merchantapi.model.Uri):
+			if uri.get_id():
+				self.set_uri_id(uri.get_id())
 
 	def get_function(self):
 		"""
 		Get the function of the request.
 
 		:returns: str
 		"""
 
-		return 'Page_Delete'
+		return 'ProductURI_Update'
 
-	def get_page_id(self) -> int:
+	def get_uri_id(self) -> int:
 		"""
-		Get Page_ID.
+		Get URI_ID.
 
 		:returns: int
 		"""
 
-		return self.page_id
+		return self.uri_id
 
-	def get_edit_page(self) -> str:
+	def get_uri(self) -> str:
 		"""
-		Get Edit_Page.
+		Get URI.
 
 		:returns: str
 		"""
 
-		return self.edit_page
+		return self.uri
 
-	def get_page_code(self) -> str:
+	def get_status(self) -> int:
 		"""
-		Get Page_Code.
+		Get Status.
 
-		:returns: str
+		:returns: int
+		"""
+
+		return self.status
+
+	def get_canonical(self) -> bool:
+		"""
+		Get Canonical.
+
+		:returns: bool
 		"""
 
-		return self.page_code
+		return self.canonical
+
+	def set_uri_id(self, uri_id: int) -> 'ProductURIUpdate':
+		"""
+		Set URI_ID.
+
+		:param uri_id: int
+		:returns: ProductURIUpdate
+		"""
+
+		self.uri_id = uri_id
+		return self
 
-	def set_page_id(self, page_id: int) -> 'PageDelete':
+	def set_uri(self, uri: str) -> 'ProductURIUpdate':
 		"""
-		Set Page_ID.
+		Set URI.
 
-		:param page_id: int
-		:returns: PageDelete
+		:param uri: str
+		:returns: ProductURIUpdate
 		"""
 
-		self.page_id = page_id
+		self.uri = uri
 		return self
 
-	def set_edit_page(self, edit_page: str) -> 'PageDelete':
+	def set_status(self, status: int) -> 'ProductURIUpdate':
 		"""
-		Set Edit_Page.
+		Set Status.
 
-		:param edit_page: str
-		:returns: PageDelete
+		:param status: int
+		:returns: ProductURIUpdate
 		"""
 
-		self.edit_page = edit_page
+		self.status = status
 		return self
 
-	def set_page_code(self, page_code: str) -> 'PageDelete':
+	def set_canonical(self, canonical: bool) -> 'ProductURIUpdate':
 		"""
-		Set Page_Code.
+		Set Canonical.
 
-		:param page_code: str
-		:returns: PageDelete
+		:param canonical: bool
+		:returns: ProductURIUpdate
 		"""
 
-		self.page_code = page_code
+		self.canonical = canonical
 		return self
 
 	# noinspection PyTypeChecker
-	def send(self) -> 'merchantapi.response.PageDelete':
+	def send(self) -> 'merchantapi.response.ProductURIUpdate':
 		return super().send()
 
-	def create_response(self, http_response: HttpResponse, data) -> 'PageDelete':
+	def create_response(self, http_response: HttpResponse, data) -> 'ProductURIUpdate':
 		"""
 		Create a response object from the response data
 
 		:param http_response: requests.models.Response
 		:param data:
 		:returns: Response
 		"""
 
-		return merchantapi.response.PageDelete(self, http_response, data)
+		return merchantapi.response.ProductURIUpdate(self, http_response, data)
 
 	def to_dict(self) -> dict:
 		"""
 		Reduce the request to a dict
 
 		:override:
 		:returns: dict
 		"""
 
 		data = super().to_dict()
 
-		if self.page_id is not None:
-			data['Page_ID'] = self.page_id
-		elif self.edit_page is not None:
-			data['Edit_Page'] = self.edit_page
-		elif self.page_code is not None:
-			data['Page_Code'] = self.page_code
+		if self.uri_id is not None:
+			data['URI_ID'] = self.uri_id
 
+		if self.uri is not None:
+			data['URI'] = self.uri
+		if self.status is not None:
+			data['Status'] = self.status
+		if self.canonical is not None:
+			data['Canonical'] = self.canonical
 		return data
```

### Comparing `merchantapi-2.5.0/merchantapi/request/page_insert.py` & `merchantapi-2.6.0/merchantapi/request/page_insert.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,17 @@
 		self.page_template = None
 		self.page_layout = None
 		self.page_secure = None
 		self.page_cache = None
 		self.changeset_notes = None
 		self.page_uri = None
 		self.custom_field_values = merchantapi.model.CustomFieldValues()
+		self.branch_id = None
+		self.edit_branch = None
+		self.branch_name = None
 
 	def get_function(self):
 		"""
 		Get the function of the request.
 
 		:returns: str
 		"""
@@ -133,14 +136,41 @@
 		Get CustomField_Values.
 
 		:returns: CustomFieldValues}|None
 		"""
 
 		return self.custom_field_values
 
+	def get_branch_id(self) -> int:
+		"""
+		Get Branch_ID.
+
+		:returns: int
+		"""
+
+		return self.branch_id
+
+	def get_edit_branch(self) -> str:
+		"""
+		Get Edit_Branch.
+
+		:returns: str
+		"""
+
+		return self.edit_branch
+
+	def get_branch_name(self) -> str:
+		"""
+		Get Branch_Name.
+
+		:returns: str
+		"""
+
+		return self.branch_name
+
 	def set_page_code(self, page_code: str) -> 'PageInsert':
 		"""
 		Set Page_Code.
 
 		:param page_code: str
 		:returns: PageInsert
 		"""
@@ -246,14 +276,47 @@
 		"""
 
 		if not isinstance(custom_field_values, merchantapi.model.CustomFieldValues):
 			raise Exception("Expected instance of CustomFieldValues")
 		self.custom_field_values = custom_field_values
 		return self
 
+	def set_branch_id(self, branch_id: int) -> 'PageInsert':
+		"""
+		Set Branch_ID.
+
+		:param branch_id: int
+		:returns: PageInsert
+		"""
+
+		self.branch_id = branch_id
+		return self
+
+	def set_edit_branch(self, edit_branch: str) -> 'PageInsert':
+		"""
+		Set Edit_Branch.
+
+		:param edit_branch: str
+		:returns: PageInsert
+		"""
+
+		self.edit_branch = edit_branch
+		return self
+
+	def set_branch_name(self, branch_name: str) -> 'PageInsert':
+		"""
+		Set Branch_Name.
+
+		:param branch_name: str
+		:returns: PageInsert
+		"""
+
+		self.branch_name = branch_name
+		return self
+
 	# noinspection PyTypeChecker
 	def send(self) -> 'merchantapi.response.PageInsert':
 		return super().send()
 
 	def create_response(self, http_response: HttpResponse, data) -> 'PageInsert':
 		"""
 		Create a response object from the response data
@@ -271,14 +334,21 @@
 
 		:override:
 		:returns: dict
 		"""
 
 		data = super().to_dict()
 
+		if self.branch_id is not None:
+			data['Branch_ID'] = self.branch_id
+		elif self.edit_branch is not None:
+			data['Edit_Branch'] = self.edit_branch
+		elif self.branch_name is not None:
+			data['Branch_Name'] = self.branch_name
+
 		data['Page_Code'] = self.page_code
 		data['Page_Name'] = self.page_name
 		if self.page_title is not None:
 			data['Page_Title'] = self.page_title
 		if self.page_template is not None:
 			data['Page_Template'] = self.page_template
 		if self.page_layout is not None:
```

### Comparing `merchantapi-2.5.0/merchantapi/request/page_update.py` & `merchantapi-2.6.0/merchantapi/request/page_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 		self.page_name = None
 		self.page_title = None
 		self.page_secure = None
 		self.page_cache = None
 		self.changeset_notes = None
 		self.page_uri = None
 		self.custom_field_values = merchantapi.model.CustomFieldValues()
+		self.branch_id = None
+		self.edit_branch = None
+		self.branch_name = None
 		if isinstance(page, merchantapi.model.Page):
 			if page.get_id():
 				self.set_page_id(page.get_id())
 			elif page.get_code():
 				self.set_edit_page(page.get_code())
 
 			self.set_page_code(page.get_code())
@@ -144,14 +147,41 @@
 		Get CustomField_Values.
 
 		:returns: CustomFieldValues}|None
 		"""
 
 		return self.custom_field_values
 
+	def get_branch_id(self) -> int:
+		"""
+		Get Branch_ID.
+
+		:returns: int
+		"""
+
+		return self.branch_id
+
+	def get_edit_branch(self) -> str:
+		"""
+		Get Edit_Branch.
+
+		:returns: str
+		"""
+
+		return self.edit_branch
+
+	def get_branch_name(self) -> str:
+		"""
+		Get Branch_Name.
+
+		:returns: str
+		"""
+
+		return self.branch_name
+
 	def set_page_id(self, page_id: int) -> 'PageUpdate':
 		"""
 		Set Page_ID.
 
 		:param page_id: int
 		:returns: PageUpdate
 		"""
@@ -257,14 +287,47 @@
 		"""
 
 		if not isinstance(custom_field_values, merchantapi.model.CustomFieldValues):
 			raise Exception("Expected instance of CustomFieldValues")
 		self.custom_field_values = custom_field_values
 		return self
 
+	def set_branch_id(self, branch_id: int) -> 'PageUpdate':
+		"""
+		Set Branch_ID.
+
+		:param branch_id: int
+		:returns: PageUpdate
+		"""
+
+		self.branch_id = branch_id
+		return self
+
+	def set_edit_branch(self, edit_branch: str) -> 'PageUpdate':
+		"""
+		Set Edit_Branch.
+
+		:param edit_branch: str
+		:returns: PageUpdate
+		"""
+
+		self.edit_branch = edit_branch
+		return self
+
+	def set_branch_name(self, branch_name: str) -> 'PageUpdate':
+		"""
+		Set Branch_Name.
+
+		:param branch_name: str
+		:returns: PageUpdate
+		"""
+
+		self.branch_name = branch_name
+		return self
+
 	# noinspection PyTypeChecker
 	def send(self) -> 'merchantapi.response.PageUpdate':
 		return super().send()
 
 	def create_response(self, http_response: HttpResponse, data) -> 'PageUpdate':
 		"""
 		Create a response object from the response data
@@ -289,14 +352,21 @@
 		if self.page_id is not None:
 			data['Page_ID'] = self.page_id
 		elif self.edit_page is not None:
 			data['Edit_Page'] = self.edit_page
 		elif self.page_code is not None:
 			data['Page_Code'] = self.page_code
 
+		if self.branch_id is not None:
+			data['Branch_ID'] = self.branch_id
+		elif self.edit_branch is not None:
+			data['Edit_Branch'] = self.edit_branch
+		elif self.branch_name is not None:
+			data['Branch_Name'] = self.branch_name
+
 		if self.page_code is not None:
 			data['Page_Code'] = self.page_code
 		data['Page_Name'] = self.page_name
 		if self.page_title is not None:
 			data['Page_Title'] = self.page_title
 		if self.page_secure is not None:
 			data['Page_Secure'] = self.page_secure
```

### Comparing `merchantapi-2.5.0/merchantapi/request/pagelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pagelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pageuri_insert.py` & `merchantapi-2.6.0/merchantapi/request/pageuri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pageuri_redirect.py` & `merchantapi-2.6.0/merchantapi/request/pageuri_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pageuri_update.py` & `merchantapi-2.6.0/merchantapi/request/pageuri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pageurilist_delete.py` & `merchantapi-2.6.0/merchantapi/request/pageurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pageurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pageurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/paymentmethodlist_load.py` & `merchantapi-2.6.0/merchantapi/request/paymentmethodlist_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroup_delete.py` & `merchantapi-2.6.0/merchantapi/request/pricegroup_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroup_insert.py` & `merchantapi-2.6.0/merchantapi/request/pricegroup_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroup_update.py` & `merchantapi-2.6.0/merchantapi/request/pricegroup_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupbusinessaccount_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupbusinessaccount_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupbusinessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupbusinessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupexcludedcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupexcludedcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupexcludedcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupexcludedcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupexcludedproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupexcludedproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupexcludedproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupexcludedproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupqualifyingproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupqualifyingproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/pricegroupqualifyingproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/pricegroupqualifyingproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/printqueuejob_delete.py` & `merchantapi-2.6.0/merchantapi/request/printqueuejob_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/printqueuejob_insert.py` & `merchantapi-2.6.0/merchantapi/request/printqueuejob_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/printqueuejob_status.py` & `merchantapi-2.6.0/merchantapi/request/printqueuejob_status.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/printqueuejoblist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/printqueuejoblist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/printqueuelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/printqueuelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/product_copy.py` & `merchantapi-2.6.0/merchantapi/request/product_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/product_delete.py` & `merchantapi-2.6.0/merchantapi/request/product_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/product_insert.py` & `merchantapi-2.6.0/merchantapi/request/product_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/product_update.py` & `merchantapi-2.6.0/merchantapi/request/product_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productandsubscriptiontermlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/productandsubscriptiontermlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productattributeandoptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/productattributeandoptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productimage_add.py` & `merchantapi-2.6.0/merchantapi/request/productimage_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productimage_delete.py` & `merchantapi-2.6.0/merchantapi/request/productimage_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productimage_update_type.py` & `merchantapi-2.6.0/merchantapi/request/productimage_update_type.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productkit_generate_variants.py` & `merchantapi-2.6.0/merchantapi/request/productkit_generate_variants.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productkit_update_parts.py` & `merchantapi-2.6.0/merchantapi/request/productkit_update_parts.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productkit_variant_count.py` & `merchantapi-2.6.0/merchantapi/request/productkit_variant_count.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productkitlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/productkitlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productlist_adjust_inventory.py` & `merchantapi-2.6.0/merchantapi/request/productlist_adjust_inventory.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/productlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productsubscriptiontermlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/productsubscriptiontermlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/producturi_insert.py` & `merchantapi-2.6.0/merchantapi/request/producturi_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/producturi_redirect.py` & `merchantapi-2.6.0/merchantapi/request/producturi_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/producturi_update.py` & `merchantapi-2.6.0/merchantapi/request/productvariantlist_load_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,161 +2,152 @@
 This file is part of the MerchantAPI package.
 
 (c) Miva Inc <https://www.miva.com/>
 
 For the full copyright and license information, please view the LICENSE
 file that was distributed with this source code.
 
-Handles API Request ProductURI_Update. 
+Handles API Request ProductVariantList_Load_Query. 
 Scope: Store.
-:see: https://docs.miva.com/json-api/functions/producturi_update
+:see: https://docs.miva.com/json-api/functions/productvariantlist_load_query
 """
 
 import merchantapi.abstract
 import merchantapi.model
 import merchantapi.response
+from merchantapi.listquery import ListQueryRequest
 from merchantapi.client import BaseClient as Client
 from requests.models import Response as HttpResponse
 
 
-class ProductURIUpdate(merchantapi.abstract.Request):
-	def __init__(self, client: Client = None, uri: merchantapi.model.Uri = None):
+class ProductVariantListLoadQuery(ListQueryRequest):
+
+	available_search_fields = [
+		'product_code',
+		'product_name',
+		'product_sku',
+		'option_id',
+		'option_code'
+	]
+
+	def __init__(self, client: Client = None, product: merchantapi.model.Product = None):
 		"""
-		ProductURIUpdate Constructor.
+		ProductVariantListLoadQuery Constructor.
 
 		:param client: Client
-		:param uri: Uri
+		:param product: Product
 		"""
 
 		super().__init__(client)
-		self.uri_id = None
-		self.uri = None
-		self.status = None
-		self.canonical = None
-		if isinstance(uri, merchantapi.model.Uri):
-			if uri.get_id():
-				self.set_uri_id(uri.get_id())
+		self.product_id = None
+		self.product_code = None
+		self.edit_product = None
+		if isinstance(product, merchantapi.model.Product):
+			if product.get_id():
+				self.set_product_id(product.get_id())
+			elif product.get_code():
+				self.set_product_code(product.get_code())
+			elif product.get_code():
+				self.set_edit_product(product.get_code())
 
 	def get_function(self):
 		"""
 		Get the function of the request.
 
 		:returns: str
 		"""
 
-		return 'ProductURI_Update'
+		return 'ProductVariantList_Load_Query'
 
-	def get_uri_id(self) -> int:
+	def get_product_id(self) -> int:
 		"""
-		Get URI_ID.
+		Get Product_ID.
 
 		:returns: int
 		"""
 
-		return self.uri_id
+		return self.product_id
 
-	def get_uri(self) -> str:
+	def get_product_code(self) -> str:
 		"""
-		Get URI.
+		Get Product_Code.
 
 		:returns: str
 		"""
 
-		return self.uri
-
-	def get_status(self) -> int:
-		"""
-		Get Status.
-
-		:returns: int
-		"""
-
-		return self.status
+		return self.product_code
 
-	def get_canonical(self) -> bool:
+	def get_edit_product(self) -> str:
 		"""
-		Get Canonical.
+		Get Edit_Product.
 
-		:returns: bool
-		"""
-
-		return self.canonical
-
-	def set_uri_id(self, uri_id: int) -> 'ProductURIUpdate':
-		"""
-		Set URI_ID.
-
-		:param uri_id: int
-		:returns: ProductURIUpdate
+		:returns: str
 		"""
 
-		self.uri_id = uri_id
-		return self
+		return self.edit_product
 
-	def set_uri(self, uri: str) -> 'ProductURIUpdate':
+	def set_product_id(self, product_id: int) -> 'ProductVariantListLoadQuery':
 		"""
-		Set URI.
+		Set Product_ID.
 
-		:param uri: str
-		:returns: ProductURIUpdate
+		:param product_id: int
+		:returns: ProductVariantListLoadQuery
 		"""
 
-		self.uri = uri
+		self.product_id = product_id
 		return self
 
-	def set_status(self, status: int) -> 'ProductURIUpdate':
+	def set_product_code(self, product_code: str) -> 'ProductVariantListLoadQuery':
 		"""
-		Set Status.
+		Set Product_Code.
 
-		:param status: int
-		:returns: ProductURIUpdate
+		:param product_code: str
+		:returns: ProductVariantListLoadQuery
 		"""
 
-		self.status = status
+		self.product_code = product_code
 		return self
 
-	def set_canonical(self, canonical: bool) -> 'ProductURIUpdate':
+	def set_edit_product(self, edit_product: str) -> 'ProductVariantListLoadQuery':
 		"""
-		Set Canonical.
+		Set Edit_Product.
 
-		:param canonical: bool
-		:returns: ProductURIUpdate
+		:param edit_product: str
+		:returns: ProductVariantListLoadQuery
 		"""
 
-		self.canonical = canonical
+		self.edit_product = edit_product
 		return self
 
 	# noinspection PyTypeChecker
-	def send(self) -> 'merchantapi.response.ProductURIUpdate':
+	def send(self) -> 'merchantapi.response.ProductVariantListLoadQuery':
 		return super().send()
 
-	def create_response(self, http_response: HttpResponse, data) -> 'ProductURIUpdate':
+	def create_response(self, http_response: HttpResponse, data) -> 'ProductVariantListLoadQuery':
 		"""
 		Create a response object from the response data
 
 		:param http_response: requests.models.Response
 		:param data:
 		:returns: Response
 		"""
 
-		return merchantapi.response.ProductURIUpdate(self, http_response, data)
+		return merchantapi.response.ProductVariantListLoadQuery(self, http_response, data)
 
 	def to_dict(self) -> dict:
 		"""
 		Reduce the request to a dict
 
 		:override:
 		:returns: dict
 		"""
 
 		data = super().to_dict()
 
-		if self.uri_id is not None:
-			data['URI_ID'] = self.uri_id
+		if self.product_id is not None:
+			data['Product_ID'] = self.product_id
+		elif self.product_code is not None:
+			data['Product_Code'] = self.product_code
+		elif self.edit_product is not None:
+			data['Edit_Product'] = self.edit_product
 
-		if self.uri is not None:
-			data['URI'] = self.uri
-		if self.status is not None:
-			data['Status'] = self.status
-		if self.canonical is not None:
-			data['Canonical'] = self.canonical
 		return data
```

### Comparing `merchantapi-2.5.0/merchantapi/request/producturilist_delete.py` & `merchantapi-2.6.0/merchantapi/request/producturilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/producturilist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/producturilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariant_generate.py` & `merchantapi-2.6.0/merchantapi/request/productvariant_generate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariant_generate_delimiter.py` & `merchantapi-2.6.0/merchantapi/request/productvariant_generate_delimiter.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariant_insert.py` & `merchantapi-2.6.0/merchantapi/request/productvariant_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariant_update.py` & `merchantapi-2.6.0/merchantapi/request/productvariant_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariantlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/productvariantlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/productvariantlist_load_product.py` & `merchantapi-2.6.0/merchantapi/request/productvariantlist_load_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/provision_domain.py` & `merchantapi-2.6.0/merchantapi/request/provision_domain.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/provision_store.py` & `merchantapi-2.6.0/merchantapi/request/provision_store.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/relatedproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/request/relatedproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/relatedproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/relatedproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/request_builder.py` & `merchantapi-2.6.0/merchantapi/request/request_builder.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/resourcegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/resourcegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/store_load.py` & `merchantapi-2.6.0/merchantapi/request/store_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/storelist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/storelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscription_insert.py` & `merchantapi-2.6.0/merchantapi/request/subscription_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscription_update.py` & `merchantapi-2.6.0/merchantapi/request/subscription_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscriptionandorderitem_add.py` & `merchantapi-2.6.0/merchantapi/request/subscriptionandorderitem_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscriptionandorderitem_update.py` & `merchantapi-2.6.0/merchantapi/request/subscriptionandorderitem_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscriptionlist_delete.py` & `merchantapi-2.6.0/merchantapi/request/subscriptionlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscriptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/subscriptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/subscriptionshippingmethodlist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/subscriptionshippingmethodlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/uri_delete.py` & `merchantapi-2.6.0/merchantapi/request/uri_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/uri_insert.py` & `merchantapi-2.6.0/merchantapi/request/uri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/uri_update.py` & `merchantapi-2.6.0/merchantapi/request/uri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/urilist_delete.py` & `merchantapi-2.6.0/merchantapi/request/urilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/request/urilist_load_query.py` & `merchantapi-2.6.0/merchantapi/request/urilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/__init__.py` & `merchantapi-2.6.0/merchantapi/response/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,22 @@
 from .copyproductruleslist_delete import CopyProductRulesListDelete
 from .copyproductruleslist_load_query import CopyProductRulesListLoadQuery
 from .copyproductrulesmodulelist_load_query import CopyProductRulesModuleListLoadQuery
 from .copyproductrulesmodule_update_assigned import CopyProductRulesModuleUpdateAssigned
 from .copyproductrulescustomfieldlist_load_query import CopyProductRulesCustomFieldListLoadQuery
 from .copyproductrulescustomfield_update_assigned import CopyProductRulesCustomFieldUpdateAssigned
 from .orderlist_archive import OrderListArchive
+from .page_copy_branch import PageCopyBranch
+from .branchitemversionlist_load_query import BranchItemVersionListLoadQuery
+from .changesetitemversionlist_load_query import ChangesetItemVersionListLoadQuery
+from .branchpageversionlist_load_query import BranchPageVersionListLoadQuery
+from .couponbusinessaccountlist_load_query import CouponBusinessAccountListLoadQuery
+from .couponbusinessaccount_update_assigned import CouponBusinessAccountUpdateAssigned
+from .productvariantpricing_update import ProductVariantPricingUpdate
+from .productshippingrules_update import ProductShippingRulesUpdate
 from .categoryproductlist_load_query import CategoryProductListLoadQuery
 from .couponpricegrouplist_load_query import CouponPriceGroupListLoadQuery
 from .pricegroupcustomerlist_load_query import PriceGroupCustomerListLoadQuery
 from .pricegroupproductlist_load_query import PriceGroupProductListLoadQuery
 from .customerpricegrouplist_load_query import CustomerPriceGroupListLoadQuery
 from .orderpricegrouplist_load_query import OrderPriceGroupListLoadQuery
 from .ordercouponlist_load_query import OrderCouponListLoadQuery
```

### Comparing `merchantapi-2.5.0/merchantapi/response/allorderpaymentlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/allorderpaymentlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_copylinkedtemplate.py` & `merchantapi-2.6.0/merchantapi/response/attribute_copylinkedtemplate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_copytemplate.py` & `merchantapi-2.6.0/merchantapi/response/attribute_copytemplate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_delete.py` & `merchantapi-2.6.0/merchantapi/response/attribute_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_insert.py` & `merchantapi-2.6.0/merchantapi/response/attribute_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_load_code.py` & `merchantapi-2.6.0/merchantapi/response/attribute_load_code.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attribute_update.py` & `merchantapi-2.6.0/merchantapi/response/attribute_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributeandoptionlist_load_product.py` & `merchantapi-2.6.0/merchantapi/response/attributeandoptionlist_load_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplate_delete.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplate_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplate_insert.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplate_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplate_update.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplate_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_delete.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_insert.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateattribute_update.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateattribute_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateattributelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateattributelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplatelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplatelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateoption_delete.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateoption_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateoption_insert.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateoption_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateoption_set_default.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateoption_set_default.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateoption_update.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateoption_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateoptionlist_load_attribute.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateoptionlist_load_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/attributetemplateproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/attributetemplateproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroup_delete.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroup_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroup_insert.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroup_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroup_update.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroup_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupbusinessaccount_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupbusinessaccount_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupbusinessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupbusinessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygrouppaymentmethod_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygrouppaymentmethod_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupshippingmethod_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupshippingmethod_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/availabilitygroupshippingmethodlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/availabilitygroupshippingmethodlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branch_copy.py` & `merchantapi-2.6.0/merchantapi/response/branch_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branch_create.py` & `merchantapi-2.6.0/merchantapi/response/branch_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branch_delete.py` & `merchantapi-2.6.0/merchantapi/response/branch_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branch_setprimary.py` & `merchantapi-2.6.0/merchantapi/response/branch_setprimary.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branch_update.py` & `merchantapi-2.6.0/merchantapi/response/branch_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchcssresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/branchcssresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchjavascriptresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/branchjavascriptresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/branchlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/branchlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchpropertyversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/branchpropertyversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/branchtemplateversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/branchtemplateversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccount_insert.py` & `merchantapi-2.6.0/merchantapi/response/businessaccount_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccount_update.py` & `merchantapi-2.6.0/merchantapi/response/businessaccount_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccountcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/businessaccountcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccountcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/businessaccountcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccountlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/businessaccountlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/businessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/businessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/category_delete.py` & `merchantapi-2.6.0/merchantapi/response/category_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/category_insert.py` & `merchantapi-2.6.0/merchantapi/response/category_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/category_update.py` & `merchantapi-2.6.0/merchantapi/response/category_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categorylist_load_parent.py` & `merchantapi-2.6.0/merchantapi/response/categorylist_load_parent.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/categorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/categoryproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/categoryproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryuri_insert.py` & `merchantapi-2.6.0/merchantapi/response/categoryuri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryuri_redirect.py` & `merchantapi-2.6.0/merchantapi/response/categoryuri_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryuri_update.py` & `merchantapi-2.6.0/merchantapi/response/categoryuri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryurilist_delete.py` & `merchantapi-2.6.0/merchantapi/response/categoryurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/categoryurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/categoryurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changeset_create.py` & `merchantapi-2.6.0/merchantapi/response/changeset_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetchangelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesetchangelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetcssresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesetcssresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetjavascriptresourceversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesetjavascriptresourceversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesetlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetlist_merge.py` & `merchantapi-2.6.0/merchantapi/response/changesetlist_merge.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesetpropertyversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesetpropertyversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/changesettemplateversionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/changesettemplateversionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/childcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/childcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypagerules_insert.py` & `merchantapi-2.6.0/merchantapi/response/copypagerules_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypagerules_update.py` & `merchantapi-2.6.0/merchantapi/response/copypagerules_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypageruleslist_delete.py` & `merchantapi-2.6.0/merchantapi/response/copypageruleslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypageruleslist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/copypageruleslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypagerulessettings_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/copypagerulessettings_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copypagerulessettingslist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/copypagerulessettingslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrules_insert.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrules_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrules_update.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrules_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrulescustomfield_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrulescustomfield_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrulescustomfieldlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrulescustomfieldlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductruleslist_delete.py` & `merchantapi-2.6.0/merchantapi/response/copyproductruleslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductruleslist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/copyproductruleslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrulesmodule_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrulesmodule_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/copyproductrulesmodulelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/copyproductrulesmodulelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/coupon_insert.py` & `merchantapi-2.6.0/merchantapi/response/coupon_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/coupon_update.py` & `merchantapi-2.6.0/merchantapi/response/coupon_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/couponcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/couponcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/couponlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/couponlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponpricegroup_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/couponpricegroup_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/couponpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/couponpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/cssresource_delete.py` & `merchantapi-2.6.0/merchantapi/response/cssresource_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/cssresource_insert.py` & `merchantapi-2.6.0/merchantapi/response/cssresource_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/cssresource_update.py` & `merchantapi-2.6.0/merchantapi/response/cssresource_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/cssresourcelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/cssresourcelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customer_delete.py` & `merchantapi-2.6.0/merchantapi/response/customer_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customer_insert.py` & `merchantapi-2.6.0/merchantapi/response/customer_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customer_update.py` & `merchantapi-2.6.0/merchantapi/response/customer_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddress_delete.py` & `merchantapi-2.6.0/merchantapi/response/customeraddress_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddress_insert.py` & `merchantapi-2.6.0/merchantapi/response/customeraddress_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddress_update.py` & `merchantapi-2.6.0/merchantapi/response/customeraddress_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddress_update_residential.py` & `merchantapi-2.6.0/merchantapi/response/customeraddress_update_residential.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddresslist_delete.py` & `merchantapi-2.6.0/merchantapi/response/customeraddresslist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customeraddresslist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customeraddresslist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customercredithistory_delete.py` & `merchantapi-2.6.0/merchantapi/response/customercredithistory_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customercredithistory_insert.py` & `merchantapi-2.6.0/merchantapi/response/customercredithistory_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customercredithistorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customercredithistorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customerpaymentcard_register.py` & `merchantapi-2.6.0/merchantapi/response/customerpaymentcard_register.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customerpaymentcardlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customerpaymentcardlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customerpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customerpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/customersubscriptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/customersubscriptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/feeduri_insert.py` & `merchantapi-2.6.0/merchantapi/response/feeduri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/feeduri_update.py` & `merchantapi-2.6.0/merchantapi/response/feeduri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/feedurilist_delete.py` & `merchantapi-2.6.0/merchantapi/response/feedurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/feedurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/feedurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/imagetypelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/imagetypelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/inventoryproductsettings_update.py` & `merchantapi-2.6.0/merchantapi/response/inventoryproductsettings_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/javascriptresource_delete.py` & `merchantapi-2.6.0/merchantapi/response/javascriptresource_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/javascriptresource_insert.py` & `merchantapi-2.6.0/merchantapi/response/javascriptresource_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/javascriptresource_update.py` & `merchantapi-2.6.0/merchantapi/response/javascriptresource_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/javascriptresourcelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/javascriptresourcelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/mivamerchantversion.py` & `merchantapi-2.6.0/merchantapi/response/mivamerchantversion.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/module.py` & `merchantapi-2.6.0/merchantapi/response/module.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/note_delete.py` & `merchantapi-2.6.0/merchantapi/response/note_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/note_insert.py` & `merchantapi-2.6.0/merchantapi/response/note_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/note_update.py` & `merchantapi-2.6.0/merchantapi/response/note_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/notelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/notelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/option_delete.py` & `merchantapi-2.6.0/merchantapi/response/option_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/option_insert.py` & `merchantapi-2.6.0/merchantapi/response/option_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/option_load_code.py` & `merchantapi-2.6.0/merchantapi/response/option_load_code.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/option_set_default.py` & `merchantapi-2.6.0/merchantapi/response/option_set_default.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/option_update.py` & `merchantapi-2.6.0/merchantapi/response/option_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/optionlist_load_attribute.py` & `merchantapi-2.6.0/merchantapi/response/optionlist_load_attribute.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/order_authorize.py` & `merchantapi-2.6.0/merchantapi/response/order_authorize.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/order_create.py` & `merchantapi-2.6.0/merchantapi/response/order_create.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/order_create_fromorder.py` & `merchantapi-2.6.0/merchantapi/response/order_create_fromorder.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/order_delete.py` & `merchantapi-2.6.0/merchantapi/response/order_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/order_update_customer_information.py` & `merchantapi-2.6.0/merchantapi/response/order_update_customer_information.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordercoupon_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/ordercoupon_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordercouponlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/ordercouponlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordercustomfieldlist_load.py` & `merchantapi-2.6.0/merchantapi/response/ordercustomfieldlist_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordercustomfields_update.py` & `merchantapi-2.6.0/merchantapi/response/ordercustomfields_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitem_add.py` & `merchantapi-2.6.0/merchantapi/response/orderitem_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitem_split.py` & `merchantapi-2.6.0/merchantapi/response/orderitem_split.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitem_update.py` & `merchantapi-2.6.0/merchantapi/response/orderitem_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_backorder.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_backorder.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_cancel.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_cancel.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_createreturn.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_createreturn.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_createshipment.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_createshipment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderitemlist_removefromshipment.py` & `merchantapi-2.6.0/merchantapi/response/orderitemlist_removefromshipment.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderlist_archive.py` & `merchantapi-2.6.0/merchantapi/response/orderlist_archive.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/orderlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderpayment_capture.py` & `merchantapi-2.6.0/merchantapi/response/orderpayment_capture.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderpayment_refund.py` & `merchantapi-2.6.0/merchantapi/response/orderpayment_refund.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderpayment_void.py` & `merchantapi-2.6.0/merchantapi/response/orderpayment_void.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderpricegroup_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/orderpricegroup_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderpricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/orderpricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/orderreturnlist_received.py` & `merchantapi-2.6.0/merchantapi/response/orderreturnlist_received.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordershipmentlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/ordershipmentlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/ordershipmentlist_update.py` & `merchantapi-2.6.0/merchantapi/response/ordershipmentlist_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/page_copy.py` & `merchantapi-2.6.0/merchantapi/response/page_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/page_delete.py` & `merchantapi-2.6.0/merchantapi/response/page_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/page_insert.py` & `merchantapi-2.6.0/merchantapi/response/page_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/page_update.py` & `merchantapi-2.6.0/merchantapi/response/page_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pagelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pagelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pageuri_insert.py` & `merchantapi-2.6.0/merchantapi/response/pageuri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pageuri_redirect.py` & `merchantapi-2.6.0/merchantapi/response/pageuri_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pageuri_update.py` & `merchantapi-2.6.0/merchantapi/response/pageuri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pageurilist_delete.py` & `merchantapi-2.6.0/merchantapi/response/pageurilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pageurilist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pageurilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/paymentmethodlist_load.py` & `merchantapi-2.6.0/merchantapi/response/paymentmethodlist_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroup_delete.py` & `merchantapi-2.6.0/merchantapi/response/pricegroup_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroup_insert.py` & `merchantapi-2.6.0/merchantapi/response/pricegroup_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroup_update.py` & `merchantapi-2.6.0/merchantapi/response/pricegroup_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupbusinessaccount_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupbusinessaccount_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupbusinessaccountlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupbusinessaccountlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupcustomer_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupcustomer_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupcustomerlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupcustomerlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupexcludedcategory_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupexcludedcategory_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupexcludedcategorylist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupexcludedcategorylist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupexcludedproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupexcludedproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupexcludedproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupexcludedproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupqualifyingproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupqualifyingproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/pricegroupqualifyingproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/pricegroupqualifyingproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/printqueuejob_delete.py` & `merchantapi-2.6.0/merchantapi/response/printqueuejob_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/printqueuejob_insert.py` & `merchantapi-2.6.0/merchantapi/response/printqueuejob_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/printqueuejob_status.py` & `merchantapi-2.6.0/merchantapi/response/printqueuejob_status.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/printqueuejoblist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/printqueuejoblist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/printqueuelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/printqueuelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/product_copy.py` & `merchantapi-2.6.0/merchantapi/response/product_copy.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/product_delete.py` & `merchantapi-2.6.0/merchantapi/response/product_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/product_insert.py` & `merchantapi-2.6.0/merchantapi/response/product_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/product_update.py` & `merchantapi-2.6.0/merchantapi/response/product_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productandsubscriptiontermlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productandsubscriptiontermlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productattributeandoptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productattributeandoptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productimage_add.py` & `merchantapi-2.6.0/merchantapi/response/productimage_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productimage_delete.py` & `merchantapi-2.6.0/merchantapi/response/productimage_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productimage_update_type.py` & `merchantapi-2.6.0/merchantapi/response/productimage_update_type.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productkit_generate_variants.py` & `merchantapi-2.6.0/merchantapi/response/productkit_generate_variants.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productkit_update_parts.py` & `merchantapi-2.6.0/merchantapi/response/productkit_update_parts.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productkit_variant_count.py` & `merchantapi-2.6.0/merchantapi/response/productkit_variant_count.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productkitlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productkitlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productlist_adjust_inventory.py` & `merchantapi-2.6.0/merchantapi/response/productlist_adjust_inventory.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productsubscriptiontermlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productsubscriptiontermlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/producturi_insert.py` & `merchantapi-2.6.0/merchantapi/response/producturi_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/producturi_redirect.py` & `merchantapi-2.6.0/merchantapi/response/producturi_redirect.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/producturi_update.py` & `merchantapi-2.6.0/merchantapi/response/producturi_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/producturilist_delete.py` & `merchantapi-2.6.0/merchantapi/response/producturilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/producturilist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/producturilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariant_generate.py` & `merchantapi-2.6.0/merchantapi/response/productvariant_generate.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariant_generate_delimiter.py` & `merchantapi-2.6.0/merchantapi/response/productvariant_generate_delimiter.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariant_insert.py` & `merchantapi-2.6.0/merchantapi/response/productvariant_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariant_update.py` & `merchantapi-2.6.0/merchantapi/response/productvariant_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariantlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/productvariantlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariantlist_load_product.py` & `merchantapi-2.6.0/merchantapi/response/productvariantlist_load_product.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/productvariantlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/productvariantlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/provision_domain.py` & `merchantapi-2.6.0/merchantapi/response/provision_domain.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/provision_store.py` & `merchantapi-2.6.0/merchantapi/response/provision_store.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/relatedproduct_update_assigned.py` & `merchantapi-2.6.0/merchantapi/response/relatedproduct_update_assigned.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/relatedproductlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/relatedproductlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/resourcegrouplist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/resourcegrouplist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/store_load.py` & `merchantapi-2.6.0/merchantapi/response/store_load.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/storelist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/storelist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscription_insert.py` & `merchantapi-2.6.0/merchantapi/response/subscription_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscription_update.py` & `merchantapi-2.6.0/merchantapi/response/subscription_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscriptionandorderitem_add.py` & `merchantapi-2.6.0/merchantapi/response/subscriptionandorderitem_add.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscriptionandorderitem_update.py` & `merchantapi-2.6.0/merchantapi/response/subscriptionandorderitem_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscriptionlist_delete.py` & `merchantapi-2.6.0/merchantapi/response/subscriptionlist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscriptionlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/subscriptionlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/subscriptionshippingmethodlist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/subscriptionshippingmethodlist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/uri_delete.py` & `merchantapi-2.6.0/merchantapi/response/uri_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/uri_insert.py` & `merchantapi-2.6.0/merchantapi/response/uri_insert.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/uri_update.py` & `merchantapi-2.6.0/merchantapi/response/uri_update.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/urilist_delete.py` & `merchantapi-2.6.0/merchantapi/response/urilist_delete.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/response/urilist_load_query.py` & `merchantapi-2.6.0/merchantapi/response/urilist_load_query.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi/sshagent.py` & `merchantapi-2.6.0/merchantapi/sshagent.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/merchantapi.egg-info/PKG-INFO` & `merchantapi-2.6.0/merchantapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merchantapi
-Version: 2.5.0
+Version: 2.6.0
 Summary: Miva Merchant JSON API SDK
 Home-page: https://www.miva.com
 Author: Miva, Inc.
 Author-email: support@miva.com
 License: Miva SDK License Agreement
 Description: # Miva Merchant API SDK for Python (3.x)
         
@@ -30,15 +30,15 @@
             
         *Note: On some operating systems the `pip` program may be named `pip3`*
         
         # Adding as a dependency in your packages
         
         You can also add it to your project's `requirements.txt` file:
         
-            merchantapi>=2.5.0
+            merchantapi>=2.6.0
             
         Then install
         
             pip install -r requirements.txt
             
         *Note: On some operating systems the `pip` program may be named `pip3`*
```

### Comparing `merchantapi-2.5.0/merchantapi.egg-info/SOURCES.txt` & `merchantapi-2.6.0/merchantapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,34 +28,38 @@
 merchantapi/model/availability_group_category.py
 merchantapi/model/availability_group_customer.py
 merchantapi/model/availability_group_product.py
 merchantapi/model/availability_group_shipping_method.py
 merchantapi/model/branch.py
 merchantapi/model/branch_css_resource.py
 merchantapi/model/branch_css_resource_version.py
+merchantapi/model/branch_item_version.py
 merchantapi/model/branch_javascript_resource_version.py
+merchantapi/model/branch_page_version.py
 merchantapi/model/branch_property_version.py
 merchantapi/model/branch_template_version.py
 merchantapi/model/business_account.py
 merchantapi/model/business_account_customer.py
 merchantapi/model/category.py
 merchantapi/model/category_product.py
 merchantapi/model/changeset.py
 merchantapi/model/changeset_change.py
 merchantapi/model/changeset_css_resource.py
 merchantapi/model/changeset_css_resource_version.py
+merchantapi/model/changeset_item_version.py
 merchantapi/model/changeset_javascript_resource_version.py
 merchantapi/model/changeset_property_version.py
 merchantapi/model/changeset_template_version.py
 merchantapi/model/copy_page_rule.py
 merchantapi/model/copy_page_rules_settings.py
 merchantapi/model/copy_product_rule.py
 merchantapi/model/copy_product_rules_custom_field.py
 merchantapi/model/copy_product_rules_module.py
 merchantapi/model/coupon.py
+merchantapi/model/coupon_business_account.py
 merchantapi/model/coupon_customer.py
 merchantapi/model/coupon_price_group.py
 merchantapi/model/css_resource.py
 merchantapi/model/css_resource_attribute.py
 merchantapi/model/css_resource_change.py
 merchantapi/model/css_resource_version.py
 merchantapi/model/css_resource_version_attribute.py
@@ -141,14 +145,15 @@
 merchantapi/model/property_version.py
 merchantapi/model/provision_message.py
 merchantapi/model/received_return.py
 merchantapi/model/related_product.py
 merchantapi/model/resource_attribute.py
 merchantapi/model/resource_group.py
 merchantapi/model/resource_group_change.py
+merchantapi/model/shipping_rule_method.py
 merchantapi/model/split_order_item.py
 merchantapi/model/store.py
 merchantapi/model/subscription.py
 merchantapi/model/subscription_attribute.py
 merchantapi/model/subscription_option.py
 merchantapi/model/subscription_shipping_method.py
 merchantapi/model/template_change.py
@@ -199,17 +204,19 @@
 merchantapi/request/availabilitygroupshippingmethodlist_load_query.py
 merchantapi/request/branch_copy.py
 merchantapi/request/branch_create.py
 merchantapi/request/branch_delete.py
 merchantapi/request/branch_setprimary.py
 merchantapi/request/branch_update.py
 merchantapi/request/branchcssresourceversionlist_load_query.py
+merchantapi/request/branchitemversionlist_load_query.py
 merchantapi/request/branchjavascriptresourceversionlist_load_query.py
 merchantapi/request/branchlist_delete.py
 merchantapi/request/branchlist_load_query.py
+merchantapi/request/branchpageversionlist_load_query.py
 merchantapi/request/branchpropertyversionlist_load_query.py
 merchantapi/request/branchtemplateversionlist_load_query.py
 merchantapi/request/businessaccount_insert.py
 merchantapi/request/businessaccount_update.py
 merchantapi/request/businessaccountcustomer_update_assigned.py
 merchantapi/request/businessaccountcustomerlist_load_query.py
 merchantapi/request/businessaccountlist_delete.py
@@ -225,14 +232,15 @@
 merchantapi/request/categoryuri_redirect.py
 merchantapi/request/categoryuri_update.py
 merchantapi/request/categoryurilist_delete.py
 merchantapi/request/categoryurilist_load_query.py
 merchantapi/request/changeset_create.py
 merchantapi/request/changesetchangelist_load_query.py
 merchantapi/request/changesetcssresourceversionlist_load_query.py
+merchantapi/request/changesetitemversionlist_load_query.py
 merchantapi/request/changesetjavascriptresourceversionlist_load_query.py
 merchantapi/request/changesetlist_load_query.py
 merchantapi/request/changesetlist_merge.py
 merchantapi/request/changesetpropertyversionlist_load_query.py
 merchantapi/request/changesettemplateversionlist_load_query.py
 merchantapi/request/childcategorylist_load_query.py
 merchantapi/request/copypagerules_insert.py
@@ -247,14 +255,16 @@
 merchantapi/request/copyproductrulescustomfieldlist_load_query.py
 merchantapi/request/copyproductruleslist_delete.py
 merchantapi/request/copyproductruleslist_load_query.py
 merchantapi/request/copyproductrulesmodule_update_assigned.py
 merchantapi/request/copyproductrulesmodulelist_load_query.py
 merchantapi/request/coupon_insert.py
 merchantapi/request/coupon_update.py
+merchantapi/request/couponbusinessaccount_update_assigned.py
+merchantapi/request/couponbusinessaccountlist_load_query.py
 merchantapi/request/couponcustomer_update_assigned.py
 merchantapi/request/couponcustomerlist_load_query.py
 merchantapi/request/couponlist_delete.py
 merchantapi/request/couponlist_load_query.py
 merchantapi/request/couponpricegroup_update_assigned.py
 merchantapi/request/couponpricegrouplist_load_query.py
 merchantapi/request/cssresource_delete.py
@@ -325,14 +335,15 @@
 merchantapi/request/orderpayment_void.py
 merchantapi/request/orderpricegroup_update_assigned.py
 merchantapi/request/orderpricegrouplist_load_query.py
 merchantapi/request/orderreturnlist_received.py
 merchantapi/request/ordershipmentlist_load_query.py
 merchantapi/request/ordershipmentlist_update.py
 merchantapi/request/page_copy.py
+merchantapi/request/page_copy_branch.py
 merchantapi/request/page_delete.py
 merchantapi/request/page_insert.py
 merchantapi/request/page_update.py
 merchantapi/request/pagelist_load_query.py
 merchantapi/request/pageuri_insert.py
 merchantapi/request/pageuri_redirect.py
 merchantapi/request/pageuri_update.py
@@ -373,27 +384,29 @@
 merchantapi/request/productimage_update_type.py
 merchantapi/request/productkit_generate_variants.py
 merchantapi/request/productkit_update_parts.py
 merchantapi/request/productkit_variant_count.py
 merchantapi/request/productkitlist_load_query.py
 merchantapi/request/productlist_adjust_inventory.py
 merchantapi/request/productlist_load_query.py
+merchantapi/request/productshippingrules_update.py
 merchantapi/request/productsubscriptiontermlist_load_query.py
 merchantapi/request/producturi_insert.py
 merchantapi/request/producturi_redirect.py
 merchantapi/request/producturi_update.py
 merchantapi/request/producturilist_delete.py
 merchantapi/request/producturilist_load_query.py
 merchantapi/request/productvariant_generate.py
 merchantapi/request/productvariant_generate_delimiter.py
 merchantapi/request/productvariant_insert.py
 merchantapi/request/productvariant_update.py
 merchantapi/request/productvariantlist_delete.py
 merchantapi/request/productvariantlist_load_product.py
 merchantapi/request/productvariantlist_load_query.py
+merchantapi/request/productvariantpricing_update.py
 merchantapi/request/provision_domain.py
 merchantapi/request/provision_store.py
 merchantapi/request/relatedproduct_update_assigned.py
 merchantapi/request/relatedproductlist_load_query.py
 merchantapi/request/request_builder.py
 merchantapi/request/resourcegrouplist_load_query.py
 merchantapi/request/store_load.py
@@ -451,17 +464,19 @@
 merchantapi/response/availabilitygroupshippingmethodlist_load_query.py
 merchantapi/response/branch_copy.py
 merchantapi/response/branch_create.py
 merchantapi/response/branch_delete.py
 merchantapi/response/branch_setprimary.py
 merchantapi/response/branch_update.py
 merchantapi/response/branchcssresourceversionlist_load_query.py
+merchantapi/response/branchitemversionlist_load_query.py
 merchantapi/response/branchjavascriptresourceversionlist_load_query.py
 merchantapi/response/branchlist_delete.py
 merchantapi/response/branchlist_load_query.py
+merchantapi/response/branchpageversionlist_load_query.py
 merchantapi/response/branchpropertyversionlist_load_query.py
 merchantapi/response/branchtemplateversionlist_load_query.py
 merchantapi/response/businessaccount_insert.py
 merchantapi/response/businessaccount_update.py
 merchantapi/response/businessaccountcustomer_update_assigned.py
 merchantapi/response/businessaccountcustomerlist_load_query.py
 merchantapi/response/businessaccountlist_delete.py
@@ -477,14 +492,15 @@
 merchantapi/response/categoryuri_redirect.py
 merchantapi/response/categoryuri_update.py
 merchantapi/response/categoryurilist_delete.py
 merchantapi/response/categoryurilist_load_query.py
 merchantapi/response/changeset_create.py
 merchantapi/response/changesetchangelist_load_query.py
 merchantapi/response/changesetcssresourceversionlist_load_query.py
+merchantapi/response/changesetitemversionlist_load_query.py
 merchantapi/response/changesetjavascriptresourceversionlist_load_query.py
 merchantapi/response/changesetlist_load_query.py
 merchantapi/response/changesetlist_merge.py
 merchantapi/response/changesetpropertyversionlist_load_query.py
 merchantapi/response/changesettemplateversionlist_load_query.py
 merchantapi/response/childcategorylist_load_query.py
 merchantapi/response/copypagerules_insert.py
@@ -499,14 +515,16 @@
 merchantapi/response/copyproductrulescustomfieldlist_load_query.py
 merchantapi/response/copyproductruleslist_delete.py
 merchantapi/response/copyproductruleslist_load_query.py
 merchantapi/response/copyproductrulesmodule_update_assigned.py
 merchantapi/response/copyproductrulesmodulelist_load_query.py
 merchantapi/response/coupon_insert.py
 merchantapi/response/coupon_update.py
+merchantapi/response/couponbusinessaccount_update_assigned.py
+merchantapi/response/couponbusinessaccountlist_load_query.py
 merchantapi/response/couponcustomer_update_assigned.py
 merchantapi/response/couponcustomerlist_load_query.py
 merchantapi/response/couponlist_delete.py
 merchantapi/response/couponlist_load_query.py
 merchantapi/response/couponpricegroup_update_assigned.py
 merchantapi/response/couponpricegrouplist_load_query.py
 merchantapi/response/cssresource_delete.py
@@ -577,14 +595,15 @@
 merchantapi/response/orderpayment_void.py
 merchantapi/response/orderpricegroup_update_assigned.py
 merchantapi/response/orderpricegrouplist_load_query.py
 merchantapi/response/orderreturnlist_received.py
 merchantapi/response/ordershipmentlist_load_query.py
 merchantapi/response/ordershipmentlist_update.py
 merchantapi/response/page_copy.py
+merchantapi/response/page_copy_branch.py
 merchantapi/response/page_delete.py
 merchantapi/response/page_insert.py
 merchantapi/response/page_update.py
 merchantapi/response/pagelist_load_query.py
 merchantapi/response/pageuri_insert.py
 merchantapi/response/pageuri_redirect.py
 merchantapi/response/pageuri_update.py
@@ -625,27 +644,29 @@
 merchantapi/response/productimage_update_type.py
 merchantapi/response/productkit_generate_variants.py
 merchantapi/response/productkit_update_parts.py
 merchantapi/response/productkit_variant_count.py
 merchantapi/response/productkitlist_load_query.py
 merchantapi/response/productlist_adjust_inventory.py
 merchantapi/response/productlist_load_query.py
+merchantapi/response/productshippingrules_update.py
 merchantapi/response/productsubscriptiontermlist_load_query.py
 merchantapi/response/producturi_insert.py
 merchantapi/response/producturi_redirect.py
 merchantapi/response/producturi_update.py
 merchantapi/response/producturilist_delete.py
 merchantapi/response/producturilist_load_query.py
 merchantapi/response/productvariant_generate.py
 merchantapi/response/productvariant_generate_delimiter.py
 merchantapi/response/productvariant_insert.py
 merchantapi/response/productvariant_update.py
 merchantapi/response/productvariantlist_delete.py
 merchantapi/response/productvariantlist_load_product.py
 merchantapi/response/productvariantlist_load_query.py
+merchantapi/response/productvariantpricing_update.py
 merchantapi/response/provision_domain.py
 merchantapi/response/provision_store.py
 merchantapi/response/relatedproduct_update_assigned.py
 merchantapi/response/relatedproductlist_load_query.py
 merchantapi/response/request_builder.py
 merchantapi/response/resourcegrouplist_load_query.py
 merchantapi/response/store_load.py
@@ -703,17 +724,19 @@
 tests/availabilitygroupshippingmethodlist_load_query_test.py
 tests/branch_copy_test.py
 tests/branch_create_test.py
 tests/branch_delete_test.py
 tests/branch_setprimary_test.py
 tests/branch_update_test.py
 tests/branchcssresourceversionlist_load_query_test.py
+tests/branchitemversionlist_load_query_test.py
 tests/branchjavascriptresourceversionlist_load_query_test.py
 tests/branchlist_delete_test.py
 tests/branchlist_load_query_test.py
+tests/branchpageversionlist_load_query_test.py
 tests/branchpropertyversionlist_load_query_test.py
 tests/branchtemplateversionlist_load_query_test.py
 tests/businessaccount_insert_test.py
 tests/businessaccount_update_test.py
 tests/businessaccountcustomer_update_assigned_test.py
 tests/businessaccountcustomerlist_load_query_test.py
 tests/businessaccountlist_delete_test.py
@@ -729,14 +752,15 @@
 tests/categoryuri_redirect_test.py
 tests/categoryuri_update_test.py
 tests/categoryurilist_delete_test.py
 tests/categoryurilist_load_query_test.py
 tests/changeset_create_test.py
 tests/changesetchangelist_load_query_test.py
 tests/changesetcssresourceversionlist_load_query_test.py
+tests/changesetitemversionlist_load_query_test.py
 tests/changesetjavascriptresourceversionlist_load_query_test.py
 tests/changesetlist_load_query_test.py
 tests/changesetlist_merge_test.py
 tests/changesetpropertyversionlist_load_query_test.py
 tests/changesettemplateversionlist_load_query_test.py
 tests/childcategorylist_load_query_test.py
 tests/client.py
@@ -753,14 +777,16 @@
 tests/copyproductrulescustomfieldlist_load_query_test.py
 tests/copyproductruleslist_delete_test.py
 tests/copyproductruleslist_load_query_test.py
 tests/copyproductrulesmodule_update_assigned_test.py
 tests/copyproductrulesmodulelist_load_query_test.py
 tests/coupon_insert_test.py
 tests/coupon_update_test.py
+tests/couponbusinessaccountList_load_query_test.py
+tests/couponbusinessaccount_update_assigned_test.py
 tests/couponcustomer_update_assigned_test.py
 tests/couponcustomerlist_load_query_test.py
 tests/couponlist_delete_test.py
 tests/couponlist_load_query_test.py
 tests/couponpricegroup_update_assigned_test.py
 tests/couponpricegrouplist_load_query_test.py
 tests/credentials.py.dist
@@ -829,14 +855,15 @@
 tests/orderitemlist_removefromshipment_test.py
 tests/orderlist_archive_test.py
 tests/orderlist_load_query_test.py
 tests/orderpricegroup_update_assigned_test.py
 tests/orderpricegrouplist_load_query_test.py
 tests/ordershipmentlist_load_query_test.py
 tests/ordershipmentlist_update_test.py
+tests/page_copy_branch_test.py
 tests/page_copy_test.py
 tests/page_delete_test.py
 tests/page_insert_test.py
 tests/page_update_test.py
 tests/pagelist_load_query_test.py
 tests/pageuri_insert_test.py
 tests/pageuri_redirect_test.py
@@ -878,27 +905,29 @@
 tests/productimage_update_type_test.py
 tests/productkit_generate_variants_test.py
 tests/productkit_update_parts_test.py
 tests/productkit_variant_count_test.py
 tests/productkitlist_load_query_test.py
 tests/productlist_adjust_inventory_test.py
 tests/productlist_load_query_test.py
+tests/productshippingrules_update_test.py
 tests/productsubscriptiontermlist_load_query_test.py
 tests/producturi_insert_test.py
 tests/producturi_redirect_test.py
 tests/producturi_update_test.py
 tests/producturilist_delete_test.py
 tests/producturilist_load_query_test.py
 tests/productvariant_generate_delimiter_test.py
 tests/productvariant_generate_test.py
 tests/productvariant_insert_test.py
 tests/productvariant_update_test.py
 tests/productvariantlist_delete_test.py
 tests/productvariantlist_load_product_test.py
 tests/productvariantlist_load_query_test.py
+tests/productvariantpricing_update_test.py
 tests/relatedproduct_update_assigned_test.py
 tests/relatedproductlist_load_query_test.py
 tests/request_builder_test.py
 tests/resourcegrouplist_load_query_test.py
 tests/store_load_test.py
 tests/storelist_load_query_test.py
 tests/subscription_insert_test.py
```

### Comparing `merchantapi-2.5.0/setup.py` & `merchantapi-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/allorderpaymentlist_load_query_test.py` & `merchantapi-2.6.0/tests/allorderpaymentlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_copylinkedtemplate_test.py` & `merchantapi-2.6.0/tests/attribute_copylinkedtemplate_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_copytemplate_test.py` & `merchantapi-2.6.0/tests/attribute_copytemplate_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_delete_test.py` & `merchantapi-2.6.0/tests/attribute_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_insert_test.py` & `merchantapi-2.6.0/tests/attribute_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_load_code_test.py` & `merchantapi-2.6.0/tests/attribute_load_code_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attribute_update_test.py` & `merchantapi-2.6.0/tests/attribute_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributeandoptionlist_load_product_test.py` & `merchantapi-2.6.0/tests/attributeandoptionlist_load_product_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplate_delete_test.py` & `merchantapi-2.6.0/tests/attributetemplate_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplate_insert_test.py` & `merchantapi-2.6.0/tests/attributetemplate_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplate_update_test.py` & `merchantapi-2.6.0/tests/attributetemplate_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateattribute_delete_test.py` & `merchantapi-2.6.0/tests/attributetemplateattribute_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateattribute_insert_test.py` & `merchantapi-2.6.0/tests/attributetemplateattribute_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateattribute_update_test.py` & `merchantapi-2.6.0/tests/attributetemplateattribute_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateattributelist_load_query_test.py` & `merchantapi-2.6.0/tests/attributetemplateattributelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplatelist_load_query_test.py` & `merchantapi-2.6.0/tests/attributetemplatelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateoption_delete_test.py` & `merchantapi-2.6.0/tests/attributetemplateoption_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateoption_insert_test.py` & `merchantapi-2.6.0/tests/attributetemplateoption_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateoption_set_default_test.py` & `merchantapi-2.6.0/tests/attributetemplateoption_set_default_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateoption_update_test.py` & `merchantapi-2.6.0/tests/attributetemplateoption_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateoptionlist_load_attribute_test.py` & `merchantapi-2.6.0/tests/attributetemplateoptionlist_load_attribute_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/attributetemplateproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/attributetemplateproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/attributetemplateproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroup_delete_test.py` & `merchantapi-2.6.0/tests/availabilitygroup_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroup_insert_test.py` & `merchantapi-2.6.0/tests/availabilitygroup_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroup_update_test.py` & `merchantapi-2.6.0/tests/availabilitygroup_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupbusinessaccount_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygroupbusinessaccount_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupbusinessaccountlist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygroupbusinessaccountlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupcategory_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygroupcategory_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupcategorylist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygroupcategorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupcustomer_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygroupcustomer_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupcustomerlist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygroupcustomerlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygrouppaymentmethod_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygrouppaymentmethod_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygroupproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygroupproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupshippingmethod_update_assigned_test.py` & `merchantapi-2.6.0/tests/availabilitygroupshippingmethod_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/availabilitygroupshippingmethodlist_load_query_test.py` & `merchantapi-2.6.0/tests/availabilitygroupshippingmethodlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branch_copy_test.py` & `merchantapi-2.6.0/tests/branch_copy_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branch_create_test.py` & `merchantapi-2.6.0/tests/branch_create_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branch_delete_test.py` & `merchantapi-2.6.0/tests/branch_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branch_setprimary_test.py` & `merchantapi-2.6.0/tests/branch_setprimary_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branch_update_test.py` & `merchantapi-2.6.0/tests/branch_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchcssresourceversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/branchcssresourceversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchjavascriptresourceversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/branchjavascriptresourceversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchlist_delete_test.py` & `merchantapi-2.6.0/tests/branchlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchlist_load_query_test.py` & `merchantapi-2.6.0/tests/branchlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchpropertyversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/branchpropertyversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/branchtemplateversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/branchtemplateversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccount_insert_test.py` & `merchantapi-2.6.0/tests/businessaccount_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccount_update_test.py` & `merchantapi-2.6.0/tests/businessaccount_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccountcustomer_update_assigned_test.py` & `merchantapi-2.6.0/tests/businessaccountcustomer_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccountcustomerlist_load_query_test.py` & `merchantapi-2.6.0/tests/businessaccountcustomerlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccountlist_delete_test.py` & `merchantapi-2.6.0/tests/businessaccountlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/businessaccountlist_load_query_test.py` & `merchantapi-2.6.0/tests/businessaccountlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/category_delete_test.py` & `merchantapi-2.6.0/tests/category_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/category_insert_test.py` & `merchantapi-2.6.0/tests/category_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/category_update_test.py` & `merchantapi-2.6.0/tests/category_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categorylist_load_parent_test.py` & `merchantapi-2.6.0/tests/categorylist_load_parent_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categorylist_load_query_test.py` & `merchantapi-2.6.0/tests/categorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/categoryproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/categoryproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryuri_insert_test.py` & `merchantapi-2.6.0/tests/categoryuri_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryuri_redirect_test.py` & `merchantapi-2.6.0/tests/categoryuri_redirect_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryuri_update_test.py` & `merchantapi-2.6.0/tests/categoryuri_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryurilist_delete_test.py` & `merchantapi-2.6.0/tests/categoryurilist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/categoryurilist_load_query_test.py` & `merchantapi-2.6.0/tests/categoryurilist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changeset_create_test.py` & `merchantapi-2.6.0/tests/changeset_create_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetchangelist_load_query_test.py` & `merchantapi-2.6.0/tests/changesetchangelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetcssresourceversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/changesetcssresourceversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetjavascriptresourceversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/changesetjavascriptresourceversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetlist_load_query_test.py` & `merchantapi-2.6.0/tests/changesetlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetlist_merge_test.py` & `merchantapi-2.6.0/tests/changesetlist_merge_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesetpropertyversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/changesetpropertyversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/changesettemplateversionlist_load_query_test.py` & `merchantapi-2.6.0/tests/changesettemplateversionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/childcategorylist_load_query_test.py` & `merchantapi-2.6.0/tests/childcategorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/client.py` & `merchantapi-2.6.0/tests/client.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/conftest.py` & `merchantapi-2.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypagerules_insert_test.py` & `merchantapi-2.6.0/tests/copypagerules_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypagerules_update_test.py` & `merchantapi-2.6.0/tests/copypagerules_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypageruleslist_delete_test.py` & `merchantapi-2.6.0/tests/copypageruleslist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypageruleslist_load_query_test.py` & `merchantapi-2.6.0/tests/copypageruleslist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypagerulessettings_update_assigned_test.py` & `merchantapi-2.6.0/tests/copypagerulessettings_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copypagerulessettingslist_load_query_test.py` & `merchantapi-2.6.0/tests/copypagerulessettingslist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrules_insert_test.py` & `merchantapi-2.6.0/tests/copyproductrules_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrules_update_test.py` & `merchantapi-2.6.0/tests/copyproductrules_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrulescustomfield_update_assigned_test.py` & `merchantapi-2.6.0/tests/copyproductrulescustomfield_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrulescustomfieldlist_load_query_test.py` & `merchantapi-2.6.0/tests/copyproductrulescustomfieldlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductruleslist_delete_test.py` & `merchantapi-2.6.0/tests/copyproductruleslist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductruleslist_load_query_test.py` & `merchantapi-2.6.0/tests/copyproductruleslist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrulesmodule_update_assigned_test.py` & `merchantapi-2.6.0/tests/copyproductrulesmodule_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/copyproductrulesmodulelist_load_query_test.py` & `merchantapi-2.6.0/tests/copyproductrulesmodulelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/coupon_insert_test.py` & `merchantapi-2.6.0/tests/coupon_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/coupon_update_test.py` & `merchantapi-2.6.0/tests/coupon_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponcustomer_update_assigned_test.py` & `merchantapi-2.6.0/tests/couponcustomer_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponcustomerlist_load_query_test.py` & `merchantapi-2.6.0/tests/couponcustomerlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponlist_delete_test.py` & `merchantapi-2.6.0/tests/couponlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponlist_load_query_test.py` & `merchantapi-2.6.0/tests/couponlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponpricegroup_update_assigned_test.py` & `merchantapi-2.6.0/tests/couponpricegroup_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/couponpricegrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/couponpricegrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/credentials.py.dist` & `merchantapi-2.6.0/tests/credentials.py.dist`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/cssresource_delete_test.py` & `merchantapi-2.6.0/tests/cssresource_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/cssresource_insert_test.py` & `merchantapi-2.6.0/tests/cssresource_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/cssresource_update_test.py` & `merchantapi-2.6.0/tests/cssresource_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/cssresourcelist_load_query_test.py` & `merchantapi-2.6.0/tests/cssresourcelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customer_delete_test.py` & `merchantapi-2.6.0/tests/customer_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customer_insert_test.py` & `merchantapi-2.6.0/tests/customer_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customer_update_test.py` & `merchantapi-2.6.0/tests/customer_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddress_delete_test.py` & `merchantapi-2.6.0/tests/customeraddress_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddress_insert_test.py` & `merchantapi-2.6.0/tests/customeraddress_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddress_update_residential_test.py` & `merchantapi-2.6.0/tests/customeraddress_update_residential_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddress_update_test.py` & `merchantapi-2.6.0/tests/customeraddress_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddresslist_delete_test.py` & `merchantapi-2.6.0/tests/customeraddresslist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customeraddresslist_load_query_test.py` & `merchantapi-2.6.0/tests/customeraddresslist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customercredithistory_delete_test.py` & `merchantapi-2.6.0/tests/customercredithistory_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customercredithistory_insert_test.py` & `merchantapi-2.6.0/tests/customercredithistory_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customercredithistorylist_load_query_test.py` & `merchantapi-2.6.0/tests/customercredithistorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customerlist_load_query_test.py` & `merchantapi-2.6.0/tests/customerlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customerpaymentcard_register_test.py` & `merchantapi-2.6.0/tests/customerpaymentcard_register_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customerpaymentcardlist_load_query_test.py` & `merchantapi-2.6.0/tests/customerpaymentcardlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customerpricegrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/customerpricegrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/customersubscriptionlist_load_query_test.py` & `merchantapi-2.6.0/tests/customersubscriptionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/feeduri_insert_test.py` & `merchantapi-2.6.0/tests/feeduri_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/feeduri_update_test.py` & `merchantapi-2.6.0/tests/feeduri_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/feedurilist_delete_test.py` & `merchantapi-2.6.0/tests/feedurilist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/feedurilist_load_query_test.py` & `merchantapi-2.6.0/tests/feedurilist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/helper.py` & `merchantapi-2.6.0/tests/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -666,14 +666,31 @@
 	response = request.send()
 
 	validate_response_success(response, merchantapi.response.CouponCustomerListLoadQuery)
 
 	return response.get_coupon_customers()
 
 
+def get_coupon_business_accounts(code: str, title: str = None, assigned: bool = True, unassigned: bool = False):
+	request = merchantapi.request.CouponBusinessAccountListLoadQuery(init_client())
+	request.set_coupon_code(code)
+	request.set_assigned(assigned)
+	request.set_unassigned(unassigned)
+
+	if isinstance(title, str) and len(title):
+		request.get_filters() \
+			.equal('title', title)
+
+	response = request.send()
+
+	validate_response_success(response, merchantapi.response.CouponBusinessAccountListLoadQuery)
+
+	return response.get_coupon_business_accounts()
+
+
 def get_customer_addresses(login: str):
 	request = merchantapi.request.CustomerAddressListLoadQuery(init_client())
 	request.set_customer_login(login)
 
 	response = request.send()
 
 	validate_response_success(response, merchantapi.response.CustomerAddressListLoadQuery)
@@ -996,28 +1013,44 @@
 
 	assert list_result['success'] in (True, 1)
 	assert 'data'in list_result
 	assert 'data' in list_result['data']
 	return None if len(list_result['data']['data']) == 0 else list_result['data']['data'][0]
 
 
-def get_page(code: str):
+def get_page(code: str, branch: merchantapi.model.Branch = None):
 	request = merchantapi.request.PageListLoadQuery(init_client())
 
 	request.get_filters().equal('code', code)
 	request.set_on_demand_columns(request.get_available_on_demand_columns())
 	request.add_on_demand_column('CustomField_Values:*')
 
+	if branch != None:
+		request.set_branch_id(branch.get_id())
+
 	response = request.send()
 
 	validate_response_success(response, merchantapi.response.PageListLoadQuery)
 
 	return response.get_pages()[0] if len(response.get_pages()) else None
 
 
+def delete_page(code: str, branch: merchantapi.model.Branch = None):
+	request = merchantapi.request.PageDelete(init_client())
+
+	request.set_page_code(code)
+
+	if branch != None:
+		request.set_branch_id(branch.get_id())
+
+	response = request.send()
+
+	validate_response_success(response, merchantapi.response.PageDelete)
+
+
 def reset_branch_state():
 	bllqrequest = merchantapi.request.BranchListLoadQuery(init_client())
 	bllqresponse = bllqrequest.send()
 
 	if len(bllqresponse.get_branches()) == 1:
 		return
 
@@ -1095,7 +1128,69 @@
 	request.get_filters().equal('name', name)
 
 	response = request.send()
 
 	validate_response_success(response, merchantapi.response.CopyPageRulesListLoadQuery)
 
 	return response.get_copy_page_rules()[0] if len(response.get_copy_page_rules()) else None
+
+
+def assign_api_token_group(group: str):
+	token_response = send_admin_request( 'APITokenList_Load_Query', {
+		'Filter': [
+			{
+				'name':	'search',
+				'value':
+				[
+					{
+						'field':		'token',
+						'operator':		'EQ',
+						'value':		MerchantApiTestCredentials.MERCHANT_API_API_TOKEN
+					}
+				]
+			}
+		]
+	}, True)
+
+	token_result = token_response.json()
+
+	assert token_result['success'] in (True, 1)
+	assert token_result['data']['data'][0]['token'] == MerchantApiTestCredentials.MERCHANT_API_API_TOKEN
+
+	store_response = send_admin_request( 'StoreList_Load_Query', {
+		'Filter': [
+			{
+				'name':	'search',
+				'value':
+				[
+					{
+						'field':		'code',
+						'operator':		'EQ',
+						'value':		MerchantApiTestCredentials.MERCHANT_API_STORE_CODE
+					}
+				]
+			}
+		]
+	}, False)
+
+	store_result = store_response.json()
+	
+	assert store_result['success'] in (True, 1)
+	assert store_result['data']['data'][0]['id'] > 0
+
+	response = send_admin_request( 'APITokenGroup_Update_Assigned', {
+		'Group_Name':	group,
+        'Store_ID':		store_result['data']['data'][0]['id'],
+        'APIToken_ID':	token_result['data']['data'][0]['id'],
+        'Assigned':		True
+	}, True)
+
+
+def get_variant_pricing(product_id: int, variant_id: int):
+	response = send_admin_request( 'ProductVariantPricing_Load', {
+		'Product_ID': product_id,
+		'Variant_ID': variant_id
+	}, False)
+
+	result = response.json()
+
+	return result['data'] if 'data' in result else None
```

### Comparing `merchantapi-2.5.0/tests/imagetypelist_load_query_test.py` & `merchantapi-2.6.0/tests/imagetypelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/inventoryproductsettings_update_test.py` & `merchantapi-2.6.0/tests/inventoryproductsettings_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/javascriptresource_delete_test.py` & `merchantapi-2.6.0/tests/javascriptresource_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/javascriptresource_insert_test.py` & `merchantapi-2.6.0/tests/javascriptresource_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/javascriptresource_update_test.py` & `merchantapi-2.6.0/tests/javascriptresource_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/javascriptresourcelist_load_query_test.py` & `merchantapi-2.6.0/tests/javascriptresourcelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/listquery.py` & `merchantapi-2.6.0/tests/listquery.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/mivamerchantversion_test.py` & `merchantapi-2.6.0/tests/mivamerchantversion_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/module_test.py` & `merchantapi-2.6.0/tests/module_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/multicall.py` & `merchantapi-2.6.0/tests/multicall.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/note_delete_test.py` & `merchantapi-2.6.0/tests/note_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/note_insert_test.py` & `merchantapi-2.6.0/tests/note_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/note_update_test.py` & `merchantapi-2.6.0/tests/note_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/notelist_load_query_test.py` & `merchantapi-2.6.0/tests/notelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/option_delete_test.py` & `merchantapi-2.6.0/tests/option_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/option_insert_test.py` & `merchantapi-2.6.0/tests/option_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/option_load_code_test.py` & `merchantapi-2.6.0/tests/option_load_code_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/option_set_default_test.py` & `merchantapi-2.6.0/tests/option_set_default_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/option_update_test.py` & `merchantapi-2.6.0/tests/option_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/optionlist_load_attribute_test.py` & `merchantapi-2.6.0/tests/optionlist_load_attribute_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/order_create_fromorder_test.py` & `merchantapi-2.6.0/tests/order_create_fromorder_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/order_create_test.py` & `merchantapi-2.6.0/tests/order_create_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/order_delete_test.py` & `merchantapi-2.6.0/tests/order_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/order_update_customer_information_test.py` & `merchantapi-2.6.0/tests/order_update_customer_information_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordercoupon_update_assigned_test.py` & `merchantapi-2.6.0/tests/ordercoupon_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordercouponlist_load_query_test.py` & `merchantapi-2.6.0/tests/ordercouponlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordercustomfieldlist_load_test.py` & `merchantapi-2.6.0/tests/ordercustomfieldlist_load_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordercustomfields_update_test.py` & `merchantapi-2.6.0/tests/ordercustomfields_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitem_add_test.py` & `merchantapi-2.6.0/tests/orderitem_add_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitem_split_test.py` & `merchantapi-2.6.0/tests/orderitem_split_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitem_update_test.py` & `merchantapi-2.6.0/tests/orderitem_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_backorder_test.py` & `merchantapi-2.6.0/tests/orderitemlist_backorder_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_cancel_test.py` & `merchantapi-2.6.0/tests/orderitemlist_cancel_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_createreturn_test.py` & `merchantapi-2.6.0/tests/orderitemlist_createreturn_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_createshipment_test.py` & `merchantapi-2.6.0/tests/orderitemlist_createshipment_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_delete_test.py` & `merchantapi-2.6.0/tests/orderitemlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderitemlist_removefromshipment_test.py` & `merchantapi-2.6.0/tests/orderitemlist_removefromshipment_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderlist_archive_test.py` & `merchantapi-2.6.0/tests/orderlist_archive_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderlist_load_query_test.py` & `merchantapi-2.6.0/tests/orderlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderpricegroup_update_assigned_test.py` & `merchantapi-2.6.0/tests/orderpricegroup_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/orderpricegrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/orderpricegrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordershipmentlist_load_query_test.py` & `merchantapi-2.6.0/tests/ordershipmentlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/ordershipmentlist_update_test.py` & `merchantapi-2.6.0/tests/ordershipmentlist_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/page_copy_test.py` & `merchantapi-2.6.0/tests/page_copy_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/page_delete_test.py` & `merchantapi-2.6.0/tests/page_delete_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,21 +17,46 @@
 	"""
 	Tests the Page_Delete API Call
 	"""
 
 	helper.provision_store('Page_Delete.xml')
 
 	page_delete_test_deletion()
+	page_delete_test_branch_deletion()
 
 
 def page_delete_test_deletion():
 	request = merchantapi.request.PageDelete(helper.init_client())
 
 	request.set_page_code('PageDeleteTest_1')
 
 	response = request.send()
 
 	helper.validate_response_success(response, merchantapi.response.PageDelete)
 
 	check = helper.get_page('PageDeleteTest_1')
 
 	assert check is None
+
+
+def page_delete_test_branch_deletion():
+	helper.delete_branch('PageDeleteTest_1')
+
+	default_branch = helper.get_branch('Production')
+	assert default_branch != None
+
+	branch = helper.create_branch('PageDeleteTest_1', default_branch.get_color(), default_branch)
+
+	request = merchantapi.request.PageDelete(helper.init_client())
+
+	request.set_page_code('PageDeleteTest_2')
+	request.set_branch_id(branch.get_id())
+
+	response = request.send()
+
+	helper.validate_response_success(response, merchantapi.response.PageDelete)
+
+	checkDefault = helper.get_page('PageDeleteTest_2')
+	checkBranch = helper.get_page('PageDeleteTest_2', branch)
+
+	assert checkBranch is None
+	assert checkDefault is not None
```

### Comparing `merchantapi-2.5.0/tests/pagelist_load_query_test.py` & `merchantapi-2.6.0/tests/pagelist_load_query_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 	response = request.send()
 
 	helper.validate_response_success(response, merchantapi.response.PageListLoadQuery)
 
 	assert len(response.get_pages()) == 6
 
 	for i, page in enumerate(response.get_pages()):
+		assert page.get_version_id() > 0
 		assert page.get_code() == 'PLLQ_' + str(i+1)
 		assert page.get_name() == 'PLLQ_' + str(i+1) + ' Page'
 		assert page.get_title() == 'PLLQ_' + str(i+1) + ' Title'
 		assert page.get_code() == 'PLLQ_' + str(i+1)		
 		assert page.get_custom_field_values() is not None
 		assert page.get_custom_field_values().has_value('PLLQ_Test_checkbox', 'customfields') is True
 		assert page.get_custom_field_values().has_value('PLLQ_Test_imageupload', 'customfields') is True
```

### Comparing `merchantapi-2.5.0/tests/pageuri_insert_test.py` & `merchantapi-2.6.0/tests/pageuri_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pageuri_redirect_test.py` & `merchantapi-2.6.0/tests/pageuri_redirect_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pageuri_update_test.py` & `merchantapi-2.6.0/tests/pageuri_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pageurilist_delete_test.py` & `merchantapi-2.6.0/tests/pageurilist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pageurilist_load_query_test.py` & `merchantapi-2.6.0/tests/pageurilist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/paymentmethodlist_load_test.py` & `merchantapi-2.6.0/tests/paymentmethodlist_load_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroup_delete_test.py` & `merchantapi-2.6.0/tests/pricegroup_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroup_insert_test.py` & `merchantapi-2.6.0/tests/pricegroup_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroup_update_test.py` & `merchantapi-2.6.0/tests/pricegroup_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupbusinessaccount_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupbusinessaccount_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupbusinessaccountlist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupbusinessaccountlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupcategory_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupcategory_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupcategorylist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupcategorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupcustomer_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupcustomer_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupcustomerlist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupcustomerlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupexcludedcategory_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupexcludedcategory_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupexcludedcategorylist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupexcludedcategorylist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupexcludedproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupexcludedproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupexcludedproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupexcludedproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupqualifyingproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/pricegroupqualifyingproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/pricegroupqualifyingproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/pricegroupqualifyingproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/printqueuejob_delete_test.py` & `merchantapi-2.6.0/tests/printqueuejob_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/printqueuejob_insert_test.py` & `merchantapi-2.6.0/tests/printqueuejob_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/printqueuejob_status_test.py` & `merchantapi-2.6.0/tests/printqueuejob_status_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/printqueuejoblist_load_query_test.py` & `merchantapi-2.6.0/tests/printqueuejoblist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/printqueuelist_load_query_test.py` & `merchantapi-2.6.0/tests/printqueuelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/product_copy_test.py` & `merchantapi-2.6.0/tests/product_copy_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/product_delete_test.py` & `merchantapi-2.6.0/tests/product_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/product_insert_test.py` & `merchantapi-2.6.0/tests/product_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/product_update_test.py` & `merchantapi-2.6.0/tests/product_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productandsubscriptiontermlist_load_query_test.py` & `merchantapi-2.6.0/tests/productandsubscriptiontermlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productattributeandoptionlist_load_query_test.py` & `merchantapi-2.6.0/tests/productattributeandoptionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productimage_add_test.py` & `merchantapi-2.6.0/tests/productimage_add_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productimage_delete_test.py` & `merchantapi-2.6.0/tests/productimage_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productimage_update_type_test.py` & `merchantapi-2.6.0/tests/productimage_update_type_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productkit_generate_variants_test.py` & `merchantapi-2.6.0/tests/productkit_generate_variants_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productkit_update_parts_test.py` & `merchantapi-2.6.0/tests/productkit_update_parts_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productkit_variant_count_test.py` & `merchantapi-2.6.0/tests/productkit_variant_count_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productkitlist_load_query_test.py` & `merchantapi-2.6.0/tests/productkitlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productlist_adjust_inventory_test.py` & `merchantapi-2.6.0/tests/productlist_adjust_inventory_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productlist_load_query_test.py` & `merchantapi-2.6.0/tests/productlist_load_query_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 	helper.upload_image('graphics/ProductListLoadQuery7.jpg')
 	helper.provision_store('ProductList_Load_Query_v10.xml')
 
 	product_list_load_query_test_list_load()
 	product_list_load_query_test_list_load_with_custom_fields()
 	product_list_load_query_test_list_load_imagetypes()
 	product_list_load_query_test_list_load_subscription_fields()
+	product_list_load_query_test_list_load_page_fields()
 
 
 def product_list_load_query_test_list_load():
 	request = merchantapi.request.ProductListLoadQuery(helper.init_client())
 
 	request.set_filters(
 		request.filter_expression()
@@ -214,7 +215,24 @@
 	assert product.get_subscription_settings().get_next_delivery_date_minimum_required_orders() == 3
 
 	assert len(product.get_subscription_terms()) == 1
 
 	product.get_subscription_terms()[0].get_id() > 0
 	product.get_subscription_terms()[0].get_product_id() == product.get_id()
 
+
+def product_list_load_query_test_list_load_page_fields():
+	# See MMAPI-284
+
+	request = merchantapi.request.ProductListLoadQuery(helper.init_client())
+	request.get_filters().equal('code', 'ProductListLoadQueryPageTest')
+
+	response = request.send()
+
+	helper.validate_response_success(response, merchantapi.response.ProductListLoadQuery)
+
+	assert len(response.get_products()) == 1
+	
+	product = response.get_products()[0]
+
+	assert product.get_page_code() == 'ProductListLoadQueryPageTest'
+	assert product.get_page_id() > 0
```

### Comparing `merchantapi-2.5.0/tests/productsubscriptiontermlist_load_query_test.py` & `merchantapi-2.6.0/tests/productsubscriptiontermlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/producturi_insert_test.py` & `merchantapi-2.6.0/tests/producturi_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/producturi_redirect_test.py` & `merchantapi-2.6.0/tests/producturi_redirect_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/producturi_update_test.py` & `merchantapi-2.6.0/tests/producturi_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/producturilist_delete_test.py` & `merchantapi-2.6.0/tests/producturilist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/producturilist_load_query_test.py` & `merchantapi-2.6.0/tests/producturilist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariant_generate_delimiter_test.py` & `merchantapi-2.6.0/tests/productvariant_generate_delimiter_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariant_generate_test.py` & `merchantapi-2.6.0/tests/productvariant_generate_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariant_insert_test.py` & `merchantapi-2.6.0/tests/productvariant_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariant_update_test.py` & `merchantapi-2.6.0/tests/productvariant_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariantlist_delete_test.py` & `merchantapi-2.6.0/tests/productvariantlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariantlist_load_product_test.py` & `merchantapi-2.6.0/tests/productvariantlist_load_product_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/productvariantlist_load_query_test.py` & `merchantapi-2.6.0/tests/productvariantlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/relatedproduct_update_assigned_test.py` & `merchantapi-2.6.0/tests/relatedproduct_update_assigned_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/relatedproductlist_load_query_test.py` & `merchantapi-2.6.0/tests/relatedproductlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/request_builder_test.py` & `merchantapi-2.6.0/tests/request_builder_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/resourcegrouplist_load_query_test.py` & `merchantapi-2.6.0/tests/resourcegrouplist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/store_load_test.py` & `merchantapi-2.6.0/tests/store_load_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/storelist_load_query_test.py` & `merchantapi-2.6.0/tests/storelist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscription_insert_test.py` & `merchantapi-2.6.0/tests/subscription_insert_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscription_update_test.py` & `merchantapi-2.6.0/tests/subscription_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscriptionandorderitem_add_test.py` & `merchantapi-2.6.0/tests/subscriptionandorderitem_add_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscriptionandorderitem_update_test.py` & `merchantapi-2.6.0/tests/subscriptionandorderitem_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscriptionlist_delete_test.py` & `merchantapi-2.6.0/tests/subscriptionlist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscriptionlist_load_query_test.py` & `merchantapi-2.6.0/tests/subscriptionlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/subscriptionshippingmethodlist_load_query_test.py` & `merchantapi-2.6.0/tests/subscriptionshippingmethodlist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/uri_delete_test.py` & `merchantapi-2.6.0/tests/uri_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/uri_insert_test.py` & `merchantapi-2.6.0/tests/uri_insert_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,8 +113,8 @@
 
 	assert isinstance(response.get_uri(), merchantapi.model.Uri)
 	assert response.get_uri().get_uri() == test_uri
 
 	check = helper.get_uri(test_uri)
 
 	assert check is not None
-	assert check.get_page_id() > 0
+	assert check.get_page_code() == 'UriInsertTest_2'
```

### Comparing `merchantapi-2.5.0/tests/uri_update_test.py` & `merchantapi-2.6.0/tests/uri_update_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/urilist_delete_test.py` & `merchantapi-2.6.0/tests/urilist_delete_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/urilist_load_query_test.py` & `merchantapi-2.6.0/tests/urilist_load_query_test.py`

 * *Files identical despite different names*

### Comparing `merchantapi-2.5.0/tests/version_settings_test.py` & `merchantapi-2.6.0/tests/version_settings_test.py`

 * *Files identical despite different names*

