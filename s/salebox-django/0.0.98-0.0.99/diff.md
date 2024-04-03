# Comparing `tmp/salebox-django-0.0.98.tar.gz` & `tmp/salebox-django-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salebox-django-0.0.98.tar", last modified: Mon Apr 22 09:30:12 2019, max compression
+gzip compressed data, was "dist/salebox-django-0.0.99.tar", last modified: Mon Apr 22 11:25:31 2019, max compression
```

## Comparing `salebox-django-0.0.98.tar` & `salebox-django-0.0.99.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       38 2019-04-22 09:30:12.000000 salebox-django-0.0.98/setup.cfg
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1031 2019-04-22 09:30:04.000000 salebox-django-0.0.98/setup.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/providers/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/providers/twoctwop/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1379 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/providers/twoctwop/callback.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/providers/twoctwop/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2080 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/providers/twoctwop/gateway.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/providers/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)    30048 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/models.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2006 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/forms.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/static/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     7656 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/static/salebox.js
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/management/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/management/commands/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/management/commands/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)    39472 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/management/commands/saleboxsync.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1039 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/management/commands/saleboxcleanbasket.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/management/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      122 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/context_processor.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1283 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/urls.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3662 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/admin.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/migrations/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      813 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/0004_transactionevent.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      572 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/0002_auto_20190411_1613.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/__init__.py
--rw-rw-r--   0 joncombe  (1000) joncombe  (1000)     1181 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/0003_auto_20190418_2014.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      363 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/0005_auto_20190419_1056.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)    32139 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/migrations/0001_initial.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3130 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/middleware.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/locale/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/locale/th/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/locale/th/LC_MESSAGES/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4628 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2206 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/locale/th/LC_MESSAGES/django.mo
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/account/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1541 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/account/address.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      681 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/account/home.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      810 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/account/basket.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/account/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      464 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/account/wishlist.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2300 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/base.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/basket/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/basket/migrate.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      264 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/basket/base.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      771 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/basket/basket.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/basket/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      725 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/basket/wishlist.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/rating/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      554 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/rating/add.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      537 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/rating/remove.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      229 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/rating/base.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/rating/__init__.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/image/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      528 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/image/image.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/image/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/__init__.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/callback/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1416 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/callback/callback.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/callback/__init__.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2921 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/base.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     5230 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_invoice_address.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      335 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/confirmation.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      655 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/payment_method.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3329 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_address.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2334 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_method.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1112 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/gateway.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      311 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/checkout/receipt.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/views/address/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1757 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/add.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      430 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/remove.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        7 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/edit.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      233 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/base.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      438 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/set_default.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/views/address/__init__.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/account/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      411 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/account/home.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      102 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/account/wishlist.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       99 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/account/basket.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      517 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/account/address.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3095 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/basket_full.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1789 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/wishlist_full.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      814 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/button_basket.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/wishlist_summary.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      646 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/button_wishlist.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/basket_summary.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/utils/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      961 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/utils/pagination.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      201 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/utils/rating.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      284 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/_basket.txt
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/transaction_created/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/transaction_created/body.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      207 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/transaction_created/body.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       27 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/transaction_created/subject.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/_base.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/shipping_shipped/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/shipping_shipped/body.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      288 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/shipping_shipped/body.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       28 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/shipping_shipped/subject.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/_base.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/email/_basket.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      369 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/confirmation.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1349 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/shipping_address.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      438 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/shipping_method.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      350 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/_ideolocator.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      387 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/receipt.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      131 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/_base.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      483 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/gateway.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      451 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/payment_method.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2932 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/shipping_invoice_address.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1437 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_static_single.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      113 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_static.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1073 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_radio_single.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4163 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/add_form.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      112 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_radio.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/product/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1095 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/product/product_list.html
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1018 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templates/salebox/product/product_list_single.html
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/templatetags/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      565 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templatetags/salebox_utils.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templatetags/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1438 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/templatetags/salebox_address.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/saleboxdjango/lib/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1525 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/common.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     7335 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/address.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2896 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/rating.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)    17239 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/basket.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/__init__.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4136 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/event_handler.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      723 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/variant.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)    15973 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/product.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4786 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/binpack.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     6229 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/category.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4920 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/shipping_options.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     9195 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/lib/checkout.py
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      130 2019-04-22 09:28:51.000000 salebox-django-0.0.98/saleboxdjango/apps.py
-drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       14 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/top_level.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)       64 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/requires.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/PKG-INFO
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        1 2019-03-05 02:47:55.000000 salebox-django-0.0.98/salebox_django.egg-info/not-zip-safe
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)     5322 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/SOURCES.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)        1 2019-04-22 09:30:12.000000 salebox-django-0.0.98/salebox_django.egg-info/dependency_links.txt
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 09:30:12.000000 salebox-django-0.0.98/PKG-INFO
--rw-rw-r--   0 joncombe  (1000) joncombe  (1000)     1487 2019-02-26 03:19:12.000000 salebox-django-0.0.98/LICENCE
--rw-rw-r--   0 joncombe  (1000) joncombe  (1000)       31 2018-12-11 02:55:58.000000 salebox-django-0.0.98/AUTHORS
--rw-r--r--   0 joncombe  (1000) joncombe  (1000)      202 2019-04-18 07:24:43.000000 salebox-django-0.0.98/MANIFEST.in
--rw-rw-r--   0 joncombe  (1000) joncombe  (1000)      119 2018-12-11 02:55:58.000000 salebox-django-0.0.98/README.md
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       38 2019-04-22 11:25:31.000000 salebox-django-0.0.99/setup.cfg
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1031 2019-04-22 11:25:27.000000 salebox-django-0.0.99/setup.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/providers/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/providers/twoctwop/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1379 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/providers/twoctwop/callback.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/providers/twoctwop/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2080 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/providers/twoctwop/gateway.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/providers/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)    30048 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/models.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2006 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/forms.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/static/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     7656 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/static/salebox.js
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/management/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/management/commands/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/management/commands/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)    39614 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/management/commands/saleboxsync.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1039 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/management/commands/saleboxcleanbasket.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/management/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      122 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/context_processor.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1283 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/urls.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3662 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/admin.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/migrations/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      813 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/0004_transactionevent.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      572 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/0002_auto_20190411_1613.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/__init__.py
+-rw-rw-r--   0 joncombe  (1000) joncombe  (1000)     1181 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/0003_auto_20190418_2014.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      363 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/0005_auto_20190419_1056.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)    32139 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/migrations/0001_initial.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3130 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/middleware.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/locale/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/locale/th/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/locale/th/LC_MESSAGES/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4628 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2206 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/locale/th/LC_MESSAGES/django.mo
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/account/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1541 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/account/address.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      681 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/account/home.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      810 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/account/basket.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/account/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      464 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/account/wishlist.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2300 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/base.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/basket/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/basket/migrate.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      264 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/basket/base.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      771 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/basket/basket.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/basket/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      725 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/basket/wishlist.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/rating/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      554 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/rating/add.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      537 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/rating/remove.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      229 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/rating/base.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/rating/__init__.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/image/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      528 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/image/image.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/image/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/__init__.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/callback/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1416 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/callback/callback.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/callback/__init__.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2921 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/base.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     5230 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_invoice_address.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      335 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/confirmation.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      655 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/payment_method.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3329 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_address.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2334 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_method.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1112 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/gateway.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      311 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/checkout/receipt.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/views/address/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1757 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/add.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      430 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/remove.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        7 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/edit.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      233 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/base.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      438 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/set_default.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/views/address/__init__.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/account/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      411 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/account/home.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      102 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/account/wishlist.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       99 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/account/basket.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      517 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/account/address.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     3095 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/basket_full.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1789 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/wishlist_full.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      814 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/button_basket.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/wishlist_summary.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      646 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/button_wishlist.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/basket_summary.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/utils/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      961 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/utils/pagination.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      201 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/utils/rating.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      284 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/_basket.txt
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/transaction_created/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/transaction_created/body.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      207 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/transaction_created/body.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       27 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/transaction_created/subject.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/_base.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/shipping_shipped/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       10 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/shipping_shipped/body.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      288 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/shipping_shipped/body.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       28 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/shipping_shipped/subject.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/_base.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       11 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/email/_basket.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      369 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/confirmation.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1349 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/shipping_address.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      438 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/shipping_method.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      350 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/_ideolocator.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      387 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/receipt.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      131 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/_base.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      483 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/gateway.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      451 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/payment_method.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2932 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/shipping_invoice_address.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1437 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_static_single.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      113 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_static.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1073 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_radio_single.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4163 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/add_form.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      112 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_radio.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/product/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1095 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/product/product_list.html
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1018 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templates/salebox/product/product_list_single.html
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/templatetags/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      565 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templatetags/salebox_utils.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templatetags/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1438 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/templatetags/salebox_address.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/saleboxdjango/lib/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     1525 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/common.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     7335 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/address.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     2896 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/rating.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)    17239 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/basket.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/__init__.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4136 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/event_handler.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      723 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/variant.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)    15973 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/product.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4786 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/binpack.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     6229 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/category.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     4920 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/shipping_options.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     9195 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/lib/checkout.py
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      130 2019-04-22 11:23:19.000000 salebox-django-0.0.99/saleboxdjango/apps.py
+drwxr-xr-x   0 joncombe  (1000) joncombe  (1000)        0 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       14 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/top_level.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)       64 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/requires.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/PKG-INFO
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        1 2019-03-05 02:47:55.000000 salebox-django-0.0.99/salebox_django.egg-info/not-zip-safe
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)     5322 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/SOURCES.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)        1 2019-04-22 11:25:31.000000 salebox-django-0.0.99/salebox_django.egg-info/dependency_links.txt
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      680 2019-04-22 11:25:31.000000 salebox-django-0.0.99/PKG-INFO
+-rw-rw-r--   0 joncombe  (1000) joncombe  (1000)     1487 2019-02-26 03:19:12.000000 salebox-django-0.0.99/LICENCE
+-rw-rw-r--   0 joncombe  (1000) joncombe  (1000)       31 2018-12-11 02:55:58.000000 salebox-django-0.0.99/AUTHORS
+-rw-r--r--   0 joncombe  (1000) joncombe  (1000)      202 2019-04-18 07:24:43.000000 salebox-django-0.0.99/MANIFEST.in
+-rw-rw-r--   0 joncombe  (1000) joncombe  (1000)      119 2018-12-11 02:55:58.000000 salebox-django-0.0.99/README.md
```

### Comparing `salebox-django-0.0.98/setup.py` & `salebox-django-0.0.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='salebox-django',
-    version='0.0.98',
+    version='0.0.99',
     author=u'Jon Combe',
     author_email='jon@getsalebox.com',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'django-mptt',
         'django-opposable-thumbs',
```

### Comparing `salebox-django-0.0.98/saleboxdjango/providers/twoctwop/callback.py` & `salebox-django-0.0.99/saleboxdjango/providers/twoctwop/callback.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/providers/twoctwop/gateway.py` & `salebox-django-0.0.99/saleboxdjango/providers/twoctwop/gateway.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/models.py` & `salebox-django-0.0.99/saleboxdjango/models.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/forms.py` & `salebox-django-0.0.99/saleboxdjango/forms.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/static/salebox.js` & `salebox-django-0.0.99/saleboxdjango/static/salebox.js`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/management/commands/saleboxsync.py` & `salebox-django-0.0.99/saleboxdjango/management/commands/saleboxsync.py`

 * *Files 0% similar despite different names*

```diff
@@ -980,14 +980,15 @@
             self.push_member(user)
 
     def push_transaction(self, store):
         # build POST
         data = self.init_post()
         data['transaction'] = json.dumps({
             'basket': self.transaction_basket(store),
+            'extras': self.transaction_extras(store),
             'invoice': self.transaction_invoice(store),
             'manual_discount': None,
             'member': self.transaction_member(store),
             'meta': self.transaction_meta(store),
             'payment': self.transaction_payment(store),
             'shipping': self.transaction_shipping(store),
             'stored_value_load': None,
@@ -1061,14 +1062,17 @@
                 'shipping_weight': v['shipping_weight'],
                 'unit_price': v['price'],
                 'variant_id': v['id'],
             })
 
         return basket
 
+    def transaction_extras(self, store):
+        return store.data.get('extras', None)
+
     def transaction_invoice(self, store):
         data = store.data['invoice_address']
 
         # invoice not requested
         if not data['required']:
             return None
```

### Comparing `salebox-django-0.0.98/saleboxdjango/management/commands/saleboxcleanbasket.py` & `salebox-django-0.0.99/saleboxdjango/management/commands/saleboxcleanbasket.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/urls.py` & `salebox-django-0.0.99/saleboxdjango/urls.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/admin.py` & `salebox-django-0.0.99/saleboxdjango/admin.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/migrations/0004_transactionevent.py` & `salebox-django-0.0.99/saleboxdjango/migrations/0004_transactionevent.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/migrations/0002_auto_20190411_1613.py` & `salebox-django-0.0.99/saleboxdjango/migrations/0002_auto_20190411_1613.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/migrations/0003_auto_20190418_2014.py` & `salebox-django-0.0.99/saleboxdjango/migrations/0003_auto_20190418_2014.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/migrations/0001_initial.py` & `salebox-django-0.0.99/saleboxdjango/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/middleware.py` & `salebox-django-0.0.99/saleboxdjango/middleware.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/locale/th/LC_MESSAGES/django.po` & `salebox-django-0.0.99/saleboxdjango/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/locale/th/LC_MESSAGES/django.mo` & `salebox-django-0.0.99/saleboxdjango/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/account/address.py` & `salebox-django-0.0.99/saleboxdjango/views/account/address.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/account/home.py` & `salebox-django-0.0.99/saleboxdjango/views/account/home.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/account/basket.py` & `salebox-django-0.0.99/saleboxdjango/views/account/basket.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/base.py` & `salebox-django-0.0.99/saleboxdjango/views/base.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/basket/migrate.py` & `salebox-django-0.0.99/saleboxdjango/views/basket/migrate.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/basket/basket.py` & `salebox-django-0.0.99/saleboxdjango/views/basket/basket.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/basket/wishlist.py` & `salebox-django-0.0.99/saleboxdjango/views/basket/wishlist.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/rating/add.py` & `salebox-django-0.0.99/saleboxdjango/views/rating/add.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/rating/remove.py` & `salebox-django-0.0.99/saleboxdjango/views/rating/remove.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/image/image.py` & `salebox-django-0.0.99/saleboxdjango/views/image/image.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/callback/callback.py` & `salebox-django-0.0.99/saleboxdjango/views/callback/callback.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/base.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/base.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_invoice_address.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_invoice_address.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/payment_method.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/payment_method.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_address.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_address.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/shipping_method.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/shipping_method.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/checkout/gateway.py` & `salebox-django-0.0.99/saleboxdjango/views/checkout/gateway.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/views/address/add.py` & `salebox-django-0.0.99/saleboxdjango/views/address/add.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/account/address.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/account/address.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/basket_full.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/basket_full.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/wishlist_full.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/wishlist_full.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/button_basket.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/button_basket.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/basket/button_wishlist.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/basket/button_wishlist.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/utils/pagination.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/utils/pagination.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/shipping_address.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/shipping_address.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/checkout/shipping_invoice_address.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/checkout/shipping_invoice_address.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_static_single.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_static_single.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/address/list_radio_single.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/address/list_radio_single.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/address/add_form.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/address/add_form.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/product/product_list.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/product/product_list.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templates/salebox/product/product_list_single.html` & `salebox-django-0.0.99/saleboxdjango/templates/salebox/product/product_list_single.html`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templatetags/salebox_utils.py` & `salebox-django-0.0.99/saleboxdjango/templatetags/salebox_utils.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/templatetags/salebox_address.py` & `salebox-django-0.0.99/saleboxdjango/templatetags/salebox_address.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/common.py` & `salebox-django-0.0.99/saleboxdjango/lib/common.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/address.py` & `salebox-django-0.0.99/saleboxdjango/lib/address.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/rating.py` & `salebox-django-0.0.99/saleboxdjango/lib/rating.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/basket.py` & `salebox-django-0.0.99/saleboxdjango/lib/basket.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/event_handler.py` & `salebox-django-0.0.99/saleboxdjango/lib/event_handler.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/variant.py` & `salebox-django-0.0.99/saleboxdjango/lib/variant.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/product.py` & `salebox-django-0.0.99/saleboxdjango/lib/product.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/binpack.py` & `salebox-django-0.0.99/saleboxdjango/lib/binpack.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/category.py` & `salebox-django-0.0.99/saleboxdjango/lib/category.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/shipping_options.py` & `salebox-django-0.0.99/saleboxdjango/lib/shipping_options.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/saleboxdjango/lib/checkout.py` & `salebox-django-0.0.99/saleboxdjango/lib/checkout.py`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/salebox_django.egg-info/PKG-INFO` & `salebox-django-0.0.99/salebox_django.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: salebox-django
-Version: 0.0.98
+Version: 0.0.99
 Summary: Django ecommerce powered by Salebox
 Home-page: https://getsalebox.com
 Author: Jon Combe
 Author-email: jon@getsalebox.com
 License: BSD licence, see LICENCE file
 Description: Connect a standalone Django ecommerce website to a GetSalebox.com backoffice
 Platform: UNKNOWN
```

### Comparing `salebox-django-0.0.98/salebox_django.egg-info/SOURCES.txt` & `salebox-django-0.0.99/salebox_django.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `salebox-django-0.0.98/PKG-INFO` & `salebox-django-0.0.99/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: salebox-django
-Version: 0.0.98
+Version: 0.0.99
 Summary: Django ecommerce powered by Salebox
 Home-page: https://getsalebox.com
 Author: Jon Combe
 Author-email: jon@getsalebox.com
 License: BSD licence, see LICENCE file
 Description: Connect a standalone Django ecommerce website to a GetSalebox.com backoffice
 Platform: UNKNOWN
```

### Comparing `salebox-django-0.0.98/LICENCE` & `salebox-django-0.0.99/LICENCE`

 * *Files identical despite different names*

