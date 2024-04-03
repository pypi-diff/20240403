# Comparing `tmp/oney-payment-1.0.2.tar.gz` & `tmp/oney-payment-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oney-payment-1.0.2.tar", last modified: Thu Mar 28 13:04:08 2024, max compression
+gzip compressed data, was "oney-payment-1.0.3.tar", last modified: Wed Apr  3 12:27:12 2024, max compression
```

## Comparing `oney-payment-1.0.2.tar` & `oney-payment-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.079630 oney-payment-1.0.2/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1335 2024-03-28 13:04:08.078933 oney-payment-1.0.2/PKG-INFO
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.055539 oney-payment-1.0.2/oney_payment/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/__init__.py
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.068203 oney-payment-1.0.2/oney_payment/commerce/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/commerce/__init__.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1311 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/commerce/checkout.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1389 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/commerce/dummy.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      822 2024-03-28 12:46:12.000000 oney-payment-1.0.2/oney_payment/forms.py
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.070399 oney-payment-1.0.2/oney_payment/templates/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      648 2024-03-28 12:46:12.000000 oney-payment-1.0.2/oney_payment/templates/oney-extension-redirect-form.html
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.076956 oney-payment-1.0.2/oney_payment/tests/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/tests/__init__.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      716 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/tests/mixins.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     2857 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/tests/test_service.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1723 2024-03-28 12:46:12.000000 oney-payment-1.0.2/oney_payment/tests/test_views.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      190 2024-03-25 14:34:53.000000 oney-payment-1.0.2/oney_payment/urls.py
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1405 2024-03-28 12:46:12.000000 oney-payment-1.0.2/oney_payment/views.py
-drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-03-28 13:04:08.078243 oney-payment-1.0.2/oney_payment.egg-info/
--rw-r--r--   0 israfilbulbul   (501) staff       (20)     1335 2024-03-28 13:04:08.000000 oney-payment-1.0.2/oney_payment.egg-info/PKG-INFO
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      596 2024-03-28 13:04:08.000000 oney-payment-1.0.2/oney_payment.egg-info/SOURCES.txt
--rw-r--r--   0 israfilbulbul   (501) staff       (20)        1 2024-03-28 13:04:08.000000 oney-payment-1.0.2/oney_payment.egg-info/dependency_links.txt
--rw-r--r--   0 israfilbulbul   (501) staff       (20)        1 2024-03-27 13:29:16.000000 oney-payment-1.0.2/oney_payment.egg-info/not-zip-safe
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      109 2024-03-28 13:04:08.000000 oney-payment-1.0.2/oney_payment.egg-info/requires.txt
--rw-r--r--   0 israfilbulbul   (501) staff       (20)       13 2024-03-28 13:04:08.000000 oney-payment-1.0.2/oney_payment.egg-info/top_level.txt
--rw-r--r--   0 israfilbulbul   (501) staff       (20)       38 2024-03-28 13:04:08.079780 oney-payment-1.0.2/setup.cfg
--rw-r--r--   0 israfilbulbul   (501) staff       (20)      835 2024-03-28 13:03:26.000000 oney-payment-1.0.2/setup.py
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.821837 oney-payment-1.0.3/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1335 2024-04-03 12:27:12.819746 oney-payment-1.0.3/PKG-INFO
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.767755 oney-payment-1.0.3/oney_payment/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/__init__.py
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.791365 oney-payment-1.0.3/oney_payment/commerce/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/commerce/__init__.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1342 2024-04-03 12:25:18.000000 oney-payment-1.0.3/oney_payment/commerce/checkout.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1389 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/commerce/dummy.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      822 2024-03-28 12:46:12.000000 oney-payment-1.0.3/oney_payment/forms.py
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.796368 oney-payment-1.0.3/oney_payment/templates/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      648 2024-03-28 12:46:12.000000 oney-payment-1.0.3/oney_payment/templates/oney-extension-redirect-form.html
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.809321 oney-payment-1.0.3/oney_payment/tests/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)        0 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/tests/__init__.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      716 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/tests/mixins.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     2884 2024-04-03 12:25:18.000000 oney-payment-1.0.3/oney_payment/tests/test_service.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1723 2024-03-28 12:46:12.000000 oney-payment-1.0.3/oney_payment/tests/test_views.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      190 2024-03-25 14:34:53.000000 oney-payment-1.0.3/oney_payment/urls.py
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1405 2024-03-28 12:46:12.000000 oney-payment-1.0.3/oney_payment/views.py
+drwxr-xr-x   0 israfilbulbul   (501) staff       (20)        0 2024-04-03 12:27:12.817242 oney-payment-1.0.3/oney_payment.egg-info/
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)     1335 2024-04-03 12:27:12.000000 oney-payment-1.0.3/oney_payment.egg-info/PKG-INFO
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      596 2024-04-03 12:27:12.000000 oney-payment-1.0.3/oney_payment.egg-info/SOURCES.txt
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)        1 2024-04-03 12:27:12.000000 oney-payment-1.0.3/oney_payment.egg-info/dependency_links.txt
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)        1 2024-03-27 13:29:16.000000 oney-payment-1.0.3/oney_payment.egg-info/not-zip-safe
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      109 2024-04-03 12:27:12.000000 oney-payment-1.0.3/oney_payment.egg-info/requires.txt
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)       13 2024-04-03 12:27:12.000000 oney-payment-1.0.3/oney_payment.egg-info/top_level.txt
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)       38 2024-04-03 12:27:12.822294 oney-payment-1.0.3/setup.cfg
+-rw-r--r--   0 israfilbulbul   (501) staff       (20)      835 2024-04-03 12:25:18.000000 oney-payment-1.0.3/setup.py
```

### Comparing `oney-payment-1.0.2/PKG-INFO` & `oney-payment-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oney-payment
-Version: 1.0.2
+Version: 1.0.3
 Summary: A common library for providing order details to Oney Payment Gateway.
 Home-page: https://bitbucket.org/akinonteam/oney-payment
 Author: Akinon
 Author-email: dev@akinon.com
 Description-Content-Type: text/markdown
 Requires-Dist: Django<4.0,>=2.2.9
 Requires-Dist: requests
```

### Comparing `oney-payment-1.0.2/oney_payment/commerce/checkout.py` & `oney-payment-1.0.3/oney_payment/commerce/checkout.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                 "country_code": pre_order["shipping_address"]["country"]["code"],
                 "address_line": pre_order["shipping_address"]["line"],
                 "municipality": pre_order["shipping_address"]["city"]["name"],
             },
             "orders": [
                 {
                     "label": item["product"]["name"],
-                    "type": item["product"]["product_type"],
+                    "type": item["product"]["attributes"].get("integration_product_state"),
                     "item_external_code": item["product"]["sku"],
                     "quantity": item["quantity"],
                     "price": item["total_amount"],
                 }
                 for item in pre_order["basket"]["basketitem_set"]
             ],
         }
```

### Comparing `oney-payment-1.0.2/oney_payment/commerce/dummy.py` & `oney-payment-1.0.3/oney_payment/commerce/dummy.py`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment/forms.py` & `oney-payment-1.0.3/oney_payment/forms.py`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment/templates/oney-extension-redirect-form.html` & `oney-payment-1.0.3/oney_payment/templates/oney-extension-redirect-form.html`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment/tests/mixins.py` & `oney-payment-1.0.3/oney_payment/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment/tests/test_service.py` & `oney-payment-1.0.3/oney_payment/tests/test_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,11 +60,11 @@
 
         orders = oney_context["orders"]
         basket_items = pre_order["basket"]["basketitem_set"]
         self.assertEqual(len(orders), len(basket_items))
 
         for order, basket_item in zip(orders, basket_items):
             self.assertEqual(order["label"], basket_item["product"]["name"])
-            self.assertEqual(order["type"], basket_item["product"]["product_type"])
+            self.assertEqual(order["type"], basket_item["product"]["attributes"]["integration_product_state"])
             self.assertEqual(order["item_external_code"], basket_item["product"]["sku"])
             self.assertEqual(order["quantity"], basket_item["quantity"])
             self.assertEqual(order["price"], basket_item["total_amount"])
```

### Comparing `oney-payment-1.0.2/oney_payment/tests/test_views.py` & `oney-payment-1.0.3/oney_payment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment/views.py` & `oney-payment-1.0.3/oney_payment/views.py`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/oney_payment.egg-info/PKG-INFO` & `oney-payment-1.0.3/oney_payment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oney-payment
-Version: 1.0.2
+Version: 1.0.3
 Summary: A common library for providing order details to Oney Payment Gateway.
 Home-page: https://bitbucket.org/akinonteam/oney-payment
 Author: Akinon
 Author-email: dev@akinon.com
 Description-Content-Type: text/markdown
 Requires-Dist: Django<4.0,>=2.2.9
 Requires-Dist: requests
```

### Comparing `oney-payment-1.0.2/oney_payment.egg-info/SOURCES.txt` & `oney-payment-1.0.3/oney_payment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oney-payment-1.0.2/setup.py` & `oney-payment-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("readme.md", "r") as f:
         return f.read()
 
 
 setuptools.setup(
     name="oney-payment",
-    version="1.0.2",
+    version="1.0.3",
     author="Akinon",
     author_email="dev@akinon.com",
     description="A common library for providing order details to Oney Payment Gateway.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/akinonteam/oney-payment",
     packages=setuptools.find_packages(exclude=["tests", "tests.*", "dummy.*"]),
```

