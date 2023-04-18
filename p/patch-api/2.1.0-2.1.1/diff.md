# Comparing `tmp/patch-api-2.1.0.tar.gz` & `tmp/patch-api-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/patch-python/patch-python/dist/tmp8xaj6hfc/patch-api-2.1.0.tar", last modified: Tue Apr  4 22:39:01 2023, max compression
+gzip compressed data, was "/home/runner/work/patch-python/patch-python/dist/tmp96phr26q/patch-api-2.1.1.tar", last modified: Tue Apr 18 21:47:20 2023, max compression
```

## Comparing `patch-api-2.1.0.tar` & `patch-api-2.1.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-04 22:39:01.000000 patch-api-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-04 22:39:01.000000 patch-api-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api/
--rw-r--r--   0 runner    (1001) docker     (122)    12988 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (122)    25703 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api/models/
--rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_response.py
--rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_air_shipping_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    11272 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/update_order_line_item_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    20183 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_road_shipping_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/place_order_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/delete_order_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4065 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/photo.py
--rw-r--r--   0 runner    (1001) docker     (122)     9734 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_flight_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     7882 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_ethereum_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/highlight.py
--rw-r--r--   0 runner    (1001) docker     (122)     5926 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_list_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4460 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_success_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     9436 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_shipping_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     7177 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_bitcoin_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/technology_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/error_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     9460 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_ecommerce_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    14253 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_order_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4000 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/meta_index_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     9157 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_hotel_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    12033 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_order_line_item_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_issued_to.py
--rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_line_item_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     4957 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/estimate_response.py
--rw-r--r--   0 runner    (1001) docker     (122)    20129 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_line_item_project.py
--rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/parent_technology_type.py
--rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/project_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/estimate_list_response.py
--rw-r--r--   0 runner    (1001) docker     (122)    10711 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/inventory.py
--rw-r--r--   0 runner    (1001) docker     (122)    13924 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_rail_shipping_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)    16571 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order.py
--rw-r--r--   0 runner    (1001) docker     (122)    12631 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/order_line_item.py
--rw-r--r--   0 runner    (1001) docker     (122)     5819 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_mass_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/estimate.py
--rw-r--r--   0 runner    (1001) docker     (122)     8136 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_vehicle_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/project_list_response.py
--rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/sdg.py
--rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/technology_type_list_response.py
--rw-r--r--   0 runner    (1001) docker     (122)    17526 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/create_sea_shipping_estimate_request.py
--rw-r--r--   0 runner    (1001) docker     (122)     5467 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api/api/
--rw-r--r--   0 runner    (1001) docker     (122)   124704 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/estimates_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    50874 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/orders_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/technology_types_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18654 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    29947 2023-04-04 22:37:50.000000 patch-api-2.1.0/patch_api/api/order_line_items_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     8625 2023-04-04 22:37:50.000000 patch-api-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2355 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 22:39:01.000000 patch-api-2.1.0/patch_api.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 22:39:01.000000 patch-api-2.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)    10721 2023-04-04 22:37:50.000000 patch-api-2.1.0/test/test_orders_api.py
--rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-04-04 22:37:50.000000 patch-api-2.1.0/test/test_estimates_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     5257 2023-04-04 22:37:50.000000 patch-api-2.1.0/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-04-04 22:37:50.000000 patch-api-2.1.0/test/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-04 22:37:50.000000 patch-api-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-18 21:47:20.000000 patch-api-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8625 2023-04-18 21:46:07.000000 patch-api-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-04-18 21:47:20.000000 patch-api-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-04-18 21:46:07.000000 patch-api-2.1.1/test/test_estimates_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5791 2023-04-18 21:46:07.000000 patch-api-2.1.1/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2089 2023-04-18 21:46:07.000000 patch-api-2.1.1/test/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10721 2023-04-18 21:46:07.000000 patch-api-2.1.1/test/test_orders_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      347 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api/models/
+-rw-r--r--   0 runner    (1001) docker     (122)    10711 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13924 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_rail_shipping_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3399 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4003 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_issued_to.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5995 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/estimate_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4640 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_line_item_project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5819 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_mass_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11272 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/update_order_line_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9734 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_flight_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12631 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4990 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/delete_order_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_line_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4000 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/meta_index_object.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5613 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/technology_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5972 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/project_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/project_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16693 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6926 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/disclaimer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9460 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_ecommerce_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6518 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/sdg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5467 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4957 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/estimate_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12033 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_order_line_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5184 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/technology_type_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9436 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_shipping_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5926 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4460 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_success_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20183 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_road_shipping_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7177 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_bitcoin_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7397 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/estimate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/order_response.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14253 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_order_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9157 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_hotel_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4065 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/photo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4178 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/parent_technology_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3435 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/place_order_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17526 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_sea_shipping_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8136 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_vehicle_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10989 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_air_shipping_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22501 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7882 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/models/create_ethereum_estimate_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:47:20.000000 patch-api-2.1.1/patch_api/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18654 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    50874 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/orders_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9461 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/technology_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)   124704 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/estimates_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29947 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api/order_line_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14803 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3707 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12988 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25703 2023-04-18 21:46:07.000000 patch-api-2.1.1/patch_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1031 2023-04-18 21:46:07.000000 patch-api-2.1.1/setup.py
```

### Comparing `patch-api-2.1.0/patch_api/configuration.py` & `patch-api-2.1.1/patch_api/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,15 +337,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: 2\n"
-            "SDK Package Version: 2.1.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 2.1.1".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `patch-api-2.1.0/patch_api/api_client.py` & `patch-api-2.1.1/patch_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
         self.rest_client = rest.RESTClientObject(api_key, configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "patch-python/2.1.0"
+        self.user_agent = "patch-python/2.1.1"
         # Set default Patch-Version
         self.patch_version = 2
 
     def __del__(self):
         if self._pool:
             self._pool.close()
             self._pool.join()
```

### Comparing `patch-api-2.1.0/patch_api/exceptions.py` & `patch-api-2.1.1/patch_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/order_response.py` & `patch-api-2.1.1/patch_api/models/order_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_air_shipping_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_air_shipping_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/update_order_line_item_request.py` & `patch-api-2.1.1/patch_api/models/update_order_line_item_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_road_shipping_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_road_shipping_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/place_order_request.py` & `patch-api-2.1.1/patch_api/models/place_order_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/delete_order_response.py` & `patch-api-2.1.1/patch_api/models/delete_order_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/photo.py` & `patch-api-2.1.1/patch_api/models/photo.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_flight_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_flight_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_ethereum_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_ethereum_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/highlight.py` & `patch-api-2.1.1/patch_api/models/highlight.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/order_list_response.py` & `patch-api-2.1.1/patch_api/models/order_list_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_success_response.py` & `patch-api-2.1.1/patch_api/models/create_success_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_shipping_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_shipping_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_bitcoin_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_bitcoin_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/technology_type.py` & `patch-api-2.1.1/patch_api/models/technology_type.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/error_response.py` & `patch-api-2.1.1/patch_api/models/error_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_ecommerce_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_ecommerce_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_order_request.py` & `patch-api-2.1.1/patch_api/models/create_order_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/meta_index_object.py` & `patch-api-2.1.1/patch_api/models/meta_index_object.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_hotel_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_hotel_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_order_line_item_request.py` & `patch-api-2.1.1/patch_api/models/create_order_line_item_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/order_issued_to.py` & `patch-api-2.1.1/patch_api/models/order_issued_to.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/order_line_item_response.py` & `patch-api-2.1.1/patch_api/models/order_line_item_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/estimate_response.py` & `patch-api-2.1.1/patch_api/models/estimate_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/project.py` & `patch-api-2.1.1/patch_api/models/project.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,116 +37,128 @@
         "id": "str",
         "production": "bool",
         "name": "str",
         "description": "str",
         "mechanism": "str",
         "country": "str",
         "state": "str",
+        "issuance_type": "str",
         "latitude": "float",
         "longitude": "float",
         "project_partner": "str",
         "photos": "list[Photo]",
         "verifier": "str",
         "standard": "Standard",
         "sdgs": "list[Sdg]",
         "tagline": "str",
         "technology_type": "TechnologyType",
         "highlights": "list[Highlight]",
         "inventory": "list[Inventory]",
+        "disclaimers": "list[Disclaimer]",
     }
 
     attribute_map = {
         "id": "id",
         "production": "production",
         "name": "name",
         "description": "description",
         "mechanism": "mechanism",
         "country": "country",
         "state": "state",
+        "issuance_type": "issuance_type",
         "latitude": "latitude",
         "longitude": "longitude",
         "project_partner": "project_partner",
         "photos": "photos",
         "verifier": "verifier",
         "standard": "standard",
         "sdgs": "sdgs",
         "tagline": "tagline",
         "technology_type": "technology_type",
         "highlights": "highlights",
         "inventory": "inventory",
+        "disclaimers": "disclaimers",
     }
 
     def __init__(
         self,
         id=None,
         production=None,
         name=None,
         description=None,
         mechanism=None,
         country=None,
         state=None,
+        issuance_type=None,
         latitude=None,
         longitude=None,
         project_partner=None,
         photos=None,
         verifier=None,
         standard=None,
         sdgs=None,
         tagline=None,
         technology_type=None,
         highlights=None,
         inventory=None,
+        disclaimers=None,
         local_vars_configuration=None,
     ):  # noqa: E501
         """Project - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
 
         self._id = None
         self._production = None
         self._name = None
         self._description = None
         self._mechanism = None
         self._country = None
         self._state = None
+        self._issuance_type = None
         self._latitude = None
         self._longitude = None
         self._project_partner = None
         self._photos = None
         self._verifier = None
         self._standard = None
         self._sdgs = None
         self._tagline = None
         self._technology_type = None
         self._highlights = None
         self._inventory = None
+        self._disclaimers = None
         self.discriminator = None
 
         self.id = id
         self.production = production
         self.name = name
         self.description = description
         if mechanism is not None:
             self.mechanism = mechanism
         self.country = country
         self.state = state
+        if issuance_type is not None:
+            self.issuance_type = issuance_type
         self.latitude = latitude
         self.longitude = longitude
         self.project_partner = project_partner
         self.photos = photos
         if verifier is not None:
             self.verifier = verifier
         self.standard = standard
         self.sdgs = sdgs
         if tagline is not None:
             self.tagline = tagline
         self.technology_type = technology_type
         self.highlights = highlights
         self.inventory = inventory
+        if disclaimers is not None:
+            self.disclaimers = disclaimers
 
     @property
     def id(self):
         """Gets the id of this Project.  # noqa: E501
 
         A unique uid for the record. UIDs will be prepended by pro_prod or pro_test depending on the mode it was created in.  # noqa: E501
 
@@ -330,14 +342,47 @@
         :param state: The state of this Project.  # noqa: E501
         :type: str
         """
 
         self._state = state
 
     @property
+    def issuance_type(self):
+        """Gets the issuance_type of this Project.  # noqa: E501
+
+        The issuance type of the project. One of: ex-ante, ex-post.  # noqa: E501
+
+        :return: The issuance_type of this Project.  # noqa: E501
+        :rtype: str
+        """
+        return self._issuance_type
+
+    @issuance_type.setter
+    def issuance_type(self, issuance_type):
+        """Sets the issuance_type of this Project.
+
+        The issuance type of the project. One of: ex-ante, ex-post.  # noqa: E501
+
+        :param issuance_type: The issuance_type of this Project.  # noqa: E501
+        :type: str
+        """
+        allowed_values = ["ex-ante", "ex-post"]  # noqa: E501
+        if (
+            self.local_vars_configuration.client_side_validation
+            and issuance_type not in allowed_values
+        ):  # noqa: E501
+            raise ValueError(
+                "Invalid value for `issuance_type` ({0}), must be one of {1}".format(  # noqa: E501
+                    issuance_type, allowed_values
+                )
+            )
+
+        self._issuance_type = issuance_type
+
+    @property
     def latitude(self):
         """Gets the latitude of this Project.  # noqa: E501
 
         The latitude at which this project is located.  # noqa: E501
 
         :return: The latitude of this Project.  # noqa: E501
         :rtype: float
@@ -606,14 +651,37 @@
         ):  # noqa: E501
             raise ValueError(
                 "Invalid value for `inventory`, must not be `None`"
             )  # noqa: E501
 
         self._inventory = inventory
 
+    @property
+    def disclaimers(self):
+        """Gets the disclaimers of this Project.  # noqa: E501
+
+        An array of objects containing disclaimers about the project. Information, warnings, and critical concerns may be present.  # noqa: E501
+
+        :return: The disclaimers of this Project.  # noqa: E501
+        :rtype: list[Disclaimer]
+        """
+        return self._disclaimers
+
+    @disclaimers.setter
+    def disclaimers(self, disclaimers):
+        """Sets the disclaimers of this Project.
+
+        An array of objects containing disclaimers about the project. Information, warnings, and critical concerns may be present.  # noqa: E501
+
+        :param disclaimers: The disclaimers of this Project.  # noqa: E501
+        :type: list[Disclaimer]
+        """
+
+        self._disclaimers = disclaimers
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.openapi_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `patch-api-2.1.0/patch_api/models/order_line_item_project.py` & `patch-api-2.1.1/patch_api/models/order_line_item_project.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/parent_technology_type.py` & `patch-api-2.1.1/patch_api/models/parent_technology_type.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/project_response.py` & `patch-api-2.1.1/patch_api/models/project_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/__init__.py` & `patch-api-2.1.1/patch_api/models/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     CreateShippingEstimateRequest,
 )
 from patch_api.models.create_success_response import CreateSuccessResponse
 from patch_api.models.create_vehicle_estimate_request import (
     CreateVehicleEstimateRequest,
 )
 from patch_api.models.delete_order_response import DeleteOrderResponse
+from patch_api.models.disclaimer import Disclaimer
 from patch_api.models.error_response import ErrorResponse
 from patch_api.models.estimate import Estimate
 from patch_api.models.estimate_list_response import EstimateListResponse
 from patch_api.models.estimate_response import EstimateResponse
 from patch_api.models.highlight import Highlight
 from patch_api.models.inventory import Inventory
 from patch_api.models.meta_index_object import MetaIndexObject
```

### Comparing `patch-api-2.1.0/patch_api/models/estimate_list_response.py` & `patch-api-2.1.1/patch_api/models/estimate_list_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/inventory.py` & `patch-api-2.1.1/patch_api/models/inventory.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_rail_shipping_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_rail_shipping_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/order.py` & `patch-api-2.1.1/patch_api/models/order.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,26 +406,26 @@
 
         self._currency = currency
 
     @property
     def registry_url(self):
         """Gets the registry_url of this Order.  # noqa: E501
 
-        The url of this order in the public registry.  # noqa: E501
+        The URL of this order in the public registry. Use this URL to access the order's accompanying certificate.  # noqa: E501
 
         :return: The registry_url of this Order.  # noqa: E501
         :rtype: str
         """
         return self._registry_url
 
     @registry_url.setter
     def registry_url(self, registry_url):
         """Sets the registry_url of this Order.
 
-        The url of this order in the public registry.  # noqa: E501
+        The URL of this order in the public registry. Use this URL to access the order's accompanying certificate.  # noqa: E501
 
         :param registry_url: The registry_url of this Order.  # noqa: E501
         :type: str
         """
 
         self._registry_url = registry_url
```

### Comparing `patch-api-2.1.0/patch_api/models/order_line_item.py` & `patch-api-2.1.1/patch_api/models/order_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,26 +179,26 @@
 
         self._vintage_year = vintage_year
 
     @property
     def vintage_start_year(self):
         """Gets the vintage_start_year of this OrderLineItem.  # noqa: E501
 
-        The starting_year in which the climate impacts of the project occurred, or will occur.  # noqa: E501
+        The starting year in which the climate impacts of the project occurred, or will occur.  # noqa: E501
 
         :return: The vintage_start_year of this OrderLineItem.  # noqa: E501
         :rtype: int
         """
         return self._vintage_start_year
 
     @vintage_start_year.setter
     def vintage_start_year(self, vintage_start_year):
         """Sets the vintage_start_year of this OrderLineItem.
 
-        The starting_year in which the climate impacts of the project occurred, or will occur.  # noqa: E501
+        The starting year in which the climate impacts of the project occurred, or will occur.  # noqa: E501
 
         :param vintage_start_year: The vintage_start_year of this OrderLineItem.  # noqa: E501
         :type: int
         """
         if (
             self.local_vars_configuration.client_side_validation
             and vintage_start_year is None
```

### Comparing `patch-api-2.1.0/patch_api/models/create_mass_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_mass_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/estimate.py` & `patch-api-2.1.1/patch_api/models/estimate.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_vehicle_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_vehicle_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/project_list_response.py` & `patch-api-2.1.1/patch_api/models/project_list_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/sdg.py` & `patch-api-2.1.1/patch_api/models/sdg.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/technology_type_list_response.py` & `patch-api-2.1.1/patch_api/models/technology_type_list_response.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/create_sea_shipping_estimate_request.py` & `patch-api-2.1.1/patch_api/models/create_sea_shipping_estimate_request.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/models/standard.py` & `patch-api-2.1.1/patch_api/models/standard.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/rest.py` & `patch-api-2.1.1/patch_api/rest.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/__init__.py` & `patch-api-2.1.1/patch_api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: engineering@usepatch.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 # import ApiClient
 from patch_api.api_client import ApiClient
 from patch_api.configuration import Configuration
 from patch_api.exceptions import OpenApiException
 from patch_api.exceptions import ApiTypeError
 from patch_api.exceptions import ApiValueError
```

### Comparing `patch-api-2.1.0/patch_api/api/estimates_api.py` & `patch-api-2.1.1/patch_api/api/estimates_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/api/orders_api.py` & `patch-api-2.1.1/patch_api/api/orders_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/api/technology_types_api.py` & `patch-api-2.1.1/patch_api/api/technology_types_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/api/projects_api.py` & `patch-api-2.1.1/patch_api/api/projects_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api/api/order_line_items_api.py` & `patch-api-2.1.1/patch_api/api/order_line_items_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/README.md` & `patch-api-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/patch_api.egg-info/SOURCES.txt` & `patch-api-2.1.1/patch_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 patch_api/models/create_rail_shipping_estimate_request.py
 patch_api/models/create_road_shipping_estimate_request.py
 patch_api/models/create_sea_shipping_estimate_request.py
 patch_api/models/create_shipping_estimate_request.py
 patch_api/models/create_success_response.py
 patch_api/models/create_vehicle_estimate_request.py
 patch_api/models/delete_order_response.py
+patch_api/models/disclaimer.py
 patch_api/models/error_response.py
 patch_api/models/estimate.py
 patch_api/models/estimate_list_response.py
 patch_api/models/estimate_response.py
 patch_api/models/highlight.py
 patch_api/models/inventory.py
 patch_api/models/meta_index_object.py
```

### Comparing `patch-api-2.1.0/test/test_orders_api.py` & `patch-api-2.1.1/test/test_orders_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/test/test_estimates_api.py` & `patch-api-2.1.1/test/test_estimates_api.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/test/test_projects_api.py` & `patch-api-2.1.1/test/test_projects_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -62,14 +62,25 @@
         self.assertTrue(isinstance(inventory[0].vintage_start_year, int))
         self.assertTrue(isinstance(inventory[0].vintage_end_year, int))
         self.assertTrue(isinstance(inventory[0].amount_available, int))
         self.assertTrue(isinstance(inventory[0].price, int))
         self.assertTrue(isinstance(inventory[0].currency, str))
         self.assertTrue(isinstance(inventory[0].unit, str))
 
+        issuance_type = project.issuance_type
+        self.assertTrue(isinstance(issuance_type, str))
+
+        disclaimers = project.disclaimers
+        self.assertTrue(isinstance(disclaimers, list))
+        self.assertTrue(isinstance(disclaimers[0].header, str))
+        self.assertTrue(isinstance(disclaimers[0].body, str))
+        self.assertTrue(isinstance(disclaimers[0].severity, str))
+        self.assertTrue(isinstance(disclaimers[0].link_text, str))
+        self.assertTrue(isinstance(disclaimers[0].link_destination, str))
+
     def test_retrieve_project_language(self):
         """Test case for retrieve_project
 
         Retrieves a project  # noqa: E501
         """
         project_id = "pro_test_2b67b11a030b66e0a6dd61a56b49079a"
         project = self.api.retrieve_project(id=project_id, accept_language="fr").data
```

### Comparing `patch-api-2.1.0/test/test_rest.py` & `patch-api-2.1.1/test/test_rest.py`

 * *Files identical despite different names*

### Comparing `patch-api-2.1.0/setup.py` & `patch-api-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "patch-api"
-VERSION = "2.1.0"
+VERSION = "2.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

