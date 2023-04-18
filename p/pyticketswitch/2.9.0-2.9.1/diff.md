# Comparing `tmp/pyticketswitch-2.9.0.tar.gz` & `tmp/pyticketswitch-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyticketswitch-2.9.0.tar", last modified: Thu Mar 24 17:04:53 2022, max compression
+gzip compressed data, was "pyticketswitch-2.9.1.tar", last modified: Mon Apr  4 11:56:50 2022, max compression
```

## Comparing `pyticketswitch-2.9.0.tar` & `pyticketswitch-2.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-03-24 17:04:53.446184 pyticketswitch-2.9.0/
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1058 2022-03-17 14:47:23.000000 pyticketswitch-2.9.0/LICENSE
--rw-r--r--   0 shannonkelly   (501) staff       (20)      516 2022-03-24 17:04:53.446393 pyticketswitch-2.9.0/PKG-INFO
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2098 2022-03-17 14:47:23.000000 pyticketswitch-2.9.0/README.md
-drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-03-24 17:04:53.442859 pyticketswitch-2.9.0/pyticketswitch/
--rw-r--r--   0 shannonkelly   (501) staff       (20)       73 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/__init__.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2727 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/address.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)    12641 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/availability.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     6498 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/bundle.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     5465 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/callout.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1188 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/cancellation.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)      513 2022-03-23 15:19:17.000000 pyticketswitch-2.9.0/pyticketswitch/card_type.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)    65507 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/client.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1380 2022-03-23 15:19:17.000000 pyticketswitch-2.9.0/pyticketswitch/commission.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1098 2022-03-23 15:19:17.000000 pyticketswitch-2.9.0/pyticketswitch/content.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     9703 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/cost_range.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1131 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/country.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     6204 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/currency.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     8650 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/customer.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2905 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/debitor.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     4249 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/discount.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)    18807 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/event.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1225 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/exceptions.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1081 2022-03-23 15:19:17.000000 pyticketswitch-2.9.0/pyticketswitch/field.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1930 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/media.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)        0 2022-03-17 14:47:23.000000 pyticketswitch-2.9.0/pyticketswitch/meta.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)      151 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/misc.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     8560 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/mixins.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     4496 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/month.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1973 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/offer.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)    18316 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/order.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     9038 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/payment_methods.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     7087 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/performance.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     8821 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/price_band.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2633 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/purchase_result.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     4018 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/reservation.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2132 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/review.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     5852 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/seat.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     3229 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/pyticketswitch/send_method.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     7698 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/status.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2229 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/ticket_type.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     6602 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/trolley.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     2164 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/user.py
--rw-r--r--   0 shannonkelly   (501) staff       (20)     6757 2022-03-24 15:07:57.000000 pyticketswitch-2.9.0/pyticketswitch/utils.py
-drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-03-24 17:04:53.445777 pyticketswitch-2.9.0/pyticketswitch.egg-info/
--rw-r--r--   0 shannonkelly   (501) staff       (20)      516 2022-03-24 17:04:53.000000 pyticketswitch-2.9.0/pyticketswitch.egg-info/PKG-INFO
--rw-r--r--   0 shannonkelly   (501) staff       (20)     1268 2022-03-24 17:04:53.000000 pyticketswitch-2.9.0/pyticketswitch.egg-info/SOURCES.txt
--rw-r--r--   0 shannonkelly   (501) staff       (20)        1 2022-03-24 17:04:53.000000 pyticketswitch-2.9.0/pyticketswitch.egg-info/dependency_links.txt
--rw-r--r--   0 shannonkelly   (501) staff       (20)       50 2022-03-24 17:04:53.000000 pyticketswitch-2.9.0/pyticketswitch.egg-info/requires.txt
--rw-r--r--   0 shannonkelly   (501) staff       (20)       15 2022-03-24 17:04:53.000000 pyticketswitch-2.9.0/pyticketswitch.egg-info/top_level.txt
--rw-r--r--   0 shannonkelly   (501) staff       (20)      393 2022-03-24 17:04:53.451182 pyticketswitch-2.9.0/setup.cfg
--rw-r--r--   0 shannonkelly   (501) staff       (20)      740 2022-03-24 17:00:51.000000 pyticketswitch-2.9.0/setup.py
+drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-04-04 11:56:50.759584 pyticketswitch-2.9.1/
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1058 2022-03-17 14:47:23.000000 pyticketswitch-2.9.1/LICENSE
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      516 2022-04-04 11:56:50.760524 pyticketswitch-2.9.1/PKG-INFO
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2098 2022-03-17 14:47:23.000000 pyticketswitch-2.9.1/README.md
+drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-04-04 11:56:50.755974 pyticketswitch-2.9.1/pyticketswitch/
+-rw-r--r--   0 shannonkelly   (501) staff       (20)       73 2022-04-04 11:52:00.000000 pyticketswitch-2.9.1/pyticketswitch/__init__.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2727 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/address.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)    12641 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/availability.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     6786 2022-04-04 11:20:53.000000 pyticketswitch-2.9.1/pyticketswitch/bundle.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     5465 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/callout.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1188 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/cancellation.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      513 2022-03-23 15:19:17.000000 pyticketswitch-2.9.1/pyticketswitch/card_type.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)    65507 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/client.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1380 2022-03-23 15:19:17.000000 pyticketswitch-2.9.1/pyticketswitch/commission.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1098 2022-03-23 15:19:17.000000 pyticketswitch-2.9.1/pyticketswitch/content.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     9703 2022-03-24 17:00:51.000000 pyticketswitch-2.9.1/pyticketswitch/cost_range.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1131 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/country.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     6204 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/currency.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     8650 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/customer.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2905 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/debitor.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     4249 2022-03-24 17:00:51.000000 pyticketswitch-2.9.1/pyticketswitch/discount.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)    18807 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/event.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1225 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/exceptions.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1081 2022-03-23 15:19:17.000000 pyticketswitch-2.9.1/pyticketswitch/field.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1930 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/media.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)        0 2022-03-17 14:47:23.000000 pyticketswitch-2.9.1/pyticketswitch/meta.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      151 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/misc.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     8560 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/mixins.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     4496 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/month.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1973 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/offer.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)    18316 2022-03-24 17:00:51.000000 pyticketswitch-2.9.1/pyticketswitch/order.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     9038 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/payment_methods.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     7087 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/performance.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     8821 2022-03-24 17:00:51.000000 pyticketswitch-2.9.1/pyticketswitch/price_band.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2633 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/purchase_result.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     4018 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/reservation.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2132 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/review.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     5852 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/seat.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     3229 2022-03-24 17:00:51.000000 pyticketswitch-2.9.1/pyticketswitch/send_method.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     7698 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/status.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2229 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/ticket_type.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     6602 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/trolley.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     2164 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/user.py
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     6757 2022-03-24 15:07:57.000000 pyticketswitch-2.9.1/pyticketswitch/utils.py
+drwxr-xr-x   0 shannonkelly   (501) staff       (20)        0 2022-04-04 11:56:50.759210 pyticketswitch-2.9.1/pyticketswitch.egg-info/
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      516 2022-04-04 11:56:50.000000 pyticketswitch-2.9.1/pyticketswitch.egg-info/PKG-INFO
+-rw-r--r--   0 shannonkelly   (501) staff       (20)     1268 2022-04-04 11:56:50.000000 pyticketswitch-2.9.1/pyticketswitch.egg-info/SOURCES.txt
+-rw-r--r--   0 shannonkelly   (501) staff       (20)        1 2022-04-04 11:56:50.000000 pyticketswitch-2.9.1/pyticketswitch.egg-info/dependency_links.txt
+-rw-r--r--   0 shannonkelly   (501) staff       (20)       50 2022-04-04 11:56:50.000000 pyticketswitch-2.9.1/pyticketswitch.egg-info/requires.txt
+-rw-r--r--   0 shannonkelly   (501) staff       (20)       15 2022-04-04 11:56:50.000000 pyticketswitch-2.9.1/pyticketswitch.egg-info/top_level.txt
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      393 2022-04-04 11:56:50.761262 pyticketswitch-2.9.1/setup.cfg
+-rw-r--r--   0 shannonkelly   (501) staff       (20)      740 2022-04-04 11:52:00.000000 pyticketswitch-2.9.1/setup.py
```

### Comparing `pyticketswitch-2.9.0/LICENSE` & `pyticketswitch-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/PKG-INFO` & `pyticketswitch-2.9.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyticketswitch
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python interface for the Ingresso F13 API
 Home-page: https://github.com/ingresso-group/pyticketswitch/
 Author: Ingresso
 Author-email: systems@ingresso.co.uk
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyticketswitch-2.9.0/README.md` & `pyticketswitch-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/address.py` & `pyticketswitch-2.9.1/pyticketswitch/address.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/availability.py` & `pyticketswitch-2.9.1/pyticketswitch/availability.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/bundle.py` & `pyticketswitch-2.9.1/pyticketswitch/bundle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyticketswitch.order import Order
 from pyticketswitch.mixins import JSONMixin
 from pyticketswitch.debitor import Debitor
+from pyticketswitch.purchase_result import PurchaseResult
 
 
 class Bundle(JSONMixin, object):
     """A collection of orders into the same backend system
 
     Attributes:
         source_code (str): the identifier of the backend system.
@@ -112,14 +113,19 @@
             kwargs.update(total=total)
 
         raw_debitor = data.get('debitor')
         if raw_debitor:
             debitor = Debitor.from_api_data(raw_debitor)
             kwargs.update(debitor=debitor)
 
+        raw_purchase_result = data.get('purchase_result')
+        if raw_purchase_result:
+            purchase_result = PurchaseResult.from_api_data(raw_purchase_result)
+            kwargs.update(purchase_result=purchase_result)
+
         total = data.get('bundle_total_cost')
         if total is not None:
             kwargs.update(total=total)
 
         send_cost_tax_component = data.get('bundle_send_cost_tax_component')
         if send_cost_tax_component is not None:
             kwargs.update(send_cost_tax_component=send_cost_tax_component)
```

### Comparing `pyticketswitch-2.9.0/pyticketswitch/callout.py` & `pyticketswitch-2.9.1/pyticketswitch/callout.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/cancellation.py` & `pyticketswitch-2.9.1/pyticketswitch/cancellation.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/card_type.py` & `pyticketswitch-2.9.1/pyticketswitch/card_type.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/client.py` & `pyticketswitch-2.9.1/pyticketswitch/client.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/commission.py` & `pyticketswitch-2.9.1/pyticketswitch/commission.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/content.py` & `pyticketswitch-2.9.1/pyticketswitch/content.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/cost_range.py` & `pyticketswitch-2.9.1/pyticketswitch/cost_range.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/country.py` & `pyticketswitch-2.9.1/pyticketswitch/country.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/currency.py` & `pyticketswitch-2.9.1/pyticketswitch/currency.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/customer.py` & `pyticketswitch-2.9.1/pyticketswitch/customer.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/debitor.py` & `pyticketswitch-2.9.1/pyticketswitch/debitor.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/discount.py` & `pyticketswitch-2.9.1/pyticketswitch/discount.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/event.py` & `pyticketswitch-2.9.1/pyticketswitch/event.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/exceptions.py` & `pyticketswitch-2.9.1/pyticketswitch/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/field.py` & `pyticketswitch-2.9.1/pyticketswitch/field.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/media.py` & `pyticketswitch-2.9.1/pyticketswitch/media.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/mixins.py` & `pyticketswitch-2.9.1/pyticketswitch/mixins.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/month.py` & `pyticketswitch-2.9.1/pyticketswitch/month.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/offer.py` & `pyticketswitch-2.9.1/pyticketswitch/offer.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/order.py` & `pyticketswitch-2.9.1/pyticketswitch/order.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/payment_methods.py` & `pyticketswitch-2.9.1/pyticketswitch/payment_methods.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/performance.py` & `pyticketswitch-2.9.1/pyticketswitch/performance.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/price_band.py` & `pyticketswitch-2.9.1/pyticketswitch/price_band.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/purchase_result.py` & `pyticketswitch-2.9.1/pyticketswitch/purchase_result.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/reservation.py` & `pyticketswitch-2.9.1/pyticketswitch/reservation.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/review.py` & `pyticketswitch-2.9.1/pyticketswitch/review.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/seat.py` & `pyticketswitch-2.9.1/pyticketswitch/seat.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/send_method.py` & `pyticketswitch-2.9.1/pyticketswitch/send_method.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/status.py` & `pyticketswitch-2.9.1/pyticketswitch/status.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/ticket_type.py` & `pyticketswitch-2.9.1/pyticketswitch/ticket_type.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/trolley.py` & `pyticketswitch-2.9.1/pyticketswitch/trolley.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/user.py` & `pyticketswitch-2.9.1/pyticketswitch/user.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch/utils.py` & `pyticketswitch-2.9.1/pyticketswitch/utils.py`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/pyticketswitch.egg-info/PKG-INFO` & `pyticketswitch-2.9.1/pyticketswitch.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pyticketswitch
-Version: 2.9.0
+Version: 2.9.1
 Summary: A Python interface for the Ingresso F13 API
 Home-page: https://github.com/ingresso-group/pyticketswitch/
 Author: Ingresso
 Author-email: systems@ingresso.co.uk
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pyticketswitch-2.9.0/pyticketswitch.egg-info/SOURCES.txt` & `pyticketswitch-2.9.1/pyticketswitch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyticketswitch-2.9.0/setup.py` & `pyticketswitch-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='pyticketswitch',
-    version='2.9.0',
+    version='2.9.1',
     author='Ingresso',
     author_email='systems@ingresso.co.uk',
     url='https://github.com/ingresso-group/pyticketswitch/',
     packages=[
         'pyticketswitch',
     ],
     license='MIT',
```

