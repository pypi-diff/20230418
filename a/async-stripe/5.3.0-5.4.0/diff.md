# Comparing `tmp/async_stripe-5.3.0.tar.gz` & `tmp/async_stripe-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_stripe-5.3.0.tar", max compression
+gzip compressed data, was "async_stripe-5.4.0.tar", max compression
```

## Comparing `async_stripe-5.3.0.tar` & `async_stripe-5.4.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1091 2023-03-29 08:39:03.154980 async_stripe-5.3.0/LICENSE.stripe.txt
--rw-r--r--   0        0        0     1478 2023-03-29 08:39:03.154980 async_stripe-5.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3017 2023-03-29 08:39:03.154980 async_stripe-5.3.0/README.md
--rw-r--r--   0        0        0      340 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/__init__.py
--rw-r--r--   0        0        0     5793 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_requestor.py
--rw-r--r--   0        0        0      973 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/__init__.py
--rw-r--r--   0        0        0      538 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/__init__.py
--rw-r--r--   0        0        0     3835 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0        0        0     2620 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0        0        0      428 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0        0        0      882 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0        0        0      554 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0        0        0      879 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0        0        0      568 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/account.py
--rw-r--r--   0        0        0      291 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/application_fee.py
--rw-r--r--   0        0        0      340 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/application_fee_refund.py
--rw-r--r--   0        0        0     1213 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/bank_account.py
--rw-r--r--   0        0        0      635 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/capability.py
--rw-r--r--   0        0        0     1101 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/card.py
--rw-r--r--   0        0        0      757 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/charge.py
--rw-r--r--   0        0        0      286 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/customer.py
--rw-r--r--   0        0        0      835 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/ephermal_key.py
--rw-r--r--   0        0        0      930 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/file.py
--rw-r--r--   0        0        0     2105 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/list_object.py
--rw-r--r--   0        0        0      707 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/person.py
--rw-r--r--   0        0        0     1319 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/quote.py
--rw-r--r--   0        0        0      737 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/reversal.py
--rw-r--r--   0        0        0     1046 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/search_result_object.py
--rw-r--r--   0        0        0      930 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/source.py
--rw-r--r--   0        0        0      227 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/transfer.py
--rw-r--r--   0        0        0      874 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/api_resources/usage_record.py
--rw-r--r--   0        0        0     4866 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/http_client.py
--rw-r--r--   0        0        0      732 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/oauth.py
--rw-r--r--   0        0        0     2066 2023-03-29 08:39:03.154980 async_stripe-5.3.0/async_stripe/stripe_object.py
--rw-r--r--   0        0        0      885 2023-03-29 08:39:03.154980 async_stripe-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 async_stripe-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-04-18 15:48:23.537321 async_stripe-5.4.0/LICENSE.stripe.txt
+-rw-r--r--   0        0        0     1478 2023-04-18 15:48:23.537321 async_stripe-5.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     3017 2023-04-18 15:48:23.537321 async_stripe-5.4.0/README.md
+-rw-r--r--   0        0        0      340 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/__init__.py
+-rw-r--r--   0        0        0     5793 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_requestor.py
+-rw-r--r--   0        0        0      973 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/__init__.py
+-rw-r--r--   0        0        0      538 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0        0        0     3835 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0        0        0     2620 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0        0        0      428 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0        0        0      882 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0        0        0      554 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0        0        0      879 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0        0        0      568 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/account.py
+-rw-r--r--   0        0        0      291 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/application_fee.py
+-rw-r--r--   0        0        0      340 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/application_fee_refund.py
+-rw-r--r--   0        0        0     1213 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/bank_account.py
+-rw-r--r--   0        0        0      635 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/capability.py
+-rw-r--r--   0        0        0     1101 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/card.py
+-rw-r--r--   0        0        0      757 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/charge.py
+-rw-r--r--   0        0        0      286 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/customer.py
+-rw-r--r--   0        0        0      835 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/ephermal_key.py
+-rw-r--r--   0        0        0      930 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/file.py
+-rw-r--r--   0        0        0     2105 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/list_object.py
+-rw-r--r--   0        0        0      707 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/person.py
+-rw-r--r--   0        0        0     1319 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/quote.py
+-rw-r--r--   0        0        0      737 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/reversal.py
+-rw-r--r--   0        0        0     1046 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/search_result_object.py
+-rw-r--r--   0        0        0      930 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/source.py
+-rw-r--r--   0        0        0      227 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/transfer.py
+-rw-r--r--   0        0        0      874 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/api_resources/usage_record.py
+-rw-r--r--   0        0        0     4866 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/http_client.py
+-rw-r--r--   0        0        0      732 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/oauth.py
+-rw-r--r--   0        0        0     2066 2023-04-18 15:48:23.537321 async_stripe-5.4.0/async_stripe/stripe_object.py
+-rw-r--r--   0        0        0      885 2023-04-18 15:48:23.541319 async_stripe-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3977 1970-01-01 00:00:00.000000 async_stripe-5.4.0/PKG-INFO
```

### Comparing `async_stripe-5.3.0/LICENSE.stripe.txt` & `async_stripe-5.4.0/LICENSE.stripe.txt`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/LICENSE.txt` & `async_stripe-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/README.md` & `async_stripe-5.4.0/README.md`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_requestor.py` & `async_stripe-5.4.0/async_stripe/api_requestor.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/__init__.py` & `async_stripe-5.4.0/async_stripe/api_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/__init__.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/api_resource.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/custom_method.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/nested_resource_class_methods.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/test_helpers.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/test_helpers.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/abstract/updateable_api_resource.py` & `async_stripe-5.4.0/async_stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/account.py` & `async_stripe-5.4.0/async_stripe/api_resources/account.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/bank_account.py` & `async_stripe-5.4.0/async_stripe/api_resources/bank_account.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/capability.py` & `async_stripe-5.4.0/async_stripe/api_resources/capability.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/card.py` & `async_stripe-5.4.0/async_stripe/api_resources/card.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/charge.py` & `async_stripe-5.4.0/async_stripe/api_resources/charge.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/ephermal_key.py` & `async_stripe-5.4.0/async_stripe/api_resources/ephermal_key.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/file.py` & `async_stripe-5.4.0/async_stripe/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/list_object.py` & `async_stripe-5.4.0/async_stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/person.py` & `async_stripe-5.4.0/async_stripe/api_resources/person.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/quote.py` & `async_stripe-5.4.0/async_stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/reversal.py` & `async_stripe-5.4.0/async_stripe/api_resources/reversal.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/search_result_object.py` & `async_stripe-5.4.0/async_stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/source.py` & `async_stripe-5.4.0/async_stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/api_resources/usage_record.py` & `async_stripe-5.4.0/async_stripe/api_resources/usage_record.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/http_client.py` & `async_stripe-5.4.0/async_stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/oauth.py` & `async_stripe-5.4.0/async_stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/async_stripe/stripe_object.py` & `async_stripe-5.4.0/async_stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `async_stripe-5.3.0/pyproject.toml` & `async_stripe-5.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-stripe"
-version = "5.3.0"
+version = "5.4.0"
 description = "An asynchronous wrapper around Stripe's official python library."
 authors = [
     "Bharat Chauhan <tell.bhch@gmail.com>", 
     "Christian Glacet <cglacet@kune.tech>",
 ]
 maintainers = [
     "Bharat Chauhan <tell.bhch@gmail.com>", 
@@ -16,15 +16,15 @@
 ]
 repository = "https://github.com/bhch/async-stripe"
 readme = "README.md"
 keywords = ["stripe", "async", "asynchronous", "wrapper"]
 
 [tool.poetry.dependencies]
 python = "^3.6"
-stripe = "5.3.0"
+stripe = "5.4.0"
 tornado = ">=5.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.0"
 mypy = "^0.940"
 flake8 = "^3.9.2"
 pytest = "7.0.1"
```

### Comparing `async_stripe-5.3.0/PKG-INFO` & `async_stripe-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-stripe
-Version: 5.3.0
+Version: 5.4.0
 Summary: An asynchronous wrapper around Stripe's official python library.
 Home-page: https://github.com/bhch/async-stripe
 License: BSD 3-Clause
 Keywords: stripe,async,asynchronous,wrapper
 Author: Bharat Chauhan
 Author-email: tell.bhch@gmail.com
 Maintainer: Bharat Chauhan
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: stripe (==5.3.0)
+Requires-Dist: stripe (==5.4.0)
 Requires-Dist: tornado (>=5.1)
 Project-URL: Repository, https://github.com/bhch/async-stripe
 Description-Content-Type: text/markdown
 
 # async-stripe
 
 [![Build Status](https://github.com/bhch/async-stripe/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/bhch/async-stripe/actions/workflows/ci.yml)
```

