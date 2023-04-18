# Comparing `tmp/klarna-orders-1.0.1.tar.gz` & `tmp/klarna-orders-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarna-orders-1.0.1.tar", last modified: Thu Apr  6 10:28:10 2023, max compression
+gzip compressed data, was "klarna-orders-1.1.0.tar", last modified: Tue Apr 18 00:08:27 2023, max compression
```

## Comparing `klarna-orders-1.0.1.tar` & `klarna-orders-1.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.140529 klarna-orders-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-06 10:28:10.140529 klarna-orders-1.0.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7461 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 10:28:10.140529 klarna-orders-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.120528 klarna-orders-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.124528 klarna-orders-1.0.1/src/klarna/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1864 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/authorizations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.124528 klarna-orders-1.0.1/src/klarna/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.128528 klarna-orders-1.0.1/src/klarna/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/cancelauthorization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/createcreditsession.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/createorder.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/purchasetoken.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/readcreditsession.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/operations/updatecreditsession.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.136528 klarna-orders-1.0.1/src/klarna/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4549 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/address.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/asset_urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/authorized_payment_method.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/create_order_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/customer_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/customer_read_create_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/customer_token_creation_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/customer_token_creation_response.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/errorv2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/merchant_session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/merchant_urls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/order.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/order_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/payment_method_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/product_identifiers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/session.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7433 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/session_create.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9509 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/session_read.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/models/shared/subscription.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3581 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/sessions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.136528 klarna-orders-1.0.1/src/klarna/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-06 10:27:52.000000 klarna-orders-1.0.1/src/klarna/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:28:10.140529 klarna-orders-1.0.1/src/klarna_orders.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-06 10:28:09.000000 klarna-orders-1.0.1/src/klarna_orders.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-06 10:28:10.000000 klarna-orders-1.0.1/src/klarna_orders.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:28:09.000000 klarna-orders-1.0.1/src/klarna_orders.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-06 10:28:09.000000 klarna-orders-1.0.1/src/klarna_orders.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 10:28:09.000000 klarna-orders-1.0.1/src/klarna_orders.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7475 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1864 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/authorizations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.612398 klarna-orders-1.1.0/src/klarna/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      659 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/cancelauthorization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/createcreditsession.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1068 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/createorder.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/purchasetoken.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/readcreditsession.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      867 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/operations/updatecreditsession.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4549 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      989 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/asset_urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      995 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1413 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/authorized_payment_method.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5395 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/create_order_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3823 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3167 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      844 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_read_create_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1940 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_response.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1733 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/errorv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1282 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/merchant_session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1897 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/merchant_urls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1830 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2075 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4993 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/order_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/payment_method_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/product_identifiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      336 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7597 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7433 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session_create.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9509 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/session_read.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/models/shared/subscription.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2840 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3581 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5485 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/sessions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2864 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-18 00:08:17.000000 klarna-orders-1.1.0/src/klarna/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:27.616397 klarna-orders-1.1.0/src/klarna_orders.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 00:08:27.000000 klarna-orders-1.1.0/src/klarna_orders.egg-info/top_level.txt
```

### Comparing `klarna-orders-1.0.1/LICENSE.md` & `klarna-orders-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/PKG-INFO` & `klarna-orders-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarna-orders
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy-Klarna
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -104,15 +104,15 @@
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
                     interval="WEEK",
                     interval_count=297534,
-                    name="debitis",
+                    name="Larry Windler",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -130,17 +130,17 @@
                     size="small",
                 ),
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
-                    interval="DAY",
-                    interval_count=963663,
-                    name="tempora",
+                    interval="WEEK",
+                    interval_count=791725,
+                    name="Ken Kshlerin",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -152,15 +152,15 @@
         shipping_address=shared.Address(
             attention="Attn",
             city="London",
             country="GB",
             email="test.sam@test.com",
             family_name="Andersson",
             given_name="Adam",
-            organization_name="suscipit",
+            organization_name="recusandae",
             phone="+44795465131",
             postal_code="W1G 0PW",
             region="OH",
             street_address="33 Cavendish Square",
             street_address2="Floor 22 / Flat 2",
             title="Mr.",
         ),
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: klarna-orders Version: 1.0.1 Summary: Python Client
+Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Speakeasy-Klarna License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
   [https://user-images.githubusercontent.com/6267663/230347878-f2873a58-f578-
                           4e95-86e0-7bebfd78f4f1.svg]
                            ****** Python SDK ******
                 An effortless integration. Designed for growth.
@@ -40,41 +40,42 @@
 "test@gmail.com","account_registration_date":"2017-02-13T10:49:
 20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
 product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
 category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="WEEK", interval_count=297534, name="debitis", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), shared.OrderLine( image_url="https://
-www.exampleobjects.com/logo.png", merchant_data="{"customer_account_info":[
-{"unique_account_identifier":"test@gmail.com","account_registration_date":
-"2017-02-13T10:49:20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}",
-name="Running shoe", product_identifiers=shared.ProductIdentifiers
-( brand="shoe-brand", category_path="Shoes > Running", color="white",
+( interval="WEEK", interval_count=297534, name="Larry Windler", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), shared.OrderLine
+( image_url="https://www.exampleobjects.com/logo.png", merchant_data="
+{"customer_account_info":[{"unique_account_identifier":
+"test@gmail.com","account_registration_date":"2017-02-13T10:49:
+20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
+product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
+category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="DAY", interval_count=963663, name="tempora", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), ], order_tax_amount=475,
-purchase_country="GB", purchase_currency="GBP", shipping_address=shared.Address
-( attention="Attn", city="London", country="GB", email="test.sam@test.com",
-family_name="Andersson", given_name="Adam", organization_name="suscipit",
-phone="+44795465131", postal_code="W1G 0PW", region="OH", street_address="33
-Cavendish Square", street_address2="Floor 22 / Flat 2", title="Mr.", ), ), )
-res = s.orders.create(req) if res.order is not None: # handle response ```   ##
-Available Resources and Operations ### authorizations * `cancel` - Cancel an
-existing authorization ### orders * `create` - Create a new order ### sessions
-* `create` - Create a new payment session * `read` - Read an existing payment
-session * `update` - Update an existing payment session ### tokens * `purchase`
-- Generate a consumer token  ### Maturity This SDK is in beta, and there may be
-breaking changes between versions without a major version update. Therefore, we
-recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ### Contributions While we value
-open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+( interval="WEEK", interval_count=791725, name="Ken Kshlerin", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), ],
+order_tax_amount=475, purchase_country="GB", purchase_currency="GBP",
+shipping_address=shared.Address( attention="Attn", city="London", country="GB",
+email="test.sam@test.com", family_name="Andersson", given_name="Adam",
+organization_name="recusandae", phone="+44795465131", postal_code="W1G 0PW",
+region="OH", street_address="33 Cavendish Square", street_address2="Floor 22 /
+Flat 2", title="Mr.", ), ), ) res = s.orders.create(req) if res.order is not
+None: # handle response ```   ## Available Resources and Operations ###
+authorizations * `cancel` - Cancel an existing authorization ### orders *
+`create` - Create a new order ### sessions * `create` - Create a new payment
+session * `read` - Read an existing payment session * `update` - Update an
+existing payment session ### tokens * `purchase` - Generate a consumer token
+### Maturity This SDK is in beta, and there may be breaking changes between
+versions without a major version update. Therefore, we recommend pinning usage
+to a specific package version. This way, you can install the same version each
+time without breaking changes unless you are intentionally looking for the
+latest version. ### Contributions While we value open-source contributions to
+this SDK, this library is generated programmatically. Feel free to open a PR or
+a Github issue as a proof of concept and we'll do our best to include it in a
+future release ! ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/
+docs/using-speakeasy/client-sdks)
```

### Comparing `klarna-orders-1.0.1/README.md` & `klarna-orders-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
                     interval="WEEK",
                     interval_count=297534,
-                    name="debitis",
+                    name="Larry Windler",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -118,17 +118,17 @@
                     size="small",
                 ),
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
-                    interval="DAY",
-                    interval_count=963663,
-                    name="tempora",
+                    interval="WEEK",
+                    interval_count=791725,
+                    name="Ken Kshlerin",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -140,15 +140,15 @@
         shipping_address=shared.Address(
             attention="Attn",
             city="London",
             country="GB",
             email="test.sam@test.com",
             family_name="Andersson",
             given_name="Adam",
-            organization_name="suscipit",
+            organization_name="recusandae",
             phone="+44795465131",
             postal_code="W1G 0PW",
             region="OH",
             street_address="33 Cavendish Square",
             street_address2="Floor 22 / Flat 2",
             title="Mr.",
         ),
```

#### html2text {}

```diff
@@ -36,41 +36,42 @@
 "test@gmail.com","account_registration_date":"2017-02-13T10:49:
 20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
 product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
 category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="WEEK", interval_count=297534, name="debitis", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), shared.OrderLine( image_url="https://
-www.exampleobjects.com/logo.png", merchant_data="{"customer_account_info":[
-{"unique_account_identifier":"test@gmail.com","account_registration_date":
-"2017-02-13T10:49:20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}",
-name="Running shoe", product_identifiers=shared.ProductIdentifiers
-( brand="shoe-brand", category_path="Shoes > Running", color="white",
+( interval="WEEK", interval_count=297534, name="Larry Windler", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), shared.OrderLine
+( image_url="https://www.exampleobjects.com/logo.png", merchant_data="
+{"customer_account_info":[{"unique_account_identifier":
+"test@gmail.com","account_registration_date":"2017-02-13T10:49:
+20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
+product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
+category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="DAY", interval_count=963663, name="tempora", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), ], order_tax_amount=475,
-purchase_country="GB", purchase_currency="GBP", shipping_address=shared.Address
-( attention="Attn", city="London", country="GB", email="test.sam@test.com",
-family_name="Andersson", given_name="Adam", organization_name="suscipit",
-phone="+44795465131", postal_code="W1G 0PW", region="OH", street_address="33
-Cavendish Square", street_address2="Floor 22 / Flat 2", title="Mr.", ), ), )
-res = s.orders.create(req) if res.order is not None: # handle response ```   ##
-Available Resources and Operations ### authorizations * `cancel` - Cancel an
-existing authorization ### orders * `create` - Create a new order ### sessions
-* `create` - Create a new payment session * `read` - Read an existing payment
-session * `update` - Update an existing payment session ### tokens * `purchase`
-- Generate a consumer token  ### Maturity This SDK is in beta, and there may be
-breaking changes between versions without a major version update. Therefore, we
-recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ### Contributions While we value
-open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+( interval="WEEK", interval_count=791725, name="Ken Kshlerin", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), ],
+order_tax_amount=475, purchase_country="GB", purchase_currency="GBP",
+shipping_address=shared.Address( attention="Attn", city="London", country="GB",
+email="test.sam@test.com", family_name="Andersson", given_name="Adam",
+organization_name="recusandae", phone="+44795465131", postal_code="W1G 0PW",
+region="OH", street_address="33 Cavendish Square", street_address2="Floor 22 /
+Flat 2", title="Mr.", ), ), ) res = s.orders.create(req) if res.order is not
+None: # handle response ```   ## Available Resources and Operations ###
+authorizations * `cancel` - Cancel an existing authorization ### orders *
+`create` - Create a new order ### sessions * `create` - Create a new payment
+session * `read` - Read an existing payment session * `update` - Update an
+existing payment session ### tokens * `purchase` - Generate a consumer token
+### Maturity This SDK is in beta, and there may be breaking changes between
+versions without a major version update. Therefore, we recommend pinning usage
+to a specific package version. This way, you can install the same version each
+time without breaking changes unless you are intentionally looking for the
+latest version. ### Contributions While we value open-source contributions to
+this SDK, this library is generated programmatically. Feel free to open a PR or
+a Github issue as a proof of concept and we'll do our best to include it in a
+future release ! ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/
+docs/using-speakeasy/client-sdks)
```

### Comparing `klarna-orders-1.0.1/setup.py` & `klarna-orders-1.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="klarna-orders",
-    version="1.0.1",
+    version="1.1.0",
     author="Speakeasy-Klarna",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `klarna-orders-1.0.1/src/klarna/authorizations.py` & `klarna-orders-1.1.0/src/klarna/authorizations.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/__init__.py` & `klarna-orders-1.1.0/src/klarna/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/cancelauthorization.py` & `klarna-orders-1.1.0/src/klarna/models/operations/cancelauthorization.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/createcreditsession.py` & `klarna-orders-1.1.0/src/klarna/models/operations/createcreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/createorder.py` & `klarna-orders-1.1.0/src/klarna/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/purchasetoken.py` & `klarna-orders-1.1.0/src/klarna/models/operations/purchasetoken.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/readcreditsession.py` & `klarna-orders-1.1.0/src/klarna/models/operations/readcreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/operations/updatecreditsession.py` & `klarna-orders-1.1.0/src/klarna/models/operations/updatecreditsession.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/__init__.py` & `klarna-orders-1.1.0/src/klarna/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/address.py` & `klarna-orders-1.1.0/src/klarna/models/shared/address.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/asset_urls.py` & `klarna-orders-1.1.0/src/klarna/models/shared/asset_urls.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/attachment.py` & `klarna-orders-1.1.0/src/klarna/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/authorized_payment_method.py` & `klarna-orders-1.1.0/src/klarna/models/shared/authorized_payment_method.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/create_order_request.py` & `klarna-orders-1.1.0/src/klarna/models/shared/create_order_request.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/customer.py` & `klarna-orders-1.1.0/src/klarna/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/customer_read.py` & `klarna-orders-1.1.0/src/klarna/models/shared/customer_read.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/customer_read_create_token.py` & `klarna-orders-1.1.0/src/klarna/models/shared/customer_read_create_token.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/customer_token_creation_request.py` & `klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_request.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/customer_token_creation_response.py` & `klarna-orders-1.1.0/src/klarna/models/shared/customer_token_creation_response.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/errorv2.py` & `klarna-orders-1.1.0/src/klarna/models/shared/errorv2.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/merchant_session.py` & `klarna-orders-1.1.0/src/klarna/models/shared/merchant_session.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/merchant_urls.py` & `klarna-orders-1.1.0/src/klarna/models/shared/merchant_urls.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/options.py` & `klarna-orders-1.1.0/src/klarna/models/shared/options.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/order.py` & `klarna-orders-1.1.0/src/klarna/models/shared/order.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/order_line.py` & `klarna-orders-1.1.0/src/klarna/models/shared/order_line.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/payment_method_category.py` & `klarna-orders-1.1.0/src/klarna/models/shared/payment_method_category.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/product_identifiers.py` & `klarna-orders-1.1.0/src/klarna/models/shared/product_identifiers.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/session.py` & `klarna-orders-1.1.0/src/klarna/models/shared/session.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/session_create.py` & `klarna-orders-1.1.0/src/klarna/models/shared/session_create.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/session_read.py` & `klarna-orders-1.1.0/src/klarna/models/shared/session_read.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/models/shared/subscription.py` & `klarna-orders-1.1.0/src/klarna/models/shared/subscription.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/orders.py` & `klarna-orders-1.1.0/src/klarna/orders.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/sdk.py` & `klarna-orders-1.1.0/src/klarna/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     tokens: Tokens
     r"""Operations related to token"""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.0.1"
-    _gen_version: str = "2.17.8"
+    _sdk_version: str = "1.1.0"
+    _gen_version: str = "2.18.0"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `klarna-orders-1.0.1/src/klarna/sessions.py` & `klarna-orders-1.1.0/src/klarna/sessions.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/tokens.py` & `klarna-orders-1.1.0/src/klarna/tokens.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/utils/retries.py` & `klarna-orders-1.1.0/src/klarna/utils/retries.py`

 * *Files identical despite different names*

### Comparing `klarna-orders-1.0.1/src/klarna/utils/utils.py` & `klarna-orders-1.1.0/src/klarna/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -148,70 +148,79 @@
         if request_metadata is not None:
             continue
 
         param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        if param_metadata.get('style', 'simple') == 'simple':
-            param = getattr(
-                path_params, field.name) if path_params is not None else None
-            param = _populate_from_globals(
-                field.name, param, 'pathParam', gbls)
-
-            if param is None:
-                continue
-
-            if isinstance(param, list):
-                pp_vals: list[str] = []
-                for pp_val in param:
-                    if pp_val is None:
-                        continue
-                    pp_vals.append(_val_to_string(pp_val))
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif isinstance(param, dict):
-                pp_vals: list[str] = []
-                for pp_key in param:
-                    if param[pp_key] is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{pp_key}={_val_to_string(param[pp_key])}")
-                    else:
-                        pp_vals.append(
-                            f"{pp_key},{_val_to_string(param[pp_key])}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            elif not isinstance(param, (str, int, float, complex, bool)):
-                pp_vals: list[str] = []
-                param_fields: Tuple[Field, ...] = fields(param)
-                for param_field in param_fields:
-                    param_value_metadata = param_field.metadata.get(
-                        'path_param')
-                    if not param_value_metadata:
-                        continue
-
-                    parm_name = param_value_metadata.get(
-                        'field_name', field.name)
-
-                    param_field_val = getattr(param, param_field.name)
-                    if param_field_val is None:
-                        continue
-                    if param_metadata.get('explode'):
-                        pp_vals.append(
-                            f"{parm_name}={_val_to_string(param_field_val)}")
-                    else:
-                        pp_vals.append(
-                            f"{parm_name},{_val_to_string(param_field_val)}")
-                path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
-            else:
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
+
+        if param is None:
+            continue
+
+        f_name = param_metadata.get("field_name", field.name)
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
+            serialized_params = _get_serialized_params(
+                param_metadata, f_name, param)
+            for key, value in serialized_params.items():
                 path = path.replace(
-                    '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    '{' + key + '}', value, 1)
+        else:
+            if param_metadata.get('style', 'simple') == 'simple':
+                if isinstance(param, list):
+                    pp_vals: list[str] = []
+                    for pp_val in param:
+                        if pp_val is None:
+                            continue
+                        pp_vals.append(_val_to_string(pp_val))
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif isinstance(param, dict):
+                    pp_vals: list[str] = []
+                    for pp_key in param:
+                        if param[pp_key] is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        else:
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                elif not isinstance(param, (str, int, float, complex, bool)):
+                    pp_vals: list[str] = []
+                    param_fields: Tuple[Field, ...] = fields(param)
+                    for param_field in param_fields:
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
+                        if not param_value_metadata:
+                            continue
+
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
+
+                        param_field_val = getattr(param, param_field.name)
+                        if param_field_val is None:
+                            continue
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{parm_name}={_val_to_string(param_field_val)}")
+                        else:
+                            pp_vals.append(
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                else:
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
     return server_url.removesuffix("/") + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
@@ -242,16 +251,20 @@
             query_params, param_name) if query_params is not None else None
 
         value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
         serialization = metadata.get('serialization', '')
         if serialization != '':
-            params = params | _get_serialized_query_params(
-                metadata, f_name, value)
+            serialized_parms = _get_serialized_params(metadata, f_name, value)
+            for key, value in serialized_parms.items():
+                if key in params:
+                    params[key].extend(value)
+                else:
+                    params[key] = [value]
         else:
             style = metadata.get('style', 'form')
             if style == 'deepObject':
                 params = params | _get_deep_object_query_params(
                     metadata, f_name, value)
             elif style == 'form':
                 params = params | _get_form_query_params(
@@ -278,16 +291,16 @@
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
 
 
-def _get_serialized_query_params(metadata: dict, field_name: str, obj: any) -> dict[str, list[str]]:
-    params: dict[str, list[str]] = {}
+def _get_serialized_params(metadata: dict, field_name: str, obj: any) -> dict[str, str]:
+    params: dict[str, str] = {}
 
     serialization = metadata.get('serialization', '')
     if serialization == 'json':
         params[metadata.get("field_name", field_name)] = marshal_json(obj)
 
     return params
```

### Comparing `klarna-orders-1.0.1/src/klarna_orders.egg-info/PKG-INFO` & `klarna-orders-1.1.0/src/klarna_orders.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: klarna-orders
-Version: 1.0.1
+Version: 1.1.0
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy-Klarna
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -104,15 +104,15 @@
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
                     interval="WEEK",
                     interval_count=297534,
-                    name="debitis",
+                    name="Larry Windler",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -130,17 +130,17 @@
                     size="small",
                 ),
                 product_url="https://.../AD6654412.html",
                 quantity=1,
                 quantity_unit="pcs",
                 reference="AD6654412",
                 subscription=shared.Subscription(
-                    interval="DAY",
-                    interval_count=963663,
-                    name="tempora",
+                    interval="WEEK",
+                    interval_count=791725,
+                    name="Ken Kshlerin",
                 ),
                 tax_rate=1900,
                 total_amount=2500,
                 total_discount_amount=500,
                 total_tax_amount=475,
                 type="physical",
                 unit_price=2500,
@@ -152,15 +152,15 @@
         shipping_address=shared.Address(
             attention="Attn",
             city="London",
             country="GB",
             email="test.sam@test.com",
             family_name="Andersson",
             given_name="Adam",
-            organization_name="suscipit",
+            organization_name="recusandae",
             phone="+44795465131",
             postal_code="W1G 0PW",
             region="OH",
             street_address="33 Cavendish Square",
             street_address2="Floor 22 / Flat 2",
             title="Mr.",
         ),
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: klarna-orders Version: 1.0.1 Summary: Python Client
+Metadata-Version: 2.1 Name: klarna-orders Version: 1.1.0 Summary: Python Client
 SDK Generated by Speakeasy Home-page: UNKNOWN Author: Speakeasy-Klarna License:
 UNKNOWN Platform: UNKNOWN Requires-Python: >=3.9 Description-Content-Type:
 text/markdown License-File: LICENSE.md
   [https://user-images.githubusercontent.com/6267663/230347878-f2873a58-f578-
                           4e95-86e0-7bebfd78f4f1.svg]
                            ****** Python SDK ******
                 An effortless integration. Designed for growth.
@@ -40,41 +40,42 @@
 "test@gmail.com","account_registration_date":"2017-02-13T10:49:
 20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
 product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
 category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="WEEK", interval_count=297534, name="debitis", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), shared.OrderLine( image_url="https://
-www.exampleobjects.com/logo.png", merchant_data="{"customer_account_info":[
-{"unique_account_identifier":"test@gmail.com","account_registration_date":
-"2017-02-13T10:49:20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}",
-name="Running shoe", product_identifiers=shared.ProductIdentifiers
-( brand="shoe-brand", category_path="Shoes > Running", color="white",
+( interval="WEEK", interval_count=297534, name="Larry Windler", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), shared.OrderLine
+( image_url="https://www.exampleobjects.com/logo.png", merchant_data="
+{"customer_account_info":[{"unique_account_identifier":
+"test@gmail.com","account_registration_date":"2017-02-13T10:49:
+20Z","account_last_modified":"2019-03-13T11:45:27Z"}]}", name="Running shoe",
+product_identifiers=shared.ProductIdentifiers( brand="shoe-brand",
+category_path="Shoes > Running", color="white",
 global_trade_item_number="4912345678904", manufacturer_part_number="AD6654412-
 334.22", size="small", ), product_url="https://.../AD6654412.html", quantity=1,
 quantity_unit="pcs", reference="AD6654412", subscription=shared.Subscription
-( interval="DAY", interval_count=963663, name="tempora", ), tax_rate=1900,
-total_amount=2500, total_discount_amount=500, total_tax_amount=475,
-type="physical", unit_price=2500, ), ], order_tax_amount=475,
-purchase_country="GB", purchase_currency="GBP", shipping_address=shared.Address
-( attention="Attn", city="London", country="GB", email="test.sam@test.com",
-family_name="Andersson", given_name="Adam", organization_name="suscipit",
-phone="+44795465131", postal_code="W1G 0PW", region="OH", street_address="33
-Cavendish Square", street_address2="Floor 22 / Flat 2", title="Mr.", ), ), )
-res = s.orders.create(req) if res.order is not None: # handle response ```   ##
-Available Resources and Operations ### authorizations * `cancel` - Cancel an
-existing authorization ### orders * `create` - Create a new order ### sessions
-* `create` - Create a new payment session * `read` - Read an existing payment
-session * `update` - Update an existing payment session ### tokens * `purchase`
-- Generate a consumer token  ### Maturity This SDK is in beta, and there may be
-breaking changes between versions without a major version update. Therefore, we
-recommend pinning usage to a specific package version. This way, you can
-install the same version each time without breaking changes unless you are
-intentionally looking for the latest version. ### Contributions While we value
-open-source contributions to this SDK, this library is generated
-programmatically. Feel free to open a PR or a Github issue as a proof of
-concept and we'll do our best to include it in a future release ! ### SDK
-Created by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/
-client-sdks)
+( interval="WEEK", interval_count=791725, name="Ken Kshlerin", ),
+tax_rate=1900, total_amount=2500, total_discount_amount=500,
+total_tax_amount=475, type="physical", unit_price=2500, ), ],
+order_tax_amount=475, purchase_country="GB", purchase_currency="GBP",
+shipping_address=shared.Address( attention="Attn", city="London", country="GB",
+email="test.sam@test.com", family_name="Andersson", given_name="Adam",
+organization_name="recusandae", phone="+44795465131", postal_code="W1G 0PW",
+region="OH", street_address="33 Cavendish Square", street_address2="Floor 22 /
+Flat 2", title="Mr.", ), ), ) res = s.orders.create(req) if res.order is not
+None: # handle response ```   ## Available Resources and Operations ###
+authorizations * `cancel` - Cancel an existing authorization ### orders *
+`create` - Create a new order ### sessions * `create` - Create a new payment
+session * `read` - Read an existing payment session * `update` - Update an
+existing payment session ### tokens * `purchase` - Generate a consumer token
+### Maturity This SDK is in beta, and there may be breaking changes between
+versions without a major version update. Therefore, we recommend pinning usage
+to a specific package version. This way, you can install the same version each
+time without breaking changes unless you are intentionally looking for the
+latest version. ### Contributions While we value open-source contributions to
+this SDK, this library is generated programmatically. Feel free to open a PR or
+a Github issue as a proof of concept and we'll do our best to include it in a
+future release ! ### SDK Created by [Speakeasy](https://docs.speakeasyapi.dev/
+docs/using-speakeasy/client-sdks)
```

### Comparing `klarna-orders-1.0.1/src/klarna_orders.egg-info/SOURCES.txt` & `klarna-orders-1.1.0/src/klarna_orders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

