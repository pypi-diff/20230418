# Comparing `tmp/mindee-3.6.0.tar.gz` & `tmp/mindee-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.6.0.tar", last modified: Fri Mar 10 19:27:45 2023, max compression
+gzip compressed data, was "mindee-3.7.0.tar", last modified: Tue Apr 18 16:25:36 2023, max compression
```

## Comparing `mindee-3.6.0.tar` & `mindee-3.7.0.tar`

### file list

```diff
@@ -1,141 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.584955 mindee-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-10 19:27:22.000000 mindee-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-10 19:27:45.584955 mindee-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-10 19:27:22.000000 mindee-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/custom/custom_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/receipt/receipt_v4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.576955 mindee-3.6.0/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.580955 mindee-3.6.0/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.580955 mindee-3.6.0/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.580955 mindee-3.6.0/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/api_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.580955 mindee-3.6.0/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-10 19:27:22.000000 mindee-3.6.0/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.572955 mindee-3.6.0/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 19:27:27.000000 mindee-3.6.0/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-10 19:27:45.000000 mindee-3.6.0/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-10 19:27:22.000000 mindee-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-03-10 19:27:45.588955 mindee-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-10 19:27:22.000000 mindee-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.580955 mindee-3.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.584955 mindee-3.6.0/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.584955 mindee-3.6.0/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.584955 mindee-3.6.0/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:45.584955 mindee-3.6.0/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_pkg_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-03-10 19:27:22.000000 mindee-3.6.0/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.375078 mindee-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-18 16:25:16.000000 mindee-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-18 16:25:36.375078 mindee-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-18 16:25:16.000000 mindee-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.343078 mindee-3.7.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/custom/custom_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/financial/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.351078 mindee-3.7.0/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/line_item_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.355078 mindee-3.7.0/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/line_item_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/receipt/receipt_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.359078 mindee-3.7.0/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.363078 mindee-3.7.0/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/api_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.363078 mindee-3.7.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 16:25:16.000000 mindee-3.7.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.347078 mindee-3.7.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:25:20.000000 mindee-3.7.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 16:25:36.000000 mindee-3.7.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-18 16:25:16.000000 mindee-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-18 16:25:36.375078 mindee-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 16:25:16.000000 mindee-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.367078 mindee-3.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11186 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.371078 mindee-3.7.0/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:36.375078 mindee-3.7.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_pkg_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-18 16:25:16.000000 mindee-3.7.0/tests/test_response.py
```

### Comparing `mindee-3.6.0/LICENSE` & `mindee-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/PKG-INFO` & `mindee-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.6.0
+Version: 3.7.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
@@ -111,15 +111,15 @@
 * [Getting started](https://developers.mindee.com/docs/getting-started)
 * [Command Line Interface (CLI)](https://developers.mindee.com/docs/python-cli)
 * [Custom APIs (API Builder)](https://developers.mindee.com/docs/python-api-builder)
 * [Invoice API](https://developers.mindee.com/docs/python-invoice-ocr)
 * [Passport API](https://developers.mindee.com/docs/python-passport-ocr)
 * [Receipt API](https://developers.mindee.com/docs/python-receipt-ocr)
 
-You can view the source code on [GitHub](https://github.com/mindee/mindee-api-nodejs).
+You can view the source code on [GitHub](https://github.com/mindee/mindee-api-python).
 
 You can also take a look at the
 **[Reference Documentation](https://mindee.github.io/mindee-api-python/)**.
 
 ## License
 Copyright © Mindee
```

### Comparing `mindee-3.6.0/README.md` & `mindee-3.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 * [Getting started](https://developers.mindee.com/docs/getting-started)
 * [Command Line Interface (CLI)](https://developers.mindee.com/docs/python-cli)
 * [Custom APIs (API Builder)](https://developers.mindee.com/docs/python-api-builder)
 * [Invoice API](https://developers.mindee.com/docs/python-invoice-ocr)
 * [Passport API](https://developers.mindee.com/docs/python-passport-ocr)
 * [Receipt API](https://developers.mindee.com/docs/python-receipt-ocr)
 
-You can view the source code on [GitHub](https://github.com/mindee/mindee-api-nodejs).
+You can view the source code on [GitHub](https://github.com/mindee/mindee-api-python).
 
 You can also take a look at the
 **[Reference Documentation](https://mindee.github.io/mindee-api-python/)**.
 
 ## License
 Copyright © Mindee
```

### Comparing `mindee-3.6.0/mindee/cli.py` & `mindee-3.7.0/mindee/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     ),
     "invoice": CommandConfig(
         help="Invoice",
         doc_class=documents.TypeInvoiceV4,
     ),
     "receipt": CommandConfig(
         help="Expense Receipt",
-        doc_class=documents.TypeReceiptV4,
+        doc_class=documents.TypeReceiptV5,
     ),
     "passport": CommandConfig(
         help="Passport",
         doc_class=documents.TypePassportV1,
     ),
     "financial-document": CommandConfig(
         help="Financial Document (receipt or invoice)",
```

### Comparing `mindee-3.6.0/mindee/client.py` & `mindee-3.7.0/mindee/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,19 @@
             ),
             ConfigSpec(
                 doc_class=documents.ReceiptV4,
                 url_name="expense_receipts",
                 version="4",
             ),
             ConfigSpec(
+                doc_class=documents.ReceiptV5,
+                url_name="expense_receipts",
+                version="5",
+            ),
+            ConfigSpec(
                 doc_class=documents.FinancialDocumentV1,
                 url_name="financial_document",
                 version="1",
             ),
             ConfigSpec(
                 doc_class=documents.PassportV1,
                 url_name="passport",
```

### Comparing `mindee-3.6.0/mindee/documents/__init__.py` & `mindee-3.7.0/mindee/documents/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,12 +7,19 @@
     FinancialV1,
     TypeFinancialDocumentV1,
     TypeFinancialV1,
 )
 from mindee.documents.invoice import InvoiceV3, InvoiceV4, TypeInvoiceV3, TypeInvoiceV4
 from mindee.documents.passport import PassportV1, TypePassportV1
 from mindee.documents.proof_of_address import ProofOfAddressV1, TypeProofOfAddressV1
-from mindee.documents.receipt import ReceiptV3, ReceiptV4, TypeReceiptV3, TypeReceiptV4
+from mindee.documents.receipt import (
+    ReceiptV3,
+    ReceiptV4,
+    ReceiptV5,
+    TypeReceiptV3,
+    TypeReceiptV4,
+    TypeReceiptV5,
+)
 from mindee.documents.shipping_container import (
     ShippingContainerV1,
     TypeShippingContainerV1,
 )
```

### Comparing `mindee-3.6.0/mindee/documents/base.py` & `mindee-3.7.0/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/config.py` & `mindee-3.7.0/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/cropper/cropper_v1.py` & `mindee-3.7.0/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/custom/custom_v1.py` & `mindee-3.7.0/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.7.0/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/financial/financial_document_v1.py` & `mindee-3.7.0/mindee/documents/financial/financial_document_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
-from mindee.documents.invoice.line_item import InvoiceLineItem
+from mindee.documents.invoice.line_item_v4 import InvoiceLineItemV4
 from mindee.fields.amount import AmountField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
@@ -40,15 +40,15 @@
     """Customer's name"""
     customer_address: TextField
     """Customer's address"""
     customer_company_registrations: List[CompanyRegistrationField]
     """Customer company registration numbers"""
     supplier_payment_details: List[PaymentDetails]
     """Payment details"""
-    line_items: List[InvoiceLineItem]
+    line_items: List[InvoiceLineItemV4]
     """Details of line items"""
     tip: AmountField
     """Total amount of tip and gratuity."""
     time: TextField
     """Time as seen on the receipt in HH:MM format."""
     document_type: TextField
     """A classification field, among predefined classes."""
@@ -122,15 +122,15 @@
             for tax_prediction in api_prediction["taxes"]
         ]
         self.supplier_payment_details = [
             PaymentDetails(payment_detail, page_n=page_n)
             for payment_detail in api_prediction["supplier_payment_details"]
         ]
         self.line_items = [
-            InvoiceLineItem(prediction=line_item, page_n=page_n)
+            InvoiceLineItemV4(prediction=line_item, page_n=page_n)
             for line_item in api_prediction["line_items"]
         ]
         self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
         self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
         self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
         self.tip = AmountField(api_prediction["tip"], page_n=page_n)
         self.time = TextField(api_prediction["time"], page_n=page_n)
```

### Comparing `mindee-3.6.0/mindee/documents/financial/financial_v1.py` & `mindee-3.7.0/mindee/documents/financial/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.7.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.7.0/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.7.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.7.0/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/invoice/checks.py` & `mindee-3.7.0/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/invoice/invoice_v3.py` & `mindee-3.7.0/mindee/documents/invoice/invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/invoice/invoice_v4.py` & `mindee-3.7.0/mindee/documents/invoice/invoice_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.documents.invoice import checks, reconstruct
-from mindee.documents.invoice.line_item import InvoiceLineItem
+from mindee.documents.invoice.line_item_v4 import InvoiceLineItemV4
 from mindee.fields.amount import AmountField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
 from mindee.fields.tax import TaxField
 from mindee.fields.text import TextField
@@ -41,15 +41,15 @@
     """Customer's name"""
     customer_address: TextField
     """Customer's address"""
     customer_company_registrations: List[CompanyRegistrationField]
     """Customer company registration numbers"""
     supplier_payment_details: List[PaymentDetails]
     """Payment details"""
-    line_items: List[InvoiceLineItem]
+    line_items: List[InvoiceLineItemV4]
     """Details of line items"""
 
     def __init__(
         self,
         api_prediction=None,
         input_source=None,
         page_n: Optional[int] = None,
@@ -112,15 +112,15 @@
             for tax_prediction in api_prediction["taxes"]
         ]
         self.supplier_payment_details = [
             PaymentDetails(payment_detail, page_n=page_n)
             for payment_detail in api_prediction["supplier_payment_details"]
         ]
         self.line_items = [
-            InvoiceLineItem(prediction=line_item, page_n=page_n)
+            InvoiceLineItemV4(prediction=line_item, page_n=page_n)
             for line_item in api_prediction["line_items"]
         ]
         self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
         self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
         self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_n=page_n)
 
     def __str__(self) -> str:
```

### Comparing `mindee-3.6.0/mindee/documents/invoice/line_item.py` & `mindee-3.7.0/mindee/documents/invoice/line_item_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Optional
 
 from mindee.fields.base import FieldPositionMixin, TypePrediction, float_to_string
 
 
-class InvoiceLineItem(FieldPositionMixin):
+class InvoiceLineItemV4(FieldPositionMixin):
     product_code: Optional[str]
     """The product code referring to the item."""
     description: Optional[str]
     """The item description."""
     quantity: Optional[float]
     """The item quantity"""
     unit_price: Optional[float]
```

### Comparing `mindee-3.6.0/mindee/documents/invoice/reconstruct.py` & `mindee-3.7.0/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/passport/passport_v1.py` & `mindee-3.7.0/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.7.0/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/receipt/receipt_v3.py` & `mindee-3.7.0/mindee/documents/receipt/receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/receipt/receipt_v4.py` & `mindee-3.7.0/mindee/documents/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.7.0/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.7.0/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/endpoints.py` & `mindee-3.7.0/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/amount.py` & `mindee-3.7.0/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/api_builder.py` & `mindee-3.7.0/mindee/fields/api_builder.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/base.py` & `mindee-3.7.0/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/company_registration.py` & `mindee-3.7.0/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/date.py` & `mindee-3.7.0/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/locale.py` & `mindee-3.7.0/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/orientation.py` & `mindee-3.7.0/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/payment_details.py` & `mindee-3.7.0/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/position.py` & `mindee-3.7.0/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/tax.py` & `mindee-3.7.0/mindee/fields/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/fields/text.py` & `mindee-3.7.0/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/geometry.py` & `mindee-3.7.0/mindee/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,18 +154,18 @@
 def get_centroid(points: Points) -> Point:
     """
     Get the central point (centroid) given a sequence of points.
 
     :param points: Polygon to process.
     :return: The centroid
     """
-    numb_vertices = len(points)
+    vertices_count = len(points)
     x_sum = sum(x for x, _ in points)
     y_sum = sum(y for _, y in points)
-    return Point(x_sum / numb_vertices, y_sum / numb_vertices)
+    return Point(x_sum / vertices_count, y_sum / vertices_count)
 
 
 def get_min_max_y(points: Points) -> MinMax:
     """
     Get the maximum and minimum Y value given a sequence of points.
 
     :param points: List of points
```

### Comparing `mindee-3.6.0/mindee/input/page_options.py` & `mindee-3.7.0/mindee/input/page_options.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import NamedTuple, Sequence
 
 KEEP_ONLY = "KEEP_ONLY"
 REMOVE = "REMOVE"
 
 
 class PageOptions(NamedTuple):
+    """Options to pass to the `parse` method for cutting multipage documents."""
+
     page_indexes: Sequence[int]
     """
     Zero-based list of page indexes.
     A negative index can be used, indicating an offset from the end of the document.
 
     `[0, -1]` represents the fist and last pages of the document.
     """
```

### Comparing `mindee-3.6.0/mindee/input/sources.py` & `mindee-3.7.0/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/response.py` & `mindee-3.7.0/mindee/response.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee/versions.py` & `mindee-3.7.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/mindee.egg-info/PKG-INFO` & `mindee-3.7.0/mindee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.6.0
+Version: 3.7.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
@@ -111,15 +111,15 @@
 * [Getting started](https://developers.mindee.com/docs/getting-started)
 * [Command Line Interface (CLI)](https://developers.mindee.com/docs/python-cli)
 * [Custom APIs (API Builder)](https://developers.mindee.com/docs/python-api-builder)
 * [Invoice API](https://developers.mindee.com/docs/python-invoice-ocr)
 * [Passport API](https://developers.mindee.com/docs/python-passport-ocr)
 * [Receipt API](https://developers.mindee.com/docs/python-receipt-ocr)
 
-You can view the source code on [GitHub](https://github.com/mindee/mindee-api-nodejs).
+You can view the source code on [GitHub](https://github.com/mindee/mindee-api-python).
 
 You can also take a look at the
 **[Reference Documentation](https://mindee.github.io/mindee-api-python/)**.
 
 ## License
 Copyright © Mindee
```

### Comparing `mindee-3.6.0/mindee.egg-info/SOURCES.txt` & `mindee-3.7.0/mindee.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -43,23 +43,25 @@
 mindee/documents/fr/carte_vitale/carte_vitale_v1.py
 mindee/documents/fr/id_card/__init__.py
 mindee/documents/fr/id_card/id_card_v1.py
 mindee/documents/invoice/__init__.py
 mindee/documents/invoice/checks.py
 mindee/documents/invoice/invoice_v3.py
 mindee/documents/invoice/invoice_v4.py
-mindee/documents/invoice/line_item.py
+mindee/documents/invoice/line_item_v4.py
 mindee/documents/invoice/reconstruct.py
 mindee/documents/passport/__init__.py
 mindee/documents/passport/passport_v1.py
 mindee/documents/proof_of_address/__init__.py
 mindee/documents/proof_of_address/proof_of_address_v1.py
 mindee/documents/receipt/__init__.py
+mindee/documents/receipt/line_item_v5.py
 mindee/documents/receipt/receipt_v3.py
 mindee/documents/receipt/receipt_v4.py
+mindee/documents/receipt/receipt_v5.py
 mindee/documents/shipping_container/__init__.py
 mindee/documents/shipping_container/shipping_container_v1.py
 mindee/documents/us/__init__.py
 mindee/documents/us/bank_check/__init__.py
 mindee/documents/us/bank_check/bank_check_v1.py
 mindee/fields/__init__.py
 mindee/fields/amount.py
@@ -89,14 +91,15 @@
 tests/documents/test_financial_v1.py
 tests/documents/test_invoice_v3.py
 tests/documents/test_invoice_v4.py
 tests/documents/test_passport_v1.py
 tests/documents/test_proof_of_address_v1.py
 tests/documents/test_receipt_v3.py
 tests/documents/test_receipt_v4.py
+tests/documents/test_receipt_v5.py
 tests/documents/test_shipping_container_v1.py
 tests/documents/fr/__init__.py
 tests/documents/fr/test_bank_account_details_v1.py
 tests/documents/fr/test_carte_grise_v1.py
 tests/documents/fr/test_carte_vitale_v1.py
 tests/documents/fr/test_id_card_v1.py
 tests/documents/us/__init__.py
```

### Comparing `mindee-3.6.0/pyproject.toml` & `mindee-3.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/setup.cfg` & `mindee-3.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 mindee = 
 	version
 	py.typed
 
 [options.extras_require]
 dev = 
 	black==23.1.0
-	mypy==1.0.0
-	pip-tools~=6.12.2
-	pylint==2.16.1
+	mypy==1.0.1
+	pip-tools~=6.12.3
+	pylint==2.17.1
 	setuptools==51.3.3
 	isort==5.11.5
 	pre-commit~=2.21.0
 	pydocstyle==6.3.0
 test = 
 	pytest~=7.1
 	pytest-cov~=4.0
```

### Comparing `mindee-3.6.0/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.7.0/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.7.0/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.7.0/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/fr/test_id_card_v1.py` & `mindee-3.7.0/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_cropper_v1.py` & `mindee-3.7.0/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_custom_v1.py` & `mindee-3.7.0/tests/documents/test_custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_financial_document_v1.py` & `mindee-3.7.0/tests/documents/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_financial_v1.py` & `mindee-3.7.0/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_invoice_v3.py` & `mindee-3.7.0/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_invoice_v4.py` & `mindee-3.7.0/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_passport_v1.py` & `mindee-3.7.0/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_proof_of_address_v1.py` & `mindee-3.7.0/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_receipt_v3.py` & `mindee-3.7.0/tests/documents/test_receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_receipt_v4.py` & `mindee-3.7.0/tests/documents/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/test_shipping_container_v1.py` & `mindee-3.7.0/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/documents/us/test_bank_check_v1.py` & `mindee-3.7.0/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_amount.py` & `mindee-3.7.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_date.py` & `mindee-3.7.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_field.py` & `mindee-3.7.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_locale.py` & `mindee-3.7.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_orientation.py` & `mindee-3.7.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_payment_details.py` & `mindee-3.7.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_position.py` & `mindee-3.7.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/fields/test_tax.py` & `mindee-3.7.0/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_cli.py` & `mindee-3.7.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_client.py` & `mindee-3.7.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_geometry.py` & `mindee-3.7.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_inputs.py` & `mindee-3.7.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_pkg_versions.py` & `mindee-3.7.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.6.0/tests/test_response.py` & `mindee-3.7.0/tests/test_response.py`

 * *Files identical despite different names*

