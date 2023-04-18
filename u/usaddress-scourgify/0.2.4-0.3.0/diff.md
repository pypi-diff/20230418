# Comparing `tmp/usaddress-scourgify-0.2.4.tar.gz` & `tmp/usaddress-scourgify-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/usaddress-scourgify-0.2.4.tar", last modified: Mon Jun 22 20:00:07 2020, max compression
+gzip compressed data, was "/home/fable/CodeProjects/GBR/usaddress-scourgify/dist/tmpx4fit9ef/usaddress-scourgify-0.3.0.tar", last modified: Tue Apr 18 17:00:11 2023, max compression
```

## Comparing `usaddress-scourgify-0.2.4.tar` & `usaddress-scourgify-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/
--rwxrwxrwx   0 fable     (1000) fable     (1000)      792 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/PKG-INFO
--rwxrwxrwx   0 fable     (1000) fable     (1000)     4811 2020-05-06 18:02:40.000000 usaddress-scourgify-0.2.4/README.rst
-drwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/scourgify/
--rwxrwxrwx   0 fable     (1000) fable     (1000)    15587 2019-11-14 19:18:38.000000 usaddress-scourgify-0.2.4/scourgify/address_constants.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)     8690 2020-05-06 22:54:49.000000 usaddress-scourgify-0.2.4/scourgify/cleaning.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)     1789 2019-11-14 19:18:38.000000 usaddress-scourgify-0.2.4/scourgify/exceptions.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)    26239 2020-05-14 22:04:38.000000 usaddress-scourgify-0.2.4/scourgify/normalize.py
-drwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/scourgify/tests/
-drwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/scourgify/tests/config/
--rwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-05-06 23:07:32.000000 usaddress-scourgify-0.2.4/scourgify/tests/config/__init__.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)    25633 2020-05-14 22:03:25.000000 usaddress-scourgify-0.2.4/scourgify/tests/test_address_normalization.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)     1093 2019-11-14 19:18:38.000000 usaddress-scourgify-0.2.4/scourgify/tests/test_cleaning.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)        0 2019-02-01 18:36:25.000000 usaddress-scourgify-0.2.4/scourgify/tests/__init__.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)     4110 2019-11-14 19:18:38.000000 usaddress-scourgify-0.2.4/scourgify/validations.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)      222 2019-02-01 18:36:25.000000 usaddress-scourgify-0.2.4/scourgify/__init__.py
--rwxrwxrwx   0 fable     (1000) fable     (1000)      935 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/setup.cfg
--rwxrwxrwx   0 fable     (1000) fable     (1000)       62 2019-02-01 18:36:25.000000 usaddress-scourgify-0.2.4/setup.py
-drwxrwxrwx   0 fable     (1000) fable     (1000)        0 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/
--rwxrwxrwx   0 fable     (1000) fable     (1000)        1 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/dependency_links.txt
--rwxrwxrwx   0 fable     (1000) fable     (1000)        1 2020-05-06 23:11:19.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/not-zip-safe
--rwxrwxrwx   0 fable     (1000) fable     (1000)      792 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/PKG-INFO
--rwxrwxrwx   0 fable     (1000) fable     (1000)       69 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/requires.txt
--rwxrwxrwx   0 fable     (1000) fable     (1000)      574 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/SOURCES.txt
--rwxrwxrwx   0 fable     (1000) fable     (1000)       10 2020-06-22 20:00:07.000000 usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:59:14.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      582 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/tests/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/test_cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/scourgify/tests/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27406 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/tests/test_address_normalization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4243 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/validations.py
+-rw-r--r--   0 root         (0) root         (0)     8940 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/scourgify/cleaning.py
+-rw-r--r--   0 root         (0) root         (0)    33262 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/normalize.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16206 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/scourgify/address_constants.py
+-rw-r--r--   0 root         (0) root         (0)      918 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       68 2023-04-17 20:22:48.000000 usaddress-scourgify-0.3.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      803 2023-04-18 17:00:11.000000 usaddress-scourgify-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5242 2023-04-18 16:58:50.000000 usaddress-scourgify-0.3.0/README.rst
```

### Comparing `usaddress-scourgify-0.2.4/PKG-INFO` & `usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.2.4
+Version: 0.3.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: usaddress,normalization,address
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `usaddress-scourgify-0.2.4/README.rst` & `usaddress-scourgify-0.3.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,128 @@
-usaddress-scourgify
-===================
-
-A Python3.x library for cleaning/normalizing US addresses following USPS pub 28 and RESO guidelines.
-
-
-
-Documentation
--------------
-Use
-
-``normalize_address_record()``
-
- or
-
-``get_geocoder_normalized_addr()``
-
-to standardize your addresses. (Note: usaddress-scourgify does not make any attempts at address validation.)
-
-Both functions take an address string, or a dict-like object, and return an address dict with all field values in uppercase format mapped to the keys address_line_1, address_line_2, city, state, postal_code... code-block:: python
-
-
-.. code-block:: python
-
-
-        from scourgify import normalize_address_record
-
-        normalize_address_record('123 southwest Main street, Boring, or, 97203')
-        
-        normalize_address_record({
-            'address_line_1': '123 southwest Main street',
-            'address_line_2': 'unit 2,
-            'city': 'Boring',
-            'state': 'or',
-            'postal_code': '97203'
-        })
-
-
-expected output
-
-
-.. code-block:: python
-
-       {
-            'address_line_1': '123 SW MAIN ST',
-            'address_line_2': 'UNIT 2'
-            'city': 'BORING',
-            'state': 'OR',
-            'postal_code': '97203'
-        }
-
-normalized_address_record() uses the included processing functions to remove unacceptable special characters, extra spaces, predictable abnormal character sub-strings and phrases. It also abbreviates directional indicators and street types according to the abbreviation mappings found in address_constants.  If applicable, line 2 address elements (ie: Apt, Unit) are separated from line 1 inputs and standard occupancy type abbreviations are applied.
-
-You may supply additional additional processing functions as a list of callable supplied to the addtl_funcs parameter. Any additional functions should take a string address and return a tuple of strings (line1, line2).
-
-If your address is in the form of a dict that does not use the keys address_line_1, address_line_2, city, state, and postal_code, you must supply a key map to the addr_map parameter in the format {standard_key: custom_key}
-
-
-.. code-block:: python
-
-        {
-            'address_line_1': 'Line1',
-            'address_line_2': 'Line2',
-            'city': 'City',
-            'state': 'State',
-            'postal_code': 'Zip'
-        }
-
-
-You can also customize the address constants used by setting up an `address_constants.yaml` config file.
-Allowed keys are::
-            DIRECTIONAL_REPLACEMENTS
-            OCCUPANCY_TYPE_ABBREVIATIONS
-            STATE_ABBREVIATIONS
-            STREET_TYPE_ABBREVIATIONS
-            KNOWN_ODDITIES
-            PROBLEM_ST_TYPE_ABBRVS
-
-You may also use the key `insertion_method` with a value of `update` or `replace` to indicate where you would like to insert your values into the existing constants or replace them. If `insertion_method` is not present, update is assumed.
-
-
-.. code-block:: yaml
-
-        insertion_method: update
-        KNOWN_ODDITIES:
-            'developed by HOST': ''
-            ', UN ': ' UNIT '
-
-        OCCUPANCY_TYPE_ABBREVIATIONS:
-            'UN': 'UNIT'
-
-
-get_geocoder_normalized_addr() uses geocoder.google to parse your address into a standard dict.  No additional cleaning is performed, so if your address contains any stray or non-conforming elements (ie: 8888 NE KILLINGSWORTH ST, UN C, PORTLAND, OR 97008), no result will be returned.
-Since geocoder accepts an address string, if your address is in dict format you will need to supply a list of the address related keys within your dict, in the order of address string composition, if your keys do not match the standard key set (address_line_1, address_line_2, city, state, postal_code)
-
-Installation
-------------
-Requires Python3.x.
-
-``pip install usaddress-scourgify``
-
-To use a custom constants yaml, set the ADDRESS_CONFIG_DIR environment variable with the full path to the directory containing your address_constants.yaml file
-
-``export ADDRESS_CONFIG_DIR=/path/to/your/config_dir``
-
-To use get_geocoder_normalized_addr, set the GOOGLE_API_KEY environment variable
-
-``export GOOGLE_API_KEY=your_google_api_key``
-
-Contributing
-------------
-Create a new branch to hold your change; no pull requests submitted directly to dev or master will be approved.  Please include a comment explain the issue your pull request solves. Make sure all appropriate test, and tox, updates are included and that all tests are passing.
-
-License
--------
-usaddress-scourgify is released under the terms of the MIT license. Full details in LICENSE file.
-
-Changelog
----------
-usaddress-scourgify was developed for use in the greenbuildingregistry project.
-For a full changelog see `CHANGELOG.rst <https://github.com/GreenBuildingRegistry/usaddress-scourgify/blob/master/CHANGELOG.rst>`_.
+usaddress-scourgify
+===================
+
+A Python3.x library for cleaning/normalizing US addresses following USPS pub 28 and RESO guidelines.
+
+
+
+Documentation
+-------------
+Use
+
+``normalize_address_record()``
+
+ or
+
+``get_geocoder_normalized_addr()``
+
+or
+
+``NormalizeAddress().normalize()``
+
+to standardize your addresses. (Note: usaddress-scourgify does not make any attempts at address validation.)
+
+Both functions, and the class init, take an address string, or a dict-like object, and return an address dict with all field values in uppercase format mapped to the keys address_line_1, address_line_2, city, state, postal_code... code-block:: python
+
+
+.. code-block:: python
+
+
+        from scourgify import normalize_address_record, NormalizeAddress
+
+        normalize_address_record('123 southwest Main street, Boring, or, 97203')
+        
+        normalize_address_record({
+            'address_line_1': '123 southwest Main street',
+            'address_line_2': 'unit 2,
+            'city': 'Boring',
+            'state': 'or',
+            'postal_code': '97203'
+        })
+
+        NormalizeAddress('123 southwest Main street, Boring, or, 97203').normalize()
+
+expected output
+
+
+.. code-block:: python
+
+       {
+            'address_line_1': '123 SW MAIN ST',
+            'address_line_2': 'UNIT 2'
+            'city': 'BORING',
+            'state': 'OR',
+            'postal_code': '97203'
+        }
+
+normalized_address_record() uses the included processing functions to remove unacceptable special characters, extra spaces, predictable abnormal character sub-strings and phrases. It also abbreviates directional indicators and street types according to the abbreviation mappings found in address_constants.  If applicable, line 2 address elements (ie: Apt, Unit) are separated from line 1 inputs and standard occupancy type abbreviations are applied.
+
+You may supply additional additional processing functions as a list of callable supplied to the addtl_funcs parameter. Any additional functions should take a string address and return a tuple of strings (line1, line2).
+
+Alternately, you may extend the `NormalizeAddress` class to customize the normalization behavior by overriding any of the class' methods.
+
+If your address is in the form of a dict that does not use the keys address_line_1, address_line_2, city, state, and postal_code, you must supply a key map to the addr_map parameter in the format {standard_key: custom_key}
+
+
+.. code-block:: python
+
+        {
+            'address_line_1': 'Line1',
+            'address_line_2': 'Line2',
+            'city': 'City',
+            'state': 'State',
+            'postal_code': 'Zip'
+        }
+
+
+You can also customize the address constants used by setting up an `address_constants.yaml` config file.
+Allowed keys are::
+            DIRECTIONAL_REPLACEMENTS
+            OCCUPANCY_TYPE_ABBREVIATIONS
+            STATE_ABBREVIATIONS
+            STREET_TYPE_ABBREVIATIONS
+            KNOWN_ODDITIES
+            PROBLEM_ST_TYPE_ABBRVS
+
+You may also use the key `insertion_method` with a value of `update` or `replace` to indicate where you would like to insert your values into the existing constants or replace them. If `insertion_method` is not present, update is assumed.
+
+
+.. code-block:: yaml
+
+        insertion_method: update
+        KNOWN_ODDITIES:
+            'developed by HOST': ''
+            ', UN ': ' UNIT '
+
+        OCCUPANCY_TYPE_ABBREVIATIONS:
+            'UN': 'UNIT'
+
+
+get_geocoder_normalized_addr() uses geocoder.google to parse your address into a standard dict.  No additional cleaning is performed, so if your address contains any stray or non-conforming elements (ie: 8888 NE KILLINGSWORTH ST, UN C, PORTLAND, OR 97008), no result will be returned.
+Since geocoder accepts an address string, if your address is in dict format you will need to supply a list of the address related keys within your dict, in the order of address string composition, if your keys do not match the standard key set (address_line_1, address_line_2, city, state, postal_code)
+
+Installation
+------------
+Requires Python3.x.
+
+``pip install usaddress-scourgify``
+
+To use a custom constants yaml, set the ADDRESS_CONFIG_DIR environment variable with the full path to the directory containing your address_constants.yaml file
+
+``export ADDRESS_CONFIG_DIR=/path/to/your/config_dir``
+
+To use get_geocoder_normalized_addr, set the GOOGLE_API_KEY environment variable
+
+``export GOOGLE_API_KEY=your_google_api_key``
+
+Contributing
+------------
+Create a new branch to hold your change; no pull requests submitted directly to dev or master will be approved.  Please include a comment explain the issue your pull request solves. Make sure all appropriate test, and tox, updates are included and that all tests are passing.
+
+License
+-------
+usaddress-scourgify is released under the terms of the MIT license. Full details in LICENSE file.
+
+Changelog
+---------
+usaddress-scourgify was developed for use in the greenbuildingregistry project.
+For a full changelog see `CHANGELOG.rst <https://github.com/GreenBuildingRegistry/usaddress-scourgify/blob/master/CHANGELOG.rst>`_.
```

### Comparing `usaddress-scourgify-0.2.4/scourgify/cleaning.py` & `usaddress-scourgify-0.3.0/scourgify/cleaning.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-copyright (c) 2016-2017 Earth Advantage.
-All rights reserved
-..codeauthor::Fable Turas <fable@rainsoftware.tech>
-
-[ INSERT DOC STRING ]  # TODO
-"""
-
-# Imports from Standard Library
-import re
-import unicodedata
-from typing import Any, Optional, Sequence, Union
-
-# Imports from Third Party Modules
-import usaddress
-
-# Local Imports
-from scourgify.address_constants import (
-    KNOWN_ODDITIES,
-    OCCUPANCY_TYPE_ABBREVIATIONS,
-    PROBLEM_ST_TYPE_ABBRVS,
-)
-
-# Setup
-
-# Constants
-# periods (in decimals), hyphens, / , and & are acceptable address components
-# ord('&') ord('#') ord('-'), ord('.') and ord('/')
-ALLOWED_CHARS = [35, 38, 45, 46, 47]
-
-# Don't remove ',', '(' or ')' in PRE_CLEAN
-PRECLEAN_EXCLUDE = [40, 41, 44]
-EXCLUDE_ALL = ALLOWED_CHARS + PRECLEAN_EXCLUDE
-
-STRIP_CHAR_CATS = (
-    'M', 'S', 'C', 'Nl', 'No', 'Pc', 'Ps', 'Pe', 'Pi', 'Pf', 'Po'
-)
-STRIP_PUNC_CATS = ('Z', 'Pd')
-STRIP_ALL_CATS = STRIP_CHAR_CATS + STRIP_PUNC_CATS
-
-# Data Structure Definitions
-
-# Private Functions
-
-
-# Public Classes and Functions
-
-def pre_clean_addr_str(addr_str, state=None):
-    # type: (str, Optional[str]) -> str
-    """Remove any known undesirable sub-strings and special characters.
-
-    Cleaning should be enacted on an addr_str to remove known characters
-    and phrases that might prevent usaddress from successfully parsing.
-    Follows USPS pub 28 guidelines for undesirable special characters.
-    Non-address phrases or character sets known to occur in raw addresses
-    should be added to address_constants.KNOWN_ODDITIES.
-
-    Some characters are left behind to potentially assist in second chance
-    processing of unparseable addresses and should be further cleaned
-    post_processing. (see post_clean_addr_str).
-
-    :param addr_str: raw address string
-    :type addr_str: str
-    :param state: optional string containing normalized state data.
-    :type state: str
-    :return: cleaned string
-    :rtype: str
-    """
-    # replace any easily handled, undesirable sub-strings
-    if any(oddity in addr_str for oddity in KNOWN_ODDITIES.keys()):
-        for key, replacement in KNOWN_ODDITIES.items():      # pragma: no cover
-            addr_str = addr_str.replace(key, replacement)
-
-    # remove non-decimal point period chars.
-    if '.' in addr_str:                                      # pragma: no cover
-        addr_str = clean_period_char(addr_str)
-
-    # remove special characters per USPS pub 28, except & which impacts
-    # intersection addresses, and - which impacts range addresses and zipcodes.
-    # ',', '(' and ')' are also left for potential use in additional line 2
-    # processing functions
-    addr_str = clean_upper(
-        addr_str, exclude=EXCLUDE_ALL, removal_cats=STRIP_CHAR_CATS
-    )
-
-    # to prevent any potential confusion between CT = COURT v CT = Connecticut,
-    # clean_ambiguous_street_types is not applied if state is CT.
-    if state and state != 'CT':
-        addr_str = clean_ambiguous_street_types(addr_str)
-
-    return addr_str
-
-
-def clean_ambiguous_street_types(addr_str):
-    # type: (str) -> str
-    """Clean street type abbreviations treated ambiguously by usaddress.
-
-    Some two char street type abbreviations (ie. CT) are treated as StateName
-    by usaddress when address lines are parsed in isolation. To correct this,
-    known problem abbreviations are converted to their whole word equivalent.
-
-    :param addr_str: string containing address street and occupancy data
-        without city and state.
-    :type addr_str: str | None
-    :return: original or cleaned addr_str
-    :rtype: str | None
-    """
-    if addr_str:
-        split_addr = addr_str.split()
-        for key in PROBLEM_ST_TYPE_ABBRVS:
-            if key in split_addr:
-                split_addr[split_addr.index(key)] = PROBLEM_ST_TYPE_ABBRVS[key]
-                addr_str = ' '.join(split_addr)
-                break
-    return addr_str
-
-
-def post_clean_addr_str(addr_str):
-    # type: (Union[str, None], Optional[bool]) -> str
-    """Remove any special chars or extra white space remaining post-processing.
-
-    :param addr_str: post-processing address string.
-    :type addr_str: str | None
-    :param is_line2: optional boolean to trigger extra line 2 processing.
-    :type is_line2: bool
-    :return: str set to uppercase, extra white space and special chars removed.
-    :rtype: str
-    """
-    if addr_str:
-        addr_str = clean_upper(
-            addr_str, exclude=ALLOWED_CHARS, removal_cats=STRIP_CHAR_CATS
-        )
-    return addr_str
-
-
-def _parse_occupancy(addr_line_2):
-    occupancy = None
-    if addr_line_2:
-        parsed = None
-        # first try usaddress parsing labels
-        try:
-            parsed = usaddress.tag(addr_line_2)
-        except usaddress.RepeatedLabelError:
-            pass
-        if parsed:
-            occupancy = parsed[0].get('OccupancyIdentifier')
-    return occupancy
-
-
-def strip_occupancy_type(addr_line_2):
-    # type: (str) -> str
-    """Strip occupancy type (ie apt, unit, etc) from addr_line_2 string
-
-    :param addr_line_2: address line 2 string that may contain type
-    :type addr_line_2: str
-    :return:
-    :rtype: str
-    """
-    occupancy = None
-    if addr_line_2:
-        addr_line_2 = addr_line_2.replace('#', '').strip().upper()
-        occupancy = _parse_occupancy(addr_line_2)
-
-        # if that doesn't work, clean abbrevs and try again
-        if not occupancy:
-            parts = str(addr_line_2).split()
-            for p in parts:
-                if p in OCCUPANCY_TYPE_ABBREVIATIONS:
-                    addr_line_2 = addr_line_2.replace(
-                        p, OCCUPANCY_TYPE_ABBREVIATIONS[p]
-                    )
-            occupancy = _parse_occupancy(addr_line_2)
-
-            # if that doesn't work, dissect it manually
-            if not occupancy:
-                occupancy = addr_line_2
-                types = (
-                    list(OCCUPANCY_TYPE_ABBREVIATIONS.keys())
-                    + list(OCCUPANCY_TYPE_ABBREVIATIONS.values())
-                )
-                if parts and len(parts) > 1:
-                    ids = [p for p in parts if p not in types]
-                    print(ids)
-                    occupancy = ' '.join(ids)
-
-    return occupancy
-
-
-def clean_upper(text,                           # type: Any
-                exclude=None,                   # type: Optional[Sequence[int]]
-                removal_cats=STRIP_CHAR_CATS,   # type: Optional[Sequence[str]]
-                strip_spaces=False              # type: Optional[bool]
-                ):
-    # type: (str, Optional[Sequence[int]], Optional[Sequence[str]]) -> str
-    """
-    Return text as upper case unicode string and remove unwanted characters.
-    Defaults to STRIP_CHARS e.g all  whitespace, punctuation etc
-    :param text: text to clean
-    :type text: str
-    :param exclude: sequence of char ordinals to exclude from text.translate
-    :type exclude: Sequence
-    :param removal_cats: sequence of strings identifying unicodedata categories
-        (or startswith) of characters to be removed from text
-    :type removal_cats: Sequence
-    :param strip_spaces: Bool to indicate whether to leave or remove all
-        spaces. Default is False (leaves single spaces)
-    :type strip_spaces: bool
-    :return: cleaned uppercase unicode string
-    :rtype: str
-    """
-    exclude = exclude or []
-    # coerce ints etc to str
-    if not isinstance(text, str):  # pragma: no cover
-        text = str(text)
-    # catch and convert fractions
-    text = unicodedata.normalize('NFKD', text)
-    text = text.translate({8260: '/'})
-
-    # evaluate string without commas (,) or ampersand (&) to determine if
-    # further processing is necessary
-    alnum_text = text.translate({44: None, 38: None})
-
-    # remove unwanted non-alphanumeric characters and convert all dash type
-    # characters to hyphen
-    if not alnum_text.replace(' ', '').isalnum():
-        for char in text:
-            if (unicodedata.category(char).startswith(removal_cats)
-                    and ord(char) not in exclude):
-                text = text.translate({ord(char): None})
-            elif unicodedata.category(char).startswith('Pd'):
-                text = text.translate({ord(char): '-'})
-    join_char = ' '
-    if strip_spaces:
-        join_char = ''
-    # remove extra spaces and convert to uppercase
-    return join_char.join(text.split()).upper()
-
-
-def clean_period_char(text):
-    """Remove all period characters that are not decimal points.
-
-    :param text: string text to clean
-    :type text: str
-    :return: cleaned string
-    :rtype: str
-    """
-    period_pattern = re.compile(r'\.(?!\d)')
-    return re.sub(period_pattern, '', text)
+#!/usr/bin/env python
+# encoding: utf-8
+"""
+copyright (c) 2016-2017 Earth Advantage.
+All rights reserved
+..codeauthor::Fable Turas <fable@rainsoftware.tech>
+
+[ INSERT DOC STRING ]  # TODO
+"""
+
+# Imports from Standard Library
+import re
+import unicodedata
+from typing import Any, Optional, Sequence, Union
+
+# Imports from Third Party Modules
+import usaddress
+
+# Local Imports
+from scourgify.address_constants import (
+    KNOWN_ODDITIES,
+    OCCUPANCY_TYPE_ABBREVIATIONS,
+    PROBLEM_ST_TYPE_ABBRVS,
+)
+
+# Setup
+
+# Constants
+# periods (in decimals), hyphens, / , and & are acceptable address components
+# ord('&') ord('#') ord('-'), ord('.') and ord('/')
+ALLOWED_CHARS = [35, 38, 45, 46, 47]
+
+# Don't remove ',', '(' or ')' in PRE_CLEAN
+PRECLEAN_EXCLUDE = [40, 41, 44]
+EXCLUDE_ALL = ALLOWED_CHARS + PRECLEAN_EXCLUDE
+
+STRIP_CHAR_CATS = (
+    'M', 'S', 'C', 'Nl', 'No', 'Pc', 'Ps', 'Pe', 'Pi', 'Pf', 'Po'
+)
+STRIP_PUNC_CATS = ('Z', 'Pd')
+STRIP_ALL_CATS = STRIP_CHAR_CATS + STRIP_PUNC_CATS
+
+# Data Structure Definitions
+
+# Private Functions
+
+
+# Public Classes and Functions
+
+def pre_clean_addr_str(addr_str, state=None):
+    # type: (str, Optional[str]) -> str
+    """Remove any known undesirable sub-strings and special characters.
+
+    Cleaning should be enacted on an addr_str to remove known characters
+    and phrases that might prevent usaddress from successfully parsing.
+    Follows USPS pub 28 guidelines for undesirable special characters.
+    Non-address phrases or character sets known to occur in raw addresses
+    should be added to address_constants.KNOWN_ODDITIES.
+
+    Some characters are left behind to potentially assist in second chance
+    processing of unparseable addresses and should be further cleaned
+    post_processing. (see post_clean_addr_str).
+
+    :param addr_str: raw address string
+    :type addr_str: str
+    :param state: optional string containing normalized state data.
+    :type state: str
+    :return: cleaned string
+    :rtype: str
+    """
+    # replace any easily handled, undesirable sub-strings
+    if any(oddity in addr_str for oddity in KNOWN_ODDITIES.keys()):
+        for key, replacement in KNOWN_ODDITIES.items():      # pragma: no cover
+            addr_str = addr_str.replace(key, replacement)
+
+    # remove non-decimal point period chars.
+    if '.' in addr_str:                                      # pragma: no cover
+        addr_str = clean_period_char(addr_str)
+
+    # remove special characters per USPS pub 28, except & which impacts
+    # intersection addresses, and - which impacts range addresses and zipcodes.
+    # ',', '(' and ')' are also left for potential use in additional line 2
+    # processing functions
+    addr_str = clean_upper(
+        addr_str, exclude=EXCLUDE_ALL, removal_cats=STRIP_CHAR_CATS
+    )
+
+    # to prevent any potential confusion between CT = COURT v CT = Connecticut,
+    # clean_ambiguous_street_types is not applied if state is CT.
+    if state and state != 'CT':
+        addr_str = clean_ambiguous_street_types(addr_str)
+
+    return addr_str
+
+
+def clean_ambiguous_street_types(addr_str):
+    # type: (str) -> str
+    """Clean street type abbreviations treated ambiguously by usaddress.
+
+    Some two char street type abbreviations (ie. CT) are treated as StateName
+    by usaddress when address lines are parsed in isolation. To correct this,
+    known problem abbreviations are converted to their whole word equivalent.
+
+    :param addr_str: string containing address street and occupancy data
+        without city and state.
+    :type addr_str: str | None
+    :return: original or cleaned addr_str
+    :rtype: str | None
+    """
+    if addr_str:
+        split_addr = addr_str.split()
+        for key in PROBLEM_ST_TYPE_ABBRVS:
+            if key in split_addr:
+                split_addr[split_addr.index(key)] = PROBLEM_ST_TYPE_ABBRVS[key]
+                addr_str = ' '.join(split_addr)
+                break
+    return addr_str
+
+
+def post_clean_addr_str(addr_str):
+    # type: (Union[str, None], Optional[bool]) -> str
+    """Remove any special chars or extra white space remaining post-processing.
+
+    :param addr_str: post-processing address string.
+    :type addr_str: str | None
+    :param is_line2: optional boolean to trigger extra line 2 processing.
+    :type is_line2: bool
+    :return: str set to uppercase, extra white space and special chars removed.
+    :rtype: str
+    """
+    if addr_str:
+        addr_str = clean_upper(
+            addr_str, exclude=ALLOWED_CHARS, removal_cats=STRIP_CHAR_CATS
+        )
+    return addr_str
+
+
+def _parse_occupancy(addr_line_2):
+    occupancy = None
+    if addr_line_2:
+        parsed = None
+        # first try usaddress parsing labels
+        try:
+            parsed = usaddress.tag(addr_line_2)
+        except usaddress.RepeatedLabelError:
+            pass
+        if parsed:
+            occupancy = parsed[0].get('OccupancyIdentifier')
+    return occupancy
+
+
+def strip_occupancy_type(addr_line_2):
+    # type: (str) -> str
+    """Strip occupancy type (ie apt, unit, etc) from addr_line_2 string
+
+    :param addr_line_2: address line 2 string that may contain type
+    :type addr_line_2: str
+    :return:
+    :rtype: str
+    """
+    occupancy = None
+    if addr_line_2:
+        addr_line_2 = addr_line_2.replace('#', '').strip().upper()
+        occupancy = _parse_occupancy(addr_line_2)
+
+        # if that doesn't work, clean abbrevs and try again
+        if not occupancy:
+            parts = str(addr_line_2).split()
+            for p in parts:
+                if p in OCCUPANCY_TYPE_ABBREVIATIONS:
+                    addr_line_2 = addr_line_2.replace(
+                        p, OCCUPANCY_TYPE_ABBREVIATIONS[p]
+                    )
+            occupancy = _parse_occupancy(addr_line_2)
+
+            # if that doesn't work, dissect it manually
+            if not occupancy:
+                occupancy = addr_line_2
+                types = (
+                    list(OCCUPANCY_TYPE_ABBREVIATIONS.keys())
+                    + list(OCCUPANCY_TYPE_ABBREVIATIONS.values())
+                )
+                if parts and len(parts) > 1:
+                    ids = [p for p in parts if p not in types]
+                    print(ids)
+                    occupancy = ' '.join(ids)
+
+    return occupancy
+
+
+def clean_upper(text,                           # type: Any
+                exclude=None,                   # type: Optional[Sequence[int]]
+                removal_cats=STRIP_CHAR_CATS,   # type: Optional[Sequence[str]]
+                strip_spaces=False              # type: Optional[bool]
+                ):
+    # type: (str, Optional[Sequence[int]], Optional[Sequence[str]]) -> str
+    """
+    Return text as upper case unicode string and remove unwanted characters.
+    Defaults to STRIP_CHARS e.g all  whitespace, punctuation etc
+    :param text: text to clean
+    :type text: str
+    :param exclude: sequence of char ordinals to exclude from text.translate
+    :type exclude: Sequence
+    :param removal_cats: sequence of strings identifying unicodedata categories
+        (or startswith) of characters to be removed from text
+    :type removal_cats: Sequence
+    :param strip_spaces: Bool to indicate whether to leave or remove all
+        spaces. Default is False (leaves single spaces)
+    :type strip_spaces: bool
+    :return: cleaned uppercase unicode string
+    :rtype: str
+    """
+    exclude = exclude or []
+    # coerce ints etc to str
+    if not isinstance(text, str):  # pragma: no cover
+        text = str(text)
+    # catch and convert fractions
+    text = unicodedata.normalize('NFKD', text)
+    text = text.translate({8260: '/'})
+
+    # evaluate string without commas (,) or ampersand (&) to determine if
+    # further processing is necessary
+    alnum_text = text.translate({44: None, 38: None})
+
+    # remove unwanted non-alphanumeric characters and convert all dash type
+    # characters to hyphen
+    if not alnum_text.replace(' ', '').isalnum():
+        for char in text:
+            if (unicodedata.category(char).startswith(removal_cats)
+                    and ord(char) not in exclude):
+                text = text.translate({ord(char): None})
+            elif unicodedata.category(char).startswith('Pd'):
+                text = text.translate({ord(char): '-'})
+    join_char = ' '
+    if strip_spaces:
+        join_char = ''
+    # remove extra spaces and convert to uppercase
+    return join_char.join(text.split()).upper()
+
+
+def clean_period_char(text):
+    """Remove all period characters that are not decimal points.
+
+    :param text: string text to clean
+    :type text: str
+    :return: cleaned string
+    :rtype: str
+    """
+    period_pattern = re.compile(r'\.(?!\d)')
+    return re.sub(period_pattern, '', text)
```

### Comparing `usaddress-scourgify-0.2.4/scourgify/normalize.py` & `usaddress-scourgify-0.3.0/scourgify/normalize.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,681 +1,829 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-copyright (c) 2016  Earth Advantage.
-All rights reserved
-..codeauthor::Fable Turas <fable@rainsoftware.tech>
-
-Provides functions to normalize address per USPS pub 28 and/or RESO standards.
-"""
-# TODO: Find why # with no street gets through
-# form_normalization = {
-#     'jurisdiction_property_id': 'TST123',
-#     'address_line_1': '123',
-#     'city': 'Portland',
-#     'state': 'OR',
-#     'postal_code': '97212'
-# }
-
-# Imports from Standard Library
-
-from string import Template
-from collections import OrderedDict  # noqa # pylint: disable=unused-import
-from typing import (  # noqa # pylint: disable=unused-import
-    Callable,
-    Mapping,
-    MutableMapping,
-    Optional,
-    Sequence,
-    Union,
-)
-
-# Imports from Third Party Modules
-import geocoder
-import usaddress
-
-# Local Imports
-from scourgify.address_constants import (
-    ABNORMAL_OCCUPANCY_ABBRVS,
-    ADDRESS_KEYS,
-    DIRECTIONAL_REPLACEMENTS,
-    OCCUPANCY_TYPE_ABBREVIATIONS,
-    STATE_ABBREVIATIONS,
-    STREET_TYPE_ABBREVIATIONS,
-)
-from scourgify.cleaning import (
-    clean_upper,
-    post_clean_addr_str,
-    pre_clean_addr_str,
-    strip_occupancy_type,
-)
-from scourgify.exceptions import (
-    AddressNormalizationError,
-    AmbiguousAddressError,
-    UnParseableAddressError,
-)
-from scourgify.validations import (
-    validate_address_components,
-    validate_parens_groups_parsed,
-    validate_us_postal_code_format,
-)
-
-# Setup
-
-# Constants
-
-LINE1_USADDRESS_LABELS = (
-    'AddressNumber',
-    'StreetName',
-    'AddressNumberPrefix',
-    'AddressNumberSuffix',
-    'StreetNamePreDirectional',
-    'StreetNamePostDirectional',
-    'StreetNamePreModifier',
-    'StreetNamePostType',
-    'StreetNamePreType',
-    'IntersectionSeparator',
-    'SecondStreetNamePreDirectional',
-    'SecondStreetNamePostDirectional',
-    'SecondStreetNamePreModifier',
-    'SecondStreetNamePostType',
-    'SecondStreetNamePreType',
-    'LandmarkName',
-    'CornerOf',
-    'IntersectionSeparator',
-    'BuildingName',
-)
-LINE2_USADDRESS_LABELS = (
-    'OccupancyType',
-    'OccupancyIdentifier',
-    'SubaddressIdentifier',
-    'SubaddressType',
-)
-
-LAST_LINE_LABELS = (
-    'PlaceName',
-    'StateName',
-    'ZipCode',
-)
-
-AMBIGUOUS_LABELS = (
-    'Recipient',
-    'USPSBoxType',
-    'USPSBoxID',
-    'USPSBoxGroupType',
-    'USPSBoxGroupID',
-    'NotAddress'
-)
-
-STRIP_CHAR_CATS = (
-    'M', 'S', 'C', 'Nl', 'No', 'Pc', 'Ps', 'Pe', 'Pi', 'Pf', 'Po'
-)
-STRIP_PUNC_CATS = ('Z', 'Pd')
-STRIP_ALL_CATS = STRIP_CHAR_CATS + STRIP_PUNC_CATS
-
-
-# Private Functions
-
-# Public Classes and Functions
-
-def normalize_address_record(address, addr_map=None, addtl_funcs=None,
-                             strict=True):
-    # type: (Union[str, Mapping[str, str]]) -> Mapping[str, str]
-    """Normalize an address according to USPS pub. 28 standards.
-
-    Takes an address string, or a dict-like with standard address fields
-    (address_line_1, address_line_2, city, state, postal_code), removes
-    unacceptable special characters, extra spaces, predictable abnormal
-    character sub-strings and phrases, abbreviates directional indicators
-    and street types.  If applicable, line 2 address elements (ie: Apt, Unit)
-    are separated from line 1 inputs.
-
-    addr_map, if used, must be in the format {standard_key: custom_key} based
-    on standard address keys sighted above.
-
-    Returns an address dict with all field values in uppercase format.
-
-    :param address: str or dict-like object containing details of a single
-        address.
-    :type address: str | Mapping[str, str]
-    :param addr_map: mapping of standard address fields to custom key names
-    :type addr_map: Mapping[str, str]
-    :param addtl_funcs: optional sequence of funcs that take string for further
-        processing and return line1 and line2 strings
-    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
-    :param strict: bool indicating strict handling of components address parts
-        city, state and postal_code, vs city and state OR postal_code
-    :return: address dict containing parsed and normalized address values.
-    :rtype: Mapping[str, str]
-    """
-    if isinstance(address, str):
-        return normalize_addr_str(address, addtl_funcs=addtl_funcs)
-    else:
-        return normalize_addr_dict(
-            address, addr_map=addr_map, addtl_funcs=addtl_funcs, strict=strict
-        )
-
-
-def normalize_addr_str(addr_str,         # type: str
-                       line2=None,       # type: Optional[str]
-                       city=None,        # type: Optional[str]
-                       state=None,       # type: Optional[str]
-                       zipcode=None,     # type: Optional[str]
-                       addtl_funcs=None  # type: Sequence[Callable[[str,str], str]]  # noqa
-                      ):                                        # noqa
-    # type (...) -> Mapping[str, str]                                        # noqa
-    # type (...) -> Mapping[str, str]
-    """Normalize a complete or partial address string.
-
-    :param addr_str: str containing address data.
-    :type addr_str: str
-    :param line2: optional str containing occupancy or sub-address data
-        (eg: Unit, Apt, Lot).
-    :type line2: str
-    :param city: optional str city name that does not need to be parsed from
-        addr_str.
-    :type city: str
-    :param state: optional str state name that does not need to be parsed from
-        addr_str.
-    :type state: str
-    :param zipcode: optional str postal code that does not need to be parsed
-        from addr_str.
-    :type zipcode: str
-    :param addtl_funcs: optional sequence of funcs that take string for further
-        processing and return line1 and line2 strings
-    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
-    :return: address dict with uppercase parsed and normalized address values.
-    :rtype: Mapping[str, str]
-    """
-    # get address parsed into usaddress components.
-    error = None
-    parsed_addr = None
-    addr_str = pre_clean_addr_str(addr_str, normalize_state(state))
-    try:
-        parsed_addr = parse_address_string(addr_str)
-    except (usaddress.RepeatedLabelError, AmbiguousAddressError) as err:
-        error = err
-        if not line2 and addtl_funcs:
-            for func in addtl_funcs:
-                try:
-                    line1, line2 = func(addr_str)
-                    error = False
-                    # send refactored line_1 and line_2 back through processing
-                    return normalize_addr_str(line1, line2=line2, city=city,
-                                              state=state, zipcode=zipcode)
-                except ValueError:
-                    # try a different additional processing function
-                    pass
-
-    if parsed_addr and not parsed_addr.get('StreetName'):
-        addr_dict = dict(
-            address_line_1=addr_str, address_line_2=line2, city=city,
-            state=state, postal_code=zipcode
-        )
-        full_addr = format_address_record(addr_dict)
-        try:
-            parsed_addr = parse_address_string(full_addr)
-        except (usaddress.RepeatedLabelError, AmbiguousAddressError) as err:
-            parsed_addr = None
-            error = err
-
-    if parsed_addr:
-        parsed_addr = normalize_address_components(parsed_addr)
-        zipcode = get_parsed_values(parsed_addr, zipcode, 'ZipCode', addr_str)
-        city = get_parsed_values(parsed_addr, city, 'PlaceName', addr_str)
-        state = get_parsed_values(parsed_addr, state, 'StateName', addr_str)
-        state = normalize_state(state)
-
-        # assumes if line2 is passed in that it need not be parsed from
-        # addr_str. Primarily used to allow advanced processing of otherwise
-        # unparsable addresses.
-        line2 = line2 if line2 else get_normalized_line_segment(
-            parsed_addr, LINE2_USADDRESS_LABELS
-        )
-        line2 = post_clean_addr_str(line2)
-        # line 1 is fully post cleaned in get_normalized_line_segment.
-        line1 = get_normalized_line_segment(
-            parsed_addr, LINE1_USADDRESS_LABELS
-        )
-        validate_parens_groups_parsed(line1)
-    else:
-        # line1 is set to addr_str so complete dict can be passed to error.
-        line1 = addr_str
-
-    addr_rec = dict(
-        address_line_1=line1, address_line_2=line2, city=city,
-        state=state, postal_code=zipcode
-    )
-    if error:
-        raise UnParseableAddressError(None, None, addr_rec)
-    else:
-        return addr_rec
-
-
-def normalize_addr_dict(addr_dict, addr_map=None, addtl_funcs=None,
-                        strict=True):
-    # type: (Mapping[str, str]) -> Mapping[str, str]
-    """Normalize an address from dict or dict-like object.
-
-    Assumes addr_dict will have standard address related keys (address_line_1,
-    address_line_2, city, state, postal_code), unless addr_map is provided.
-
-    addr_map, if used, must be in the format {standard_key: custom_key} based
-    on standard address keys sighted above.
-
-    :param addr_dict: mapping containing address keys and values.
-    :type addr_dict: Mapping
-    :param addr_map: mapping of standard address fields to custom key names
-    :type addr_map: Mapping[str, str]
-    :param addtl_funcs: optional sequence of funcs that take string for further
-        processing and return line1 and line2 strings
-    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
-    :param strict: bool indicating strict handling of components address parts
-        city, state and postal_code, vs city and state OR postal_code
-    :return: address dict with normalized, uppercase address values.
-    :rtype: Mapping[str, str]
-    """
-    if addr_map:
-        addr_dict = {key: addr_dict.get(val) for key, val in addr_map.items()}
-    addr_dict = validate_address_components(addr_dict, strict=strict)
-
-    # line 1 and line 2 elements are combined to ensure consistent processing
-    # whether the line 2 elements are pre-parsed or included in line 1
-    addr_str = get_addr_line_str(addr_dict, comma_separate=True)
-    postal_code = addr_dict.get('postal_code')
-    zipcode = validate_us_postal_code_format(
-        postal_code, addr_dict
-    ) if postal_code else None
-    city = addr_dict.get('city')
-    state = addr_dict.get('state')
-    try:
-        address = normalize_addr_str(
-            addr_str, city=city, state=state,
-            zipcode=zipcode, addtl_funcs=addtl_funcs
-        )
-    except AddressNormalizationError:
-        addr_str = get_addr_line_str(
-            addr_dict, comma_separate=True, addr_parts=ADDRESS_KEYS
-        )
-        address = normalize_addr_str(
-            addr_str, city=city, state=state,
-            zipcode=zipcode, addtl_funcs=addtl_funcs
-        )
-    return address
-
-
-def parse_address_string(addr_str):
-    # type: (str) -> MutableMapping[str, str]
-    """Separate an address string into its component parts per usaddress.
-
-    Attempts to parse addr_str into it's component parts, using usaddress.
-
-    If usaddress identifies the address type as Ambiguous or the resulting
-    OrderedDict includes any keys from AMBIGUOUS_LABELS that would constitute
-    ambiguous address in the SEED/GBR use case (ie: Recipient) then
-    an AmbiguousAddressError is raised.
-
-    :param addr_str: str address to be processed.
-    :type addr_str: str
-    :return: usaddress OrderedDict
-    :rtype: MutableMapping
-    """
-    parsed_results = usaddress.tag(addr_str)
-    parsed_addr = parsed_results[0]
-    # if the address is parseable but some form of ambiguity is found that
-    # may result in data corruption NormalizationError is raised.
-    if (parsed_results[1] == 'Ambiguous' or
-            any(key in AMBIGUOUS_LABELS for key in parsed_addr.keys())):
-        raise AmbiguousAddressError()
-    parsed_addr = handle_abnormal_occupancy(parsed_addr, addr_str)
-    return parsed_addr
-
-
-def handle_abnormal_occupancy(parsed_addr, addr_str):
-    """Handle abnormal occupancy abbreviations that are parsed as street type.
-
-    Evaluates addresses with an Occupancy or Subaddress identifier whose type
-    may be parsed into StreetNamePostType and swaps the StreetNamePostType tag
-    for the OccupancyType tag if necessary.
-
-    For example: Portland Maps uses 'UN' as an abbreviation for 'Unit' which
-    usaddress parses to 'StreetNamePostType' since 'UN' is correctly an
-    abbreviation for 'Union' street type.
-        123 MAIN UN => 123 MAIN UN
-        123 MAIN UN A => 123 MAIN, UNIT A
-        123 MAIN UN UN A => 123 MAIN UN, UNIT A
-
-    :param parsed_addr: address parsed into usaddress components
-    :type parsed_addr: OrderedDict
-    :param addr_str: Original address string
-    :type addr_str: str
-    :return: parsed address
-    :rtype: OrderedDict
-    """
-    occupancy_id_key = None
-    occupany_type_key = 'OccupancyType'
-    street_type_key = 'StreetNamePostType'
-    occupany_type_keys = (occupany_type_key, 'SubaddressType')
-    occupancy_identifier_keys = ('OccupancyIdentifier', 'SubaddressIdentifier')
-    street_type = parsed_addr.get(street_type_key)
-    if street_type in ABNORMAL_OCCUPANCY_ABBRVS:
-        occupancy_type = None
-        occupancy = None
-        for key in occupany_type_keys:
-            try:
-                occupancy_type = parsed_addr[key]
-                break
-            except KeyError:
-                pass
-        for key in occupancy_identifier_keys:
-            try:
-                occupancy = parsed_addr[key]
-                occupancy_id_key = key
-                break
-            except KeyError:
-                break
-        if occupancy and not occupancy_type:
-            if street_type in occupancy:
-                occupancy = occupancy.replace(street_type, '').strip()
-                del parsed_addr[occupancy_id_key]
-            else:
-                line2 = "{} {}".format(street_type, occupancy)
-                addr_str = addr_str.replace(line2, '')
-                parsed_addr = parse_address_string(addr_str)
-            parsed_addr.update({occupany_type_key: street_type})
-            parsed_addr.update({occupancy_id_key: occupancy})
-    return parsed_addr
-
-
-def get_parsed_values(parsed_addr, orig_val, val_label, orig_addr_str):
-    # type: (Mapping[str, str], str, str, str) -> Union[str, None]
-    """Get valid values from parsed_addr corresponding to val_label.
-
-    Retrieves values from parsed_addr corresponding to the label supplied in
-    val_label.
-    If a value for val_label is found in parsed_addr AND an orig_val is
-    supplied, a single string will be returned if the values match. If only
-    one of the two contains a non-null value.
-    If both values are empty, None is returned.
-    If the values an AmbiguousAddressError will be returned if the two values
-    are not equal. This provides a check against misidentified address
-    components when known values are available. (For example when a city is
-    supplied from the address dict or record being normalized, but usaddress
-    identifies extra information stored in address_line_1 as a PlaceName.)
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr: Mapping
-    :param orig_val: related value passed in from incoming data source.
-    :type orig_val: str
-    :param val_label: label to locate in parsed_addr
-    :type val_label: str
-    :param orig_addr_str: address string to pass to error, if applicable.
-    :type orig_addr_str: str
-    :return: str | None
-    """
-    val_from_parse = parsed_addr.get(val_label)
-    orig_val = post_clean_addr_str(orig_val)
-    val_from_parse = post_clean_addr_str(val_from_parse)
-    non_null_val_set = {orig_val, val_from_parse} - {None}
-    if len(non_null_val_set) > 1:
-        raise AmbiguousAddressError(None, None, orig_addr_str)
-    else:
-        return non_null_val_set.pop() if non_null_val_set else None
-
-
-def normalize_address_components(parsed_addr):
-    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
-    """Normalize parsed sections of address as appropriate.
-
-    Processes parsed address through subsets of normalization rules.
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr:Mapping
-    :return: parsed_addr with normalization processing applied to elements.
-    :rtype: dict
-    """
-    parsed_addr = normalize_numbered_streets(parsed_addr)
-    parsed_addr = normalize_directionals(parsed_addr)
-    parsed_addr = normalize_street_types(parsed_addr)
-    parsed_addr = normalize_occupancy_type(parsed_addr)
-    return parsed_addr
-
-
-def normalize_numbered_streets(parsed_addr):
-    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
-    """Change numbered street names to include missing original identifiers.
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr: Mapping
-    :return: parsed_addr with ordinal identifiers appended to numbered streets.
-    :rtype: dict"""
-    street_tags = ['StreetName', 'SecondStreetName']
-    for tag in street_tags:
-        post_type_tag = '{}PostType'.format(tag)
-        # limits updates to numbered street names that include a post street
-        # type, since an ordinal indicator would be inappropriate for some
-        # numbered streets (ie. Country Road 97).
-        if tag in parsed_addr.keys() and post_type_tag in parsed_addr.keys():
-            try:
-                cardinal = int(parsed_addr[tag])
-                ord_indicator = get_ordinal_indicator(cardinal)
-                parsed_addr[tag] = '{}{}'.format(cardinal, ord_indicator)
-            except ValueError:
-                pass
-    return parsed_addr
-
-
-def normalize_directionals(parsed_addr):
-    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
-    """Change directional notations to standard abbreviations.
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr: Mapping
-    :return: parsed_addr with directionals updated to abbreviated format.
-    :rtype: dict
-    """
-    # get the directional related keys from the current address.
-    found_directional_tags = (
-        tag for tag in parsed_addr.keys() if 'Directional' in tag
-    )
-    for found in found_directional_tags:
-        # get the original directional related value per key.
-        dir_str = parsed_addr[found]
-        # remove spaces, punctuation, hyphens etc so two part directions
-        # conform to a single word standard. Convert to upper case
-        dir_str = clean_upper(
-            dir_str, exclude=[], removal_cats=STRIP_ALL_CATS, strip_spaces=True
-        )
-        if dir_str in DIRECTIONAL_REPLACEMENTS.keys():
-            parsed_addr[found] = DIRECTIONAL_REPLACEMENTS[dir_str]
-    return parsed_addr
-
-
-def normalize_street_types(parsed_addr):
-    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
-    """Change street types to accepted abbreviated format.
-
-    No change is made if street types do not conform to common usages per
-    USPS pub 28 appendix C.
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr: Mapping
-    :return: parsed_addr with street types updated to abbreviated format.
-    :rtype: dict
-    """
-    # get the *Street*Type keys from the current parsed address.
-    found_type_tags = (
-        tag for tag in parsed_addr.keys() if 'Street' in tag and 'Type' in tag
-    )
-    for found in found_type_tags:
-        # lookup the appropriate abbrev for the street type found per key.
-        type_abbr = STREET_TYPE_ABBREVIATIONS.get(parsed_addr[found])
-        # update the street type only if a new abbreviation is found.
-        if type_abbr:
-            parsed_addr[found] = type_abbr
-    return parsed_addr
-
-
-def normalize_occupancy_type(parsed_addr, default=None):
-    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
-    """Change occupancy types to accepted abbreviated format.
-
-    If there is an occupancy and it does not conform to one of the
-    OCCUPANCY_TYPE_ABBREVIATIONS, occupancy is changed to the generic 'UNIT'.
-    OCCUPANCY_TYPE_ABBREVIATIONS contains common abbreviations per
-    USPS pub 28 appendix C, however, OCCUPANCY_TYPE_ABBREVIATIONS can be
-    customized to allow alternate abbreviations to pass through. (see README)
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :type parsed_addr: Mapping
-    :param default: default abbreviation to use for types that fall outside the
-     standard abbreviations. Default is 'UNIT'
-    :return: parsed_addr with occupancy types updated to abbreviated format.
-    :rtype: dict
-    """
-    default = default if default is not None else 'UNIT'
-    occupancy_type_label = 'OccupancyType'
-    occupancy_type = parsed_addr.pop(occupancy_type_label, None)
-    occupancy_type_abbr = (
-        occupancy_type
-        if occupancy_type in OCCUPANCY_TYPE_ABBREVIATIONS.values()
-        else OCCUPANCY_TYPE_ABBREVIATIONS.get(occupancy_type)
-    )
-    occupancy_id = parsed_addr.get('OccupancyIdentifier')
-    if ((occupancy_id and not occupancy_id.startswith('#'))
-            and not occupancy_type_abbr):
-        occupancy_type_abbr = default
-    if occupancy_type_abbr:
-        parsed_list = list(parsed_addr.items())
-        index = parsed_list.index(('OccupancyIdentifier', occupancy_id))
-        parsed_list.insert(index, (occupancy_type_label, occupancy_type_abbr))
-        parsed_addr = OrderedDict(parsed_list)
-    return parsed_addr
-
-
-def normalize_state(state):
-    # type: (Union[str, None]) -> Union[str, None]
-    """Change state string to accepted abbreviated format.
-
-    :param state: string containing state name or abbreviation.
-    :type state: str | None
-    :return: 2 char state abbreviation, or original state string if not found
-        in state names or standard long abbreviations.
-    :rtype: str | None
-    """
-    if state:
-        state_abbrv = STATE_ABBREVIATIONS.get(state.upper())
-        if state_abbrv:
-            state = state_abbrv
-    return state
-
-
-def get_normalized_line_segment(parsed_addr, line_labels):
-    # type: (Mapping[str, str], Sequence[str]) -> str
-    """
-
-    :param parsed_addr: address parsed into ordereddict per usaddress.
-    :param line_labels: tuple of str labels of all the potential keys related
-        to the desired address segment (ie address_line_1 or address_line_2).
-    :return: s/r joined values from parsed_addr corresponding to given labels.
-    """
-    line_elems = [
-        elem for key, elem in parsed_addr.items() if key in line_labels
-    ]
-    line_str = ' '.join(line_elems) if line_elems else None
-    return post_clean_addr_str(line_str)
-
-
-def get_addr_line_str(addr_dict, addr_parts=None, comma_separate=False):
-    # type: (Mapping[str, str], Optional[Sequence], bool) -> str
-    """Get address 'line' elements as a single string.
-
-    Combines 'address_line_1' and 'address_line_2' elements as a single string
-    to ensure no data is lost and line_2 can be processed according to a
-    standard set of rules.
-
-    :param addr_dict: dict containing keys 'address_line_1', 'address_line_2'.
-    :type addr_dict: Mapping
-    :param addr_parts: optional sequence of address elements
-    :type addr_parts:
-    :param comma_separate: optional boolean to separate dict values by comma
-        useful for dealing with potentially ambiguous line 2 segments
-    :type bool:
-    :return: string combining 'address_line_1' & 'address_line_2' values.
-    :rtype: str
-    """
-    if not addr_parts:
-        addr_parts = ['address_line_1', 'address_line_2']
-    if not isinstance(addr_parts, (list, tuple)):
-        raise TypeError('addr_parts must be a list or tuple')
-    separator = ', ' if comma_separate else ' '
-    addr_str = separator.join(
-        str(addr_dict[elem]) for elem in addr_parts if addr_dict.get(elem)
-    )
-    return addr_str
-
-
-def format_address_record(address):
-    # type AddressRecord -> str
-    """Format AddressRecord as string."""
-    address_template = Template('$address')
-    address = dict(address)
-    addr_parts = [
-        str(address[field]) for field in ADDRESS_KEYS if address.get(field)
-    ]
-    return address_template.safe_substitute(address=', '.join(addr_parts))
-
-
-def get_geocoder_normalized_addr(address, addr_keys=ADDRESS_KEYS):
-    # type: (Union[Mapping, str], Optional[Sequence]) -> dict
-    """Get geocoder normalized address parsed to dict with addr_keys.
-
-    :param address: string or dict-like containing address data
-    :param addr_keys: optional list of address keys. standard list of keys will
-        be used if not supplied
-    :return: dict containing geocoder address result
-    """
-    address_line_2 = None
-    geo_addr_dict = {}
-    if not isinstance(address, str):
-        address_line_2 = address.get('address_line_2')
-        address = get_addr_line_str(address, addr_parts=addr_keys)
-    geo_resp = geocoder.google(address)
-    if geo_resp.ok and geo_resp.housenumber:
-        line2 = geo_resp.subpremise or address_line_2
-        geo_addr_dict = {
-            'address_line_1':
-                ' '.join([geo_resp.housenumber, geo_resp.street]),
-            'address_line_2': strip_occupancy_type(line2),
-            'city': geo_resp.city,
-            'state': geo_resp.state,
-            'postal_code': geo_resp.postal
-        }
-        for key, value in geo_addr_dict.items():
-            geo_addr_dict[key] = value.upper() if value else None
-    return geo_addr_dict
-
-
-def get_ordinal_indicator(number):
-    # type: (int) -> str
-    """Get the ordinal indicator suffix applicable to the supplied number.
-
-     Ordinal numbers are words representing position or rank in a sequential
-     order (1st, 2nd, 3rd, etc).
-     Ordinal indicators are the suffix characters (st, nd, rd, th) that, when
-     applied to a numeral (int), denote that it an ordinal number.
-
-    :param number: int
-    :type: int
-    :return: ordinal indicator appropriate to the number supplied.
-    :rtype: str
-    """
-    str_num = str(number)
-    digits = len(str_num)
-    if str_num[-1] == '1' and not (digits >= 2 and str_num[-2:] == '11'):
-        return 'st'
-    elif str_num[-1] == '2' and not (digits >= 2 and str_num[-2:] == '12'):
-        return 'nd'
-    elif str_num[-1] == '3' and not (digits >= 2 and str_num[-2:] == '13'):
-        return 'rd'
-    else:
-        return 'th'
+#!/usr/bin/env python
+# encoding: utf-8
+"""
+copyright (c) 2016  Earth Advantage.
+All rights reserved
+..codeauthor::Fable Turas <fable@rainsoftware.tech>
+
+Provides functions to normalize address per USPS pub 28 and/or RESO standards.
+"""
+# TODO: Find why # with no street gets through
+# form_normalization = {
+#     'jurisdiction_property_id': 'TST123',
+#     'address_line_1': '123',
+#     'city': 'Portland',
+#     'state': 'OR',
+#     'postal_code': '97212'
+# }
+
+# Imports from Standard Library
+
+from string import Template
+from collections import OrderedDict  # noqa # pylint: disable=unused-import
+from typing import (  # noqa # pylint: disable=unused-import
+    Callable,
+    Mapping,
+    MutableMapping,
+    Optional,
+    Sequence,
+    Union,
+)
+
+# Imports from Third Party Modules
+import geocoder
+import usaddress
+
+# Local Imports
+from scourgify.address_constants import (
+    ABNORMAL_OCCUPANCY_ABBRVS,
+    ADDRESS_KEYS,
+    DIRECTIONAL_REPLACEMENTS,
+    OCCUPANCY_TYPE_ABBREVIATIONS,
+    STATE_ABBREVIATIONS,
+    STREET_TYPE_ABBREVIATIONS,
+)
+from scourgify.cleaning import (
+    clean_upper,
+    post_clean_addr_str,
+    pre_clean_addr_str,
+    strip_occupancy_type,
+)
+from scourgify.exceptions import (
+    AddressNormalizationError,
+    AmbiguousAddressError,
+    UnParseableAddressError,
+)
+from scourgify.validations import (
+    validate_address_components,
+    validate_parens_groups_parsed,
+    validate_us_postal_code_format,
+)
+
+# Setup
+
+# Constants
+
+LINE1_USADDRESS_LABELS = (
+    'AddressNumber',
+    'StreetName',
+    'AddressNumberPrefix',
+    'AddressNumberSuffix',
+    'StreetNamePreDirectional',
+    'StreetNamePostDirectional',
+    'StreetNamePreModifier',
+    'StreetNamePostType',
+    'StreetNamePreType',
+    'IntersectionSeparator',
+    'SecondStreetNamePreDirectional',
+    'SecondStreetNamePostDirectional',
+    'SecondStreetNamePreModifier',
+    'SecondStreetNamePostType',
+    'SecondStreetNamePreType',
+    'LandmarkName',
+    'CornerOf',
+    'IntersectionSeparator',
+    'BuildingName',
+)
+LINE2_USADDRESS_LABELS = (
+    'OccupancyType',
+    'OccupancyIdentifier',
+    'SubaddressIdentifier',
+    'SubaddressType',
+)
+
+LAST_LINE_LABELS = (
+    'PlaceName',
+    'StateName',
+    'ZipCode',
+)
+
+AMBIGUOUS_LABELS = (
+    'Recipient',
+    'USPSBoxType',
+    'USPSBoxID',
+    'USPSBoxGroupType',
+    'USPSBoxGroupID',
+    'NotAddress'
+)
+
+STRIP_CHAR_CATS = (
+    'M', 'S', 'C', 'Nl', 'No', 'Pc', 'Ps', 'Pe', 'Pi', 'Pf', 'Po'
+)
+STRIP_PUNC_CATS = ('Z', 'Pd')
+STRIP_ALL_CATS = STRIP_CHAR_CATS + STRIP_PUNC_CATS
+
+
+# Private Functions
+
+# Public Classes and Functions
+
+def normalize_address_record(address, addr_map=None, addtl_funcs=None,
+                             strict=True):
+    # type: (Union[str, Mapping[str, str]]) -> Mapping[str, str]
+    """Normalize an address according to USPS pub. 28 standards.
+
+    Takes an address string, or a dict-like with standard address fields
+    (address_line_1, address_line_2, city, state, postal_code), removes
+    unacceptable special characters, extra spaces, predictable abnormal
+    character sub-strings and phrases, abbreviates directional indicators
+    and street types.  If applicable, line 2 address elements (ie: Apt, Unit)
+    are separated from line 1 inputs.
+
+    addr_map, if used, must be in the format {standard_key: custom_key} based
+    on standard address keys sighted above.
+
+    Returns an address dict with all field values in uppercase format.
+
+    :param address: str or dict-like object containing details of a single
+        address.
+    :type address: str | Mapping[str, str]
+    :param addr_map: mapping of standard address fields to custom key names
+    :type addr_map: Mapping[str, str]
+    :param addtl_funcs: optional sequence of funcs that take string for further
+        processing and return line1 and line2 strings
+    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
+    :param strict: bool indicating strict handling of components address parts
+        city, state and postal_code, vs city and state OR postal_code
+    :return: address dict containing parsed and normalized address values.
+    :rtype: Mapping[str, str]
+    """
+    if isinstance(address, str):
+        return normalize_addr_str(address, addtl_funcs=addtl_funcs)
+    else:
+        return normalize_addr_dict(
+            address, addr_map=addr_map, addtl_funcs=addtl_funcs, strict=strict
+        )
+
+
+def normalize_addr_str(addr_str,         # type: str
+                       line2=None,       # type: Optional[str]
+                       city=None,        # type: Optional[str]
+                       state=None,       # type: Optional[str]
+                       zipcode=None,     # type: Optional[str]
+                       addtl_funcs=None  # type: Sequence[Callable[[str,str], str]]  # noqa
+                      ):                                        # noqa
+    # type (...) -> Mapping[str, str]                                        # noqa
+    # type (...) -> Mapping[str, str]
+    """Normalize a complete or partial address string.
+
+    :param addr_str: str containing address data.
+    :type addr_str: str
+    :param line2: optional str containing occupancy or sub-address data
+        (eg: Unit, Apt, Lot).
+    :type line2: str
+    :param city: optional str city name that does not need to be parsed from
+        addr_str.
+    :type city: str
+    :param state: optional str state name that does not need to be parsed from
+        addr_str.
+    :type state: str
+    :param zipcode: optional str postal code that does not need to be parsed
+        from addr_str.
+    :type zipcode: str
+    :param addtl_funcs: optional sequence of funcs that take string for further
+        processing and return line1 and line2 strings
+    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
+    :return: address dict with uppercase parsed and normalized address values.
+    :rtype: Mapping[str, str]
+    """
+    # get address parsed into usaddress components.
+    error = None
+    parsed_addr = None
+    addr_str = pre_clean_addr_str(addr_str, normalize_state(state))
+    try:
+        parsed_addr = parse_address_string(addr_str)
+    except (usaddress.RepeatedLabelError, AmbiguousAddressError) as err:
+        error = err
+        if not line2 and addtl_funcs:
+            for func in addtl_funcs:
+                try:
+                    line1, line2 = func(addr_str)
+                    error = False
+                    # send refactored line_1 and line_2 back through processing
+                    return normalize_addr_str(line1, line2=line2, city=city,
+                                              state=state, zipcode=zipcode)
+                except ValueError:
+                    # try a different additional processing function
+                    pass
+
+    if parsed_addr and not parsed_addr.get('StreetName'):
+        addr_dict = dict(
+            address_line_1=addr_str, address_line_2=line2, city=city,
+            state=state, postal_code=zipcode
+        )
+        full_addr = format_address_record(addr_dict)
+        try:
+            parsed_addr = parse_address_string(full_addr)
+        except (usaddress.RepeatedLabelError, AmbiguousAddressError) as err:
+            parsed_addr = None
+            error = err
+
+    if parsed_addr:
+        parsed_addr = normalize_address_components(parsed_addr)
+        zipcode = get_parsed_values(parsed_addr, zipcode, 'ZipCode', addr_str)
+        city = get_parsed_values(parsed_addr, city, 'PlaceName', addr_str)
+        state = get_parsed_values(parsed_addr, state, 'StateName', addr_str)
+        state = normalize_state(state)
+
+        # assumes if line2 is passed in that it need not be parsed from
+        # addr_str. Primarily used to allow advanced processing of otherwise
+        # unparsable addresses.
+        line2 = line2 if line2 else get_normalized_line_segment(
+            parsed_addr, LINE2_USADDRESS_LABELS
+        )
+        line2 = post_clean_addr_str(line2)
+        # line 1 is fully post cleaned in get_normalized_line_segment.
+        line1 = get_normalized_line_segment(
+            parsed_addr, LINE1_USADDRESS_LABELS
+        )
+        validate_parens_groups_parsed(line1)
+    else:
+        # line1 is set to addr_str so complete dict can be passed to error.
+        line1 = addr_str
+
+    addr_rec = dict(
+        address_line_1=line1, address_line_2=line2, city=city,
+        state=state, postal_code=zipcode
+    )
+    if error:
+        raise UnParseableAddressError(None, None, addr_rec)
+    else:
+        return addr_rec
+
+
+def normalize_addr_dict(addr_dict, addr_map=None, addtl_funcs=None,
+                        strict=True):
+    # type: (Mapping[str, str]) -> Mapping[str, str]
+    """Normalize an address from dict or dict-like object.
+
+    Assumes addr_dict will have standard address related keys (address_line_1,
+    address_line_2, city, state, postal_code), unless addr_map is provided.
+
+    addr_map, if used, must be in the format {standard_key: custom_key} based
+    on standard address keys sighted above.
+
+    :param addr_dict: mapping containing address keys and values.
+    :type addr_dict: Mapping
+    :param addr_map: mapping of standard address fields to custom key names
+    :type addr_map: Mapping[str, str]
+    :param addtl_funcs: optional sequence of funcs that take string for further
+        processing and return line1 and line2 strings
+    :type addtl_funcs: Sequence[Callable[str, (str, str)]]
+    :param strict: bool indicating strict handling of components address parts
+        city, state and postal_code, vs city and state OR postal_code
+    :return: address dict with normalized, uppercase address values.
+    :rtype: Mapping[str, str]
+    """
+    if addr_map:
+        addr_dict = {key: addr_dict.get(val) for key, val in addr_map.items()}
+    addr_dict = validate_address_components(addr_dict, strict=strict)
+
+    # line 1 and line 2 elements are combined to ensure consistent processing
+    # whether the line 2 elements are pre-parsed or included in line 1
+    addr_str = get_addr_line_str(addr_dict, comma_separate=True)
+    postal_code = addr_dict.get('postal_code')
+    zipcode = validate_us_postal_code_format(
+        postal_code, addr_dict
+    ) if postal_code else None
+    city = addr_dict.get('city')
+    state = addr_dict.get('state')
+    try:
+        address = normalize_addr_str(
+            addr_str, city=city, state=state,
+            zipcode=zipcode, addtl_funcs=addtl_funcs
+        )
+    except AddressNormalizationError:
+        addr_str = get_addr_line_str(
+            addr_dict, comma_separate=True, addr_parts=ADDRESS_KEYS
+        )
+        address = normalize_addr_str(
+            addr_str, city=city, state=state,
+            zipcode=zipcode, addtl_funcs=addtl_funcs
+        )
+    return address
+
+
+def parse_address_string(addr_str):
+    # type: (str) -> MutableMapping[str, str]
+    """Separate an address string into its component parts per usaddress.
+
+    Attempts to parse addr_str into it's component parts, using usaddress.
+
+    If usaddress identifies the address type as Ambiguous or the resulting
+    OrderedDict includes any keys from AMBIGUOUS_LABELS that would constitute
+    ambiguous address in the SEED/GBR use case (ie: Recipient) then
+    an AmbiguousAddressError is raised.
+
+    :param addr_str: str address to be processed.
+    :type addr_str: str
+    :return: usaddress OrderedDict
+    :rtype: MutableMapping
+    """
+    parsed_results = usaddress.tag(addr_str)
+    parsed_addr = parsed_results[0]
+    # if the address is parseable but some form of ambiguity is found that
+    # may result in data corruption NormalizationError is raised.
+    if (parsed_results[1] == 'Ambiguous' or
+            any(key in AMBIGUOUS_LABELS for key in parsed_addr.keys())):
+        raise AmbiguousAddressError()
+    parsed_addr = handle_abnormal_occupancy(parsed_addr, addr_str)
+    return parsed_addr
+
+
+def handle_abnormal_occupancy(parsed_addr, addr_str):
+    """Handle abnormal occupancy abbreviations that are parsed as street type.
+
+    Evaluates addresses with an Occupancy or Subaddress identifier whose type
+    may be parsed into StreetNamePostType and swaps the StreetNamePostType tag
+    for the OccupancyType tag if necessary.
+
+    For example: Portland Maps uses 'UN' as an abbreviation for 'Unit' which
+    usaddress parses to 'StreetNamePostType' since 'UN' is correctly an
+    abbreviation for 'Union' street type.
+        123 MAIN UN => 123 MAIN UN
+        123 MAIN UN A => 123 MAIN, UNIT A
+        123 MAIN UN UN A => 123 MAIN UN, UNIT A
+
+    :param parsed_addr: address parsed into usaddress components
+    :type parsed_addr: OrderedDict
+    :param addr_str: Original address string
+    :type addr_str: str
+    :return: parsed address
+    :rtype: OrderedDict
+    """
+    occupancy_id_key = None
+    occupany_type_key = 'OccupancyType'
+    street_type_key = 'StreetNamePostType'
+    occupany_type_keys = (occupany_type_key, 'SubaddressType')
+    occupancy_identifier_keys = ('OccupancyIdentifier', 'SubaddressIdentifier')
+    street_type = parsed_addr.get(street_type_key)
+    if street_type in ABNORMAL_OCCUPANCY_ABBRVS:
+        occupancy_type = None
+        occupancy = None
+        for key in occupany_type_keys:
+            try:
+                occupancy_type = parsed_addr[key]
+                break
+            except KeyError:
+                pass
+        for key in occupancy_identifier_keys:
+            try:
+                occupancy = parsed_addr[key]
+                occupancy_id_key = key
+                break
+            except KeyError:
+                break
+        if occupancy and not occupancy_type:
+            if street_type in occupancy:
+                occupancy = occupancy.replace(street_type, '').strip()
+                del parsed_addr[occupancy_id_key]
+            else:
+                line2 = "{} {}".format(street_type, occupancy)
+                addr_str = addr_str.replace(line2, '')
+                parsed_addr = parse_address_string(addr_str)
+            parsed_addr.update({occupany_type_key: street_type})
+            parsed_addr.update({occupancy_id_key: occupancy})
+    return parsed_addr
+
+
+def get_parsed_values(parsed_addr, orig_val, val_label, orig_addr_str):
+    # type: (Mapping[str, str], str, str, str) -> Union[str, None]
+    """Get valid values from parsed_addr corresponding to val_label.
+
+    Retrieves values from parsed_addr corresponding to the label supplied in
+    val_label.
+    If a value for val_label is found in parsed_addr AND an orig_val is
+    supplied, a single string will be returned if the values match. If only
+    one of the two contains a non-null value.
+    If both values are empty, None is returned.
+    If the values an AmbiguousAddressError will be returned if the two values
+    are not equal. This provides a check against misidentified address
+    components when known values are available. (For example when a city is
+    supplied from the address dict or record being normalized, but usaddress
+    identifies extra information stored in address_line_1 as a PlaceName.)
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr: Mapping
+    :param orig_val: related value passed in from incoming data source.
+    :type orig_val: str
+    :param val_label: label to locate in parsed_addr
+    :type val_label: str
+    :param orig_addr_str: address string to pass to error, if applicable.
+    :type orig_addr_str: str
+    :return: str | None
+    """
+    val_from_parse = parsed_addr.get(val_label)
+    orig_val = post_clean_addr_str(orig_val)
+    val_from_parse = post_clean_addr_str(val_from_parse)
+    non_null_val_set = {orig_val, val_from_parse} - {None}
+    if len(non_null_val_set) > 1:
+        raise AmbiguousAddressError(None, None, orig_addr_str)
+    else:
+        return non_null_val_set.pop() if non_null_val_set else None
+
+
+def normalize_address_components(parsed_addr):
+    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
+    """Normalize parsed sections of address as appropriate.
+
+    Processes parsed address through subsets of normalization rules.
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr:Mapping
+    :return: parsed_addr with normalization processing applied to elements.
+    :rtype: dict
+    """
+    parsed_addr = normalize_numbered_streets(parsed_addr)
+    parsed_addr = normalize_directionals(parsed_addr)
+    parsed_addr = normalize_street_types(parsed_addr)
+    parsed_addr = normalize_occupancy_type(parsed_addr)
+    return parsed_addr
+
+
+def normalize_numbered_streets(parsed_addr):
+    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
+    """Change numbered street names to include missing original identifiers.
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr: Mapping
+    :return: parsed_addr with ordinal identifiers appended to numbered streets.
+    :rtype: dict"""
+    street_tags = ['StreetName', 'SecondStreetName']
+    for tag in street_tags:
+        post_type_tag = '{}PostType'.format(tag)
+        # limits updates to numbered street names that include a post street
+        # type, since an ordinal indicator would be inappropriate for some
+        # numbered streets (ie. Country Road 97).
+        if tag in parsed_addr.keys() and post_type_tag in parsed_addr.keys():
+            try:
+                cardinal = int(parsed_addr[tag])
+                ord_indicator = get_ordinal_indicator(cardinal)
+                parsed_addr[tag] = '{}{}'.format(cardinal, ord_indicator)
+            except ValueError:
+                pass
+    return parsed_addr
+
+
+def normalize_directionals(parsed_addr):
+    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
+    """Change directional notations to standard abbreviations.
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr: Mapping
+    :return: parsed_addr with directionals updated to abbreviated format.
+    :rtype: dict
+    """
+    # get the directional related keys from the current address.
+    found_directional_tags = (
+        tag for tag in parsed_addr.keys() if 'Directional' in tag
+    )
+    for found in found_directional_tags:
+        # get the original directional related value per key.
+        dir_str = parsed_addr[found]
+        # remove spaces, punctuation, hyphens etc so two part directions
+        # conform to a single word standard. Convert to upper case
+        dir_str = clean_upper(
+            dir_str, exclude=[], removal_cats=STRIP_ALL_CATS, strip_spaces=True
+        )
+        if dir_str in DIRECTIONAL_REPLACEMENTS.keys():
+            parsed_addr[found] = DIRECTIONAL_REPLACEMENTS[dir_str]
+    return parsed_addr
+
+
+def normalize_street_types(parsed_addr):
+    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
+    """Change street types to accepted abbreviated format.
+
+    No change is made if street types do not conform to common usages per
+    USPS pub 28 appendix C.
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr: Mapping
+    :return: parsed_addr with street types updated to abbreviated format.
+    :rtype: dict
+    """
+    # get the *Street*Type keys from the current parsed address.
+    found_type_tags = (
+        tag for tag in parsed_addr.keys() if 'Street' in tag and 'Type' in tag
+    )
+    for found in found_type_tags:
+        # lookup the appropriate abbrev for the street type found per key.
+        type_abbr = STREET_TYPE_ABBREVIATIONS.get(parsed_addr[found])
+        # update the street type only if a new abbreviation is found.
+        if type_abbr:
+            parsed_addr[found] = type_abbr
+    return parsed_addr
+
+
+def normalize_occupancy_type(parsed_addr, default=None):
+    # type: (MutableMapping[str, str]) -> MutableMapping[str, str]
+    """Change occupancy types to accepted abbreviated format.
+
+    If there is an occupancy and it does not conform to one of the
+    OCCUPANCY_TYPE_ABBREVIATIONS, occupancy is changed to the generic 'UNIT'.
+    OCCUPANCY_TYPE_ABBREVIATIONS contains common abbreviations per
+    USPS pub 28 appendix C, however, OCCUPANCY_TYPE_ABBREVIATIONS can be
+    customized to allow alternate abbreviations to pass through. (see README)
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :type parsed_addr: Mapping
+    :param default: default abbreviation to use for types that fall outside the
+     standard abbreviations. Default is 'UNIT'
+    :return: parsed_addr with occupancy types updated to abbreviated format.
+    :rtype: dict
+    """
+    default = default if default is not None else 'UNIT'
+    occupancy_type_label = 'OccupancyType'
+    occupancy_type = parsed_addr.pop(occupancy_type_label, None)
+    occupancy_type_abbr = (
+        occupancy_type
+        if occupancy_type in OCCUPANCY_TYPE_ABBREVIATIONS.values()
+        else OCCUPANCY_TYPE_ABBREVIATIONS.get(occupancy_type)
+    )
+    occupancy_id = parsed_addr.get('OccupancyIdentifier')
+    if ((occupancy_id and not occupancy_id.startswith('#'))
+            and not occupancy_type_abbr):
+        occupancy_type_abbr = default
+    if occupancy_type_abbr:
+        parsed_list = list(parsed_addr.items())
+        try:
+            index = parsed_list.index(('OccupancyIdentifier', occupancy_id))
+        except ValueError:
+            msg = (
+                'Address has an occupancy type (ie: Apt, Unit, etc) '
+                'but no occupancy identifier (ie: 101, A, etc)'
+            )
+            raise AddressNormalizationError(msg)
+        parsed_list.insert(index, (occupancy_type_label, occupancy_type_abbr))
+        parsed_addr = OrderedDict(parsed_list)
+    return parsed_addr
+
+
+def normalize_state(state):
+    # type: (Union[str, None]) -> Union[str, None]
+    """Change state string to accepted abbreviated format.
+
+    :param state: string containing state name or abbreviation.
+    :type state: str | None
+    :return: 2 char state abbreviation, or original state string if not found
+        in state names or standard long abbreviations.
+    :rtype: str | None
+    """
+    if state:
+        state_abbrv = STATE_ABBREVIATIONS.get(state.upper())
+        if state_abbrv:
+            state = state_abbrv
+    return state
+
+
+def get_normalized_line_segment(parsed_addr, line_labels):
+    # type: (Mapping[str, str], Sequence[str]) -> str
+    """
+
+    :param parsed_addr: address parsed into ordereddict per usaddress.
+    :param line_labels: tuple of str labels of all the potential keys related
+        to the desired address segment (ie address_line_1 or address_line_2).
+    :return: s/r joined values from parsed_addr corresponding to given labels.
+    """
+    line_elems = [
+        elem for key, elem in parsed_addr.items() if key in line_labels
+    ]
+    line_str = ' '.join(line_elems) if line_elems else None
+    return post_clean_addr_str(line_str)
+
+
+def get_addr_line_str(addr_dict, addr_parts=None, comma_separate=False):
+    # type: (Mapping[str, str], Optional[Sequence], bool) -> str
+    """Get address 'line' elements as a single string.
+
+    Combines 'address_line_1' and 'address_line_2' elements as a single string
+    to ensure no data is lost and line_2 can be processed according to a
+    standard set of rules.
+
+    :param addr_dict: dict containing keys 'address_line_1', 'address_line_2'.
+    :type addr_dict: Mapping
+    :param addr_parts: optional sequence of address elements
+    :type addr_parts:
+    :param comma_separate: optional boolean to separate dict values by comma
+        useful for dealing with potentially ambiguous line 2 segments
+    :type bool:
+    :return: string combining 'address_line_1' & 'address_line_2' values.
+    :rtype: str
+    """
+    if not addr_parts:
+        addr_parts = ['address_line_1', 'address_line_2']
+    if not isinstance(addr_parts, (list, tuple)):
+        raise TypeError('addr_parts must be a list or tuple')
+    separator = ', ' if comma_separate else ' '
+    addr_str = separator.join(
+        str(addr_dict[elem]) for elem in addr_parts if addr_dict.get(elem)
+    )
+    return addr_str
+
+
+def format_address_record(address):
+    # type AddressRecord -> str
+    """Format AddressRecord as string."""
+    address_template = Template('$address')
+    address = dict(address)
+    addr_parts = [
+        str(address[field]) for field in ADDRESS_KEYS if address.get(field)
+    ]
+    return address_template.safe_substitute(address=', '.join(addr_parts))
+
+
+def get_geocoder_normalized_addr(address, addr_keys=ADDRESS_KEYS):
+    # type: (Union[Mapping, str], Optional[Sequence]) -> dict
+    """Get geocoder normalized address parsed to dict with addr_keys.
+
+    :param address: string or dict-like containing address data
+    :param addr_keys: optional list of address keys. standard list of keys will
+        be used if not supplied
+    :return: dict containing geocoder address result
+    """
+    address_line_2 = None
+    geo_addr_dict = {}
+    if not isinstance(address, str):
+        address_line_2 = address.get('address_line_2')
+        address = get_addr_line_str(address, addr_parts=addr_keys)
+    geo_resp = geocoder.google(address)
+    if geo_resp.ok and geo_resp.housenumber:
+        line2 = geo_resp.subpremise or address_line_2
+        geo_addr_dict = {
+            'address_line_1':
+                ' '.join([geo_resp.housenumber, geo_resp.street]),
+            'address_line_2': strip_occupancy_type(line2),
+            'city': geo_resp.city,
+            'state': geo_resp.state,
+            'postal_code': geo_resp.postal
+        }
+        for key, value in geo_addr_dict.items():
+            geo_addr_dict[key] = value.upper() if value else None
+    return geo_addr_dict
+
+
+def get_ordinal_indicator(number):
+    # type: (int) -> str
+    """Get the ordinal indicator suffix applicable to the supplied number.
+
+     Ordinal numbers are words representing position or rank in a sequential
+     order (1st, 2nd, 3rd, etc).
+     Ordinal indicators are the suffix characters (st, nd, rd, th) that, when
+     applied to a numeral (int), denote that it an ordinal number.
+
+    :param number: int
+    :type: int
+    :return: ordinal indicator appropriate to the number supplied.
+    :rtype: str
+    """
+    str_num = str(number)
+    digits = len(str_num)
+    if str_num[-1] == '1' and not (digits >= 2 and str_num[-2:] == '11'):
+        return 'st'
+    elif str_num[-1] == '2' and not (digits >= 2 and str_num[-2:] == '12'):
+        return 'nd'
+    elif str_num[-1] == '3' and not (digits >= 2 and str_num[-2:] == '13'):
+        return 'rd'
+    else:
+        return 'th'
+
+
+class NormalizeAddress(object):
+    parse_address_string = staticmethod(parse_address_string)
+    pre_clean_addr_str = staticmethod(pre_clean_addr_str)
+    post_clean_addr_str = staticmethod(post_clean_addr_str)
+    format_address_record = staticmethod(format_address_record)
+    normalize_address_components = staticmethod(normalize_address_components)
+    get_parsed_values = staticmethod(get_parsed_values)
+
+    def __init__(self, address, addr_map=None, addtl_funcs=None, strict=None):
+        self.address = address
+        self.addr_map = addr_map
+        self.addtl_funcs = addtl_funcs
+        self.strict = True if strict is None else strict
+
+    def normalize(self):
+        if isinstance(self.address, str):
+            return self.normalize_addr_str(
+                self.address, addtl_funcs=self.addtl_funcs
+            )
+        else:
+            return self.normalize_addr_dict(
+                self.address, addr_map=self.addr_map,
+                addtl_funcs=self.addtl_funcs, strict=self.strict
+            )
+
+    def normalize_addr_str(self, addr_str,  # type: str
+                           line2=None,  # type: Optional[str]
+                           city=None,  # type: Optional[str]
+                           state=None,  # type: Optional[str]
+                           zipcode=None,  # type: Optional[str]
+                           addtl_funcs=None
+                           # type: Sequence[Callable[[str,str], str]]  # noqa
+                           ):  # noqa
+        # get address parsed into usaddress components.
+        error = None
+        parsed_addr = None
+        addr_str = self.pre_clean_addr_str(addr_str, normalize_state(state))
+        try:
+            parsed_addr = self.parse_address_string(addr_str)
+        except (usaddress.RepeatedLabelError, AmbiguousAddressError) as err:
+            error = err
+            if not line2 and self.addtl_funcs:
+                for func in self.addtl_funcs:
+                    try:
+                        line1, line2 = func(addr_str)
+                        error = False
+                        # send refactored line_1 and line_2 back through
+                        # processing
+                        return self.normalize_addr_str(
+                            line1, line2=line2,
+                            city=city,
+                            state=state, zipcode=zipcode
+                        )
+                    except ValueError:
+                        # try a different additional processing function
+                        pass
+
+        if parsed_addr and not parsed_addr.get('StreetName'):
+            addr_dict = dict(
+                address_line_1=addr_str, address_line_2=line2, city=city,
+                state=state, postal_code=zipcode
+            )
+            full_addr = self.format_address_record(addr_dict)
+            try:
+                parsed_addr = self.parse_address_string(full_addr)
+            except (usaddress.RepeatedLabelError,
+                    AmbiguousAddressError) as err:
+                parsed_addr = None
+                error = err
+
+        if parsed_addr:
+            parsed_addr = self.normalize_address_components(parsed_addr)
+            zipcode = self.get_parsed_values(
+                parsed_addr, zipcode, 'ZipCode', addr_str
+            )
+            city = self.get_parsed_values(
+                parsed_addr, city, 'PlaceName', addr_str
+            )
+            state = self.get_parsed_values(
+                parsed_addr, state, 'StateName', addr_str
+            )
+            state = normalize_state(state)
+
+            # assumes if line2 is passed in that it need not be parsed from
+            # addr_str. Primarily used to allow advanced processing of
+            # otherwise unparsable addresses.
+            line2 = line2 if line2 else get_normalized_line_segment(
+                parsed_addr, LINE2_USADDRESS_LABELS
+            )
+            line2 = self.post_clean_addr_str(line2)
+            # line 1 is fully post cleaned in get_normalized_line_segment.
+            line1 = get_normalized_line_segment(
+                parsed_addr, LINE1_USADDRESS_LABELS
+            )
+            validate_parens_groups_parsed(line1)
+        else:
+            # line1 is set to addr_str so complete dict can be passed to error.
+            line1 = addr_str
+
+        addr_rec = dict(
+            address_line_1=line1, address_line_2=line2, city=city,
+            state=state, postal_code=zipcode
+        )
+        if error:
+            raise UnParseableAddressError(None, None, addr_rec)
+        else:
+            return addr_rec
+
+    def normalize_addr_dict(self, addr_dict, addr_map=None, addtl_funcs=None,
+                            strict=True):
+        if addr_map:
+            addr_dict = {key: addr_dict.get(val) for key, val in
+                         addr_map.items()}
+        addr_dict = validate_address_components(addr_dict, strict=strict)
+
+        # line 1 and line 2 elements are combined to ensure consistent
+        # processing whether the line 2 elements are pre-parsed or
+        # included in line 1
+        addr_str = get_addr_line_str(addr_dict, comma_separate=True)
+        postal_code = addr_dict.get('postal_code')
+        zipcode = validate_us_postal_code_format(
+            postal_code, addr_dict
+        ) if postal_code else None
+        city = addr_dict.get('city')
+        state = addr_dict.get('state')
+        try:
+            address = self.normalize_addr_str(
+                addr_str, city=city, state=state,
+                zipcode=zipcode, addtl_funcs=addtl_funcs
+            )
+        except AddressNormalizationError:
+            addr_str = get_addr_line_str(
+                addr_dict, comma_separate=True, addr_parts=ADDRESS_KEYS
+            )
+            address = self.normalize_addr_str(
+                addr_str, city=city, state=state,
+                zipcode=zipcode, addtl_funcs=addtl_funcs
+            )
+        return address
```

### Comparing `usaddress-scourgify-0.2.4/scourgify/tests/test_address_normalization.py` & `usaddress-scourgify-0.3.0/scourgify/tests/test_address_normalization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,760 +1,786 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-copyright (c) 2016-2019 Earth Advantage.
-All rights reserved
-
-Unit tests for scourgify.
-"""
-
-# Imports from Standard Library
-from collections import OrderedDict
-from unittest import TestCase, mock
-
-# Imports from Third Party Modules
-from yamlconf import ConfigError
-
-# Local Imports
-from scourgify import address_constants
-from scourgify.cleaning import (
-    clean_ambiguous_street_types,
-    clean_period_char,
-    post_clean_addr_str,
-    pre_clean_addr_str,
-)
-from scourgify.exceptions import (
-    AddressNormalizationError,
-    AddressValidationError,
-    AmbiguousAddressError,
-    IncompleteAddressError,
-    UnParseableAddressError,
-)
-from scourgify.normalize import (
-    get_addr_line_str,
-    get_geocoder_normalized_addr,
-    get_normalized_line_segment,
-    get_ordinal_indicator,
-    get_parsed_values,
-    normalize_addr_dict,
-    normalize_addr_str,
-    normalize_address_record,
-    normalize_directionals,
-    normalize_numbered_streets,
-    normalize_occupancy_type,
-    normalize_state,
-    normalize_street_types,
-    parse_address_string,
-)
-from scourgify.validations import (
-    validate_address_components,
-    validate_parens_groups_parsed,
-    validate_us_postal_code_format,
-)
-
-# Constants
-SERVICE = 'GBR Test Normalization'
-# Helper Functions & Classes
-
-
-# Tests
-class TestAddressNormalization(TestCase):
-    """Unit tests for scourgify"""
-    # pylint:disable=too-many-arguments
-
-    def setUp(self):
-        """setUp"""
-        self.expected = dict(
-            address_line_1='123 NOWHERE ST',
-            address_line_2='STE 0',
-            city='BORING',
-            state='OR',
-            postal_code='97009'
-        )
-        self.address_dict = dict(
-            address_line_1='123 Nowhere St',
-            address_line_2='Suite 0',
-            city='Boring',
-            state='OR',
-            postal_code='97009'
-        )
-
-        self.ordinal_addr = dict(
-            address_line_1='4333 NE 113th',
-            city='Boring',
-            state='OR',
-            postal_code='97009'
-        )
-        self.ordinal_expected = dict(
-            address_line_1='4333 NE 113TH',
-            address_line_2=None,
-            city='BORING',
-            state='OR',
-            postal_code='97009'
-        )
-        self.parseable_addr_str = '123 Nowhere Street Suite 0 Boring OR 97009'
-        self.parsed_addr = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetName', 'NOWHERE'),
-            ('StreetNamePostType', 'STREET'),
-            ('OccupancyType', 'SUITE'),
-            ('OccupancyIdentifier', '0'),
-            ('PlaceName', 'BORING'),
-            ('StateName', 'OR'),
-            ('ZipCode', '97009')
-        ])
-        self.unparesable_addr_str = '6000 SW 1000TH AVE  (BLDG  A5 RIGHT)'
-
-    def test_normalize_address_record(self):
-        """Test normalize_address_record function."""
-        result = normalize_address_record(self.parseable_addr_str)
-        self.assertDictEqual(self.expected, result)
-
-        result = normalize_address_record(self.address_dict)
-        self.assertDictEqual(self.expected, result)
-
-        result = normalize_address_record(self.ordinal_addr)
-        self.assertDictEqual(self.ordinal_expected, result)
-
-    def test_normalize_addr_str(self):
-        """Test normalize_addr_str function."""
-        result = normalize_addr_str(self.parseable_addr_str)
-        self.assertDictEqual(self.expected, result)
-
-        broken_line1 = '6000 SW 1000TH AVE '
-        broken_line2 = '(BLDG  A1 RIGHT)'
-        result = normalize_addr_str(
-            broken_line1, line2=broken_line2,
-            city='Portland', state='OR', zipcode='97203'
-        )
-        expected = {
-            'address_line_1': '6000 SW 1000TH AVE',
-            'address_line_2': 'BLDG A1 RIGHT',
-            'state': 'OR', 'city': 'PORTLAND',
-            'postal_code': '97203'
-        }
-        self.assertDictEqual(expected, result)
-
-        def addtl_test_func(addr_str):
-            if 'BLDG A1' in addr_str:
-                return '123 NOWHERE STREET', 'BLDG A1 RIGHT'
-            else:
-                raise ValueError
-
-        addtl_processing = '123 Nowhere Street (BLDG A1 RIGHT)'
-        expected = {
-            'address_line_1': '123 NOWHERE ST',
-            'address_line_2': 'BLDG A1 RIGHT',
-            'state': 'OR', 'city': 'PORTLAND',
-            'postal_code': '97203'
-        }
-        result = normalize_addr_str(
-            addtl_processing, city='Portland', state='OR', zipcode='97203',
-            addtl_funcs=[addtl_test_func]
-        )
-        self.assertDictEqual(expected, result)
-
-        self.assertRaises(
-            UnParseableAddressError,
-            normalize_addr_str,
-            self.unparesable_addr_str,
-            city='Portland', state='OR', zipcode='97203',
-            addtl_funcs=[addtl_test_func]
-
-        )
-
-    def test_normalize_addr_dict(self):
-        """Test normalize_addr_dict function."""
-        result = normalize_addr_dict(self.address_dict)
-        self.assertDictEqual(self.expected, result)
-
-        alternate_dict = dict(
-            address1='123 Nowhere St',
-            address2='Suite 0',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        dict_map = {
-            'address_line_1': 'address1',
-            'address_line_2': 'address2',
-            'city': 'city',
-            'state': 'state',
-            'postal_code': 'zip'
-        }
-        result = normalize_addr_dict(alternate_dict, addr_map=dict_map)
-        self.assertDictEqual(self.expected, result)
-
-    def test_parse_address_string(self):
-        """Test parse_address_string function."""
-        result = parse_address_string(self.parseable_addr_str)
-        self.assertIsInstance(result, OrderedDict)
-
-        ambig_addr_str = 'AWBREY VILLAGE'
-        with self.assertRaises(AmbiguousAddressError):
-            parse_address_string(ambig_addr_str)
-
-    def test_normalize_occupancies(self):
-        """Test normalize_addr_dict function with handling for occupancy
-        type oddities.  This is based on a real life incident; the original
-        behavior to allow non-standard unit types to pass through resulted
-        in an address validation service also allowing the address to pass
-        through even though no unit should have existed on the home.
-        """
-        dict_map = {
-            'address_line_1': 'address1',
-            'address_line_2': 'address2',
-            'city': 'city',
-            'state': 'state',
-            'postal_code': 'zip'
-        }
-
-        weird_unit = dict(
-            address1='123 Nowhere St',
-            address2='Ave 345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        expected = dict(
-            address_line_1='123 NOWHERE ST',
-            address_line_2='UNIT 345',
-            city='BORING',
-            state='OR',
-            postal_code='97009'
-        )
-        result = normalize_addr_dict(weird_unit, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-        late_unit_add = dict(
-            address1='123 Nowhere St',
-            address2='345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        result = normalize_addr_dict(late_unit_add, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-        expected = dict(
-            address_line_1='123 NOWHERE ST',
-            address_line_2='# 345',
-            city='BORING',
-            state='OR',
-            postal_code='97009'
-        )
-
-        hashtag_unit = dict(
-            address1='123 Nowhere St',
-            address2='# 345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        result = normalize_addr_dict(hashtag_unit, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-        hashtag_unit = dict(
-            address1='123 Nowhere St',
-            address2='#345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        result = normalize_addr_dict(hashtag_unit, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-        expected = dict(
-            address_line_1='123 NOWHERE ST',
-            address_line_2='APT 345',
-            city='BORING',
-            state='OR',
-            postal_code='97009'
-        )
-
-        abbreviation = dict(
-            address1='123 Nowhere St',
-            address2='Apt 345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        result = normalize_addr_dict(abbreviation, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-        full_name = dict(
-            address1='123 Nowhere St',
-            address2='Apartment 345',
-            city='Boring',
-            state='OR',
-            zip='97009'
-        )
-        result = normalize_addr_dict(full_name, addr_map=dict_map)
-        self.assertDictEqual(expected, result)
-
-
-class TestAddressNormalizationUtils(TestCase):
-    """Unit tests for scourgify utils"""
-
-    def setUp(self):
-
-        self.address_dict = dict(
-            address_line_1='123 Nowhere St',
-            address_line_2='Suite 0',
-            city='Boring',
-            state='OR',
-            postal_code='97009'
-        )
-        self.parseable_addr = '123 Nowhere Street Suite 0 Boring OR 97009'
-        self.parsed_addr = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetName', 'NOWHERE'),
-            ('StreetNamePostType', 'STREET'),
-            ('OccupancyType', 'SUITE'),
-            ('OccupancyIdentifier', '0'),
-            ('PlaceName', 'BORING'),
-            ('StateName', 'OR'),
-            ('ZipCode', '97009')
-        ])
-
-        self.unparesable_addr = '6000 SW 1000TH AVE  (BLDG  A1 RIGHT)'
-
-        self.unparesable_addr_dict = OrderedDict([
-            ('AddressNumber', '6000'),
-            ('StreetNamePreDirectional', 'SW'),
-            ('StreetName', '1000TH'),
-            ('StreetNamePostType', 'AVE'),
-            ('SubaddressType', 'BLDG'),
-            ('SubaddressIdentifier', 'A1'),
-            ('SubaddressType', 'RIGHT')
-        ])
-
-    def test_get_parsed_values(self):
-        """Test get_parsed_values function."""
-        expected = 'BORING'
-        result = get_parsed_values(self.parsed_addr, 'Boring',
-                                   'PlaceName', self.parseable_addr)
-        self.assertEqual(expected, result)
-
-        expected = 'ONE VALUE PRESENT'
-        result = get_parsed_values(self.parsed_addr, 'One Value Present',
-                                   'LandmarkName', self.parseable_addr)
-        self.assertEqual(expected, result)
-
-        result = get_parsed_values(self.parsed_addr, None,
-                                   'LandmarkName', self.parseable_addr)
-        self.assertIsNone(result)
-
-        with self.assertRaises(AmbiguousAddressError):
-            get_parsed_values(self.parsed_addr, 'UnMatched City',
-                              'PlaceName', self.parseable_addr)
-
-    def test_get_norm_line_segment(self):
-        """Test get normalized_line_segment function."""
-        result = get_normalized_line_segment(self.parsed_addr,
-                                             ['StreetName', 'AddressNumber'])
-        expected = '{} {}'.format(self.parsed_addr['AddressNumber'],
-                                  self.parsed_addr['StreetName'])
-        self.assertEqual(expected, result)
-
-        result = get_normalized_line_segment(
-            self.parsed_addr,
-            ['StreetName', 'StreetNamePostType', 'IntersectionSeparator']
-        )
-        expected = '{} {}'.format(self.parsed_addr['StreetName'],
-                                  self.parsed_addr['StreetNamePostType'])
-        self.assertEqual(expected, result)
-
-    def test_normalize_numbered_streets(self):
-        """Test normalize_numbered_streets function."""
-        numbered_addr = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetName', '100'),
-            ('StreetNamePostType', 'STREET')
-        ])
-        county_road = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreType', 'COUNTY ROAD'),
-            ('StreetName', '100')
-        ])
-        string_addr = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetName', '91st'),
-            ('StreetNamePostType', 'STREET')
-        ])
-
-        expected = '{}{}'.format(
-            numbered_addr['StreetName'], 'th'
-        )
-        result = normalize_numbered_streets(numbered_addr)
-        self.assertEqual(expected, result['StreetName'])
-
-        result = normalize_numbered_streets(county_road)
-        self.assertDictEqual(county_road, result)
-
-        result = normalize_numbered_streets(string_addr)
-        self.assertDictEqual(string_addr, result)
-
-    def test_normalize_directionals(self):
-        """Test normalize_directionals function."""
-        unabbr_directional = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'South West', ),
-            ('StreetName', '100'),
-            ('StreetNamePostType', 'STREET')
-        ])
-        abbrev_directional = OrderedDict([
-            ('AddressNumber', '123'),
-            ('SW', 'StreetNamePreDirectional'),
-            ('StreetNamePreType', 'COUNTY ROAD'),
-            ('StreetName', '100')
-        ])
-        no_directional = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetName', '91st'),
-            ('StreetNamePostType', 'STREET')
-        ])
-
-        expected = 'SW'
-        result = normalize_directionals(unabbr_directional)
-        self.assertEqual(expected, result['StreetNamePreDirectional'])
-
-        result = normalize_directionals(abbrev_directional)
-        self.assertDictEqual(abbrev_directional, result)
-
-        result = normalize_directionals(no_directional)
-        self.assertDictEqual(no_directional, result)
-
-    def test_normalize_street_types(self):
-        """Test normalize_street_types function."""
-        unabbr_type = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW', ),
-            ('StreetName', 'MAIN'),
-            ('StreetNamePostType', 'STREET')
-        ])
-        abbrev_type = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW', ),
-            ('StreetName', 'MAIN'),
-            ('StreetNamePostType', 'AVE')
-        ])
-        typo_type = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW', ),
-            ('StreetName', 'MAIN'),
-            ('StreetNamePostType', 'STROET')
-        ])
-        no_type = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW', ),
-            ('StreetName', 'MAIN'),
-        ])
-
-        expected = 'ST'
-        result = normalize_street_types(unabbr_type)
-        self.assertEqual(expected, result['StreetNamePostType'])
-
-        result = normalize_street_types(abbrev_type)
-        self.assertDictEqual(abbrev_type, result)
-
-        result = normalize_street_types(typo_type)
-        self.assertDictEqual(typo_type, result)
-
-        result = normalize_street_types(no_type)
-        self.assertDictEqual(no_type, result)
-
-    def test_normalize_occupancy_type(self):
-        """Test normalize_occupancy_type function."""
-        expected = 'STE'
-        result = normalize_occupancy_type(self.parsed_addr)
-        self.assertEqual(expected, result['OccupancyType'])
-
-    def test_normalize_state(self):
-        """Test normalize_state function"""
-        state = 'ore'
-        expected = 'OR'
-        result = normalize_state(state)
-        self.assertEqual(expected, result)
-
-        state = 'oregano'
-        expected = state
-        result = normalize_state(state)
-        self.assertEqual(expected, result)
-
-        self.assertIsNone(normalize_state(None))
-
-    def test_pre_clean_addr_str(self):
-        """Test pre_clean_addr_str function"""
-        odd_addr = '123 Nowhere    Street, Suite 0; @Boring OR 97009'
-        # we're leaving commas in the pre-clean until norm can be revisited
-        expected = '123 Nowhere Street, Suite 0 Boring OR 97009'.upper()
-        # expected = '123 Nowhere Street Suite 0 Boring OR 97009'.upper()
-        result = pre_clean_addr_str(odd_addr)
-        self.assertEqual(expected, result)
-
-    def test_post_clean_addr_str(self):
-        """Test post_clean_addr_str function."""
-        addr_str = '(100-104) SW NO   WHERE st'
-        expected = '100-104 SW NO WHERE ST'
-        result = post_clean_addr_str(addr_str)
-        self.assertEqual(expected, result)
-
-        self.assertIsNone(post_clean_addr_str(None))
-        self.assertEqual('', post_clean_addr_str(''))
-
-    def test_validate_address(self):
-        """Test validate_address_components function."""
-        expected = self.address_dict
-        result = validate_address_components(self.address_dict)
-        self.assertEqual(expected, result)
-
-        minus_line1 = dict(
-            address_line_1=None,
-            address_line_2='Suite 0',
-            city='Boring',
-            state='OR',
-            postal_code='97009'
-        )
-        with self.assertRaises(IncompleteAddressError):
-            validate_address_components(minus_line1)
-
-        minus_zip = dict(
-            address_line_1='123 NoWhere St',
-            address_line_2='Suite 0',
-            city='Boring',
-            state='OR',
-            postal_code=None
-        )
-        with self.assertRaises(IncompleteAddressError):
-            validate_address_components(minus_zip)
-
-        minus_city_state = dict(
-            address_line_1='123 NoWhere St',
-            address_line_2='Suite 0',
-            city=None,
-            state=None,
-            postal_code='97009'
-        )
-
-        with self.assertRaises(IncompleteAddressError):
-            validate_address_components(minus_city_state)
-
-        minus_city_state_zip = dict(
-            address_line_1='123 NoWhere St',
-            address_line_2='Suite 0',
-            city=None,
-            state=None,
-            postal_code=None
-        )
-        with self.assertRaises(IncompleteAddressError):
-            validate_address_components(minus_city_state_zip)
-
-    def test_validate_postal_code(self):
-        """Test validate_us_postal_code_format"""
-
-        with self.assertRaises(AddressValidationError):
-            zip_plus = '97219-0001-00'
-            validate_us_postal_code_format(zip_plus, self.address_dict)
-
-        with self.assertRaises(AddressValidationError):
-            zip_plus = '97219-00'
-            validate_us_postal_code_format(zip_plus, self.address_dict)
-
-        with self.assertRaises(AddressValidationError):
-            zip_plus = '972-0001'
-            validate_us_postal_code_format(zip_plus, self.address_dict)
-
-        with self.assertRaises(AddressValidationError):
-            zip_five = '9721900'
-            validate_us_postal_code_format(zip_five, self.address_dict)
-
-        with self.assertRaises(AddressValidationError):
-            zip_five = '972'
-            validate_us_postal_code_format(zip_five, self.address_dict)
-
-        expected = '97219'
-        result = validate_us_postal_code_format(expected, self.address_dict)
-        self.assertEqual(expected, result)
-
-    def test_get_addr_line_str(self):
-        """Test get_addr_line_str function."""
-        expected = '{} {}'.format(
-            self.address_dict['address_line_1'],
-            self.address_dict['address_line_2']
-        )
-        result = get_addr_line_str(self.address_dict)
-        self.assertEqual(expected, result)
-
-        no_line_2 = {
-            'address_line_1': 'address line 1'
-        }
-        expected = no_line_2['address_line_1']
-        result = get_addr_line_str(no_line_2)
-        self.assertEqual(expected, result)
-
-        empty_line_2 = {
-            'address_line_1': 'address line 1',
-            'address_line_2': None
-        }
-        expected = no_line_2['address_line_1']
-        result = get_addr_line_str(empty_line_2)
-        self.assertEqual(expected, result)
-
-        with self.assertRaises(TypeError):
-            get_addr_line_str(self.address_dict, addr_parts='line1')
-
-    @mock.patch(
-        'scourgify.normalize.geocoder'
-    )
-    def test_get_geocoder_normalized_addr(self, mock_geocoder):
-        """Test get_geocoder_normalized_addr"""
-        geo_addr = mock.MagicMock()
-        geo_addr.ok = True
-        geo_addr.housenumber = '1234'
-        geo_addr.street = "Main"
-        geo_addr.subpremise = ''
-        geo_addr.city = 'Boring'
-        geo_addr.state = 'OR'
-        geo_addr.postal = '97000'
-
-        mock_geocoder.google.return_value = geo_addr
-
-        address = {
-            'address_line_1': '1234 Main',
-            'address_line_2': None,
-            'city': 'Boring',
-            'state': 'OR',
-            'postal_code': '97000'
-        }
-        addr_str_return_value = "1234 Main Boring OR 97000"
-        get_geocoder_normalized_addr(address)
-        mock_geocoder.google.assert_called_with(addr_str_return_value)
-
-    def test_get_ordinal_indicator(self):
-        """Test get_ordinal_indicator"""
-        result = get_ordinal_indicator(11)
-        expected = 'th'
-        self.assertEqual(expected, result)
-
-        result = get_ordinal_indicator(112)
-        self.assertEqual(expected, result)
-
-        result = get_ordinal_indicator(3113)
-        self.assertEqual(expected, result)
-
-        result = get_ordinal_indicator(1)
-        expected = 'st'
-        self.assertEqual(expected, result)
-
-        result = get_ordinal_indicator(22)
-        expected = 'nd'
-        self.assertEqual(expected, result)
-
-        result = get_ordinal_indicator(31243)
-        expected = 'rd'
-        self.assertEqual(expected, result)
-
-    def test_clean_period_char(self):
-        """Test clean_period_char"""
-        text = "49.5 blah.blah."
-        expected = "49.5 blahblah"
-        result = clean_period_char(text)
-        self.assertEqual(expected, result)
-
-    def test_validate_parens_group_parsed(self):
-        """Test validate_parens_groups_parsed"""
-        broken_line1 = '6000 SW 1000TH AVE'
-        result = validate_parens_groups_parsed(broken_line1)
-        self.assertEqual(broken_line1, result)
-
-        bad_addr = '10000 NE 8TH (ROW HOUSE)'
-        with self.assertRaises(AmbiguousAddressError):
-            validate_parens_groups_parsed(bad_addr)
-
-    def test_clean_ambiguous_street_types(self):
-        """ Test clean_ambiguous_street_types"""
-        problem_addr = "1234 BROKEN CT"
-        expected = "1234 BROKEN COURT"
-        result = clean_ambiguous_street_types(problem_addr)
-        self.assertEqual(expected, result)
-
-        normal_addr = "1234 NORMAL ST"
-        result = clean_ambiguous_street_types(normal_addr)
-        self.assertEqual(normal_addr, result)
-
-    def test_address_normalization_error(self):
-        error_msg = 'Error Message'
-        error_title = 'ERROR TITLE'
-        addtl_args = 'Addition info'
-        expected = "{}: {}, {}".format(error_title, error_msg, addtl_args)
-        error = AddressNormalizationError(error_msg, error_title, addtl_args)
-        self.assertEqual(expected, str(error))
-
-    @mock.patch.object(address_constants.NormalizationConfig, 'get')
-    def test_set_constants(self, mock_config_get):
-        new_addr_keys = ['new keys']
-        new_problem_st = {
-            "PS": 'STREET'
-        }
-        mock_config_get.side_effect = (
-            'update', new_addr_keys,
-            None, None, None, None, None,
-            new_problem_st
-        )
-        address_constants.set_address_constants()
-        self.assertEqual(address_constants.ADDRESS_KEYS, new_addr_keys)
-        self.assertIn("PS", address_constants.PROBLEM_ST_TYPE_ABBRVS.keys())
-
-        mock_config_get.side_effect = (
-            'replace', new_addr_keys,
-            None, None, None, None, None,
-            new_problem_st
-        )
-        address_constants.set_address_constants()
-        self.assertEqual(address_constants.ADDRESS_KEYS, new_addr_keys)
-        self.assertDictEqual(
-            new_problem_st, address_constants.PROBLEM_ST_TYPE_ABBRVS
-        )
-
-        mock_config_get.side_effect = (
-            'invalid', new_addr_keys,
-            None, None, None, None, None,
-            new_problem_st
-        )
-        self.assertRaises(
-            ConfigError, address_constants.set_address_constants
-        )
-
-    def test_handle_abnormal_occupancy(self):
-        addr_str = '123 SW MAIN UN'
-        expected = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW'),
-            ('StreetName', 'MAIN'),
-            ('StreetNamePostType', 'UN'),
-        ])
-        result = parse_address_string(addr_str)
-        self.assertEqual(expected, result)
-
-        addr_str = '123 SW MAIN UN A'
-        expected = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW'),
-            ('StreetName', 'MAIN'),
-            ('OccupancyType', 'UN'),
-            ('OccupancyIdentifier', 'A')
-        ])
-        result = parse_address_string(addr_str)
-        self.assertEqual(expected, result)
-
-        addr_str = '123 SW MAIN UN, UN A'
-        expected = OrderedDict([
-            ('AddressNumber', '123'),
-            ('StreetNamePreDirectional', 'SW'),
-            ('StreetName', 'MAIN'),
-            ('StreetNamePostType', 'UN'),
-            ('OccupancyType', 'UN'),
-            ('OccupancyIdentifier', 'A')
-        ])
-        result = parse_address_string(addr_str)
-        self.assertEqual(expected, result)
+#!/usr/bin/env python
+# encoding: utf-8
+"""
+copyright (c) 2016-2019 Earth Advantage.
+All rights reserved
+
+Unit tests for scourgify.
+"""
+
+# Imports from Standard Library
+from collections import OrderedDict
+from unittest import TestCase, mock
+
+# Imports from Third Party Modules
+from yamlconf import ConfigError
+
+# Local Imports
+from scourgify import address_constants
+from scourgify.cleaning import (
+    clean_ambiguous_street_types,
+    clean_period_char,
+    post_clean_addr_str,
+    pre_clean_addr_str,
+)
+from scourgify.exceptions import (
+    AddressNormalizationError,
+    AddressValidationError,
+    AmbiguousAddressError,
+    IncompleteAddressError,
+    UnParseableAddressError,
+)
+from scourgify.normalize import (
+    get_addr_line_str,
+    get_geocoder_normalized_addr,
+    get_normalized_line_segment,
+    get_ordinal_indicator,
+    get_parsed_values,
+    normalize_addr_dict,
+    normalize_addr_str,
+    normalize_address_record,
+    normalize_directionals,
+    normalize_numbered_streets,
+    normalize_occupancy_type,
+    normalize_state,
+    normalize_street_types,
+    parse_address_string,
+    NormalizeAddress
+)
+from scourgify.validations import (
+    validate_address_components,
+    validate_parens_groups_parsed,
+    validate_us_postal_code_format,
+)
+
+# Constants
+SERVICE = 'GBR Test Normalization'
+# Helper Functions & Classes
+
+
+# Tests
+class TestAddressNormalization(TestCase):
+    """Unit tests for scourgify"""
+    # pylint:disable=too-many-arguments
+
+    def setUp(self):
+        """setUp"""
+        self.expected = dict(
+            address_line_1='123 NOWHERE ST',
+            address_line_2='STE 0',
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+        self.address_dict = dict(
+            address_line_1='123 Nowhere St',
+            address_line_2='Suite 0',
+            city='Boring',
+            state='OR',
+            postal_code='97009'
+        )
+
+        self.ordinal_addr = dict(
+            address_line_1='4333 NE 113th',
+            city='Boring',
+            state='OR',
+            postal_code='97009'
+        )
+        self.ordinal_expected = dict(
+            address_line_1='4333 NE 113TH',
+            address_line_2=None,
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+        self.parseable_addr_str = '123 Nowhere Street Suite 0 Boring OR 97009'
+        self.parsed_addr = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetName', 'NOWHERE'),
+            ('StreetNamePostType', 'STREET'),
+            ('OccupancyType', 'SUITE'),
+            ('OccupancyIdentifier', '0'),
+            ('PlaceName', 'BORING'),
+            ('StateName', 'OR'),
+            ('ZipCode', '97009')
+        ])
+        self.hash_tag = '999 Nowhere Street # 12 Boring OR 97009'
+        self.hash_expected = dict(
+            address_line_1='999 NOWHERE ST',
+            address_line_2='# 12',
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+        self.unparesable_addr_str = '6000 SW 1000TH AVE  (BLDG  A5 RIGHT)'
+
+    def test_normalize_address_record(self):
+        """Test normalize_address_record function."""
+        result = normalize_address_record(self.parseable_addr_str)
+        self.assertDictEqual(self.expected, result)
+
+        result = normalize_address_record(self.address_dict)
+        self.assertDictEqual(self.expected, result)
+
+        result = normalize_address_record(self.ordinal_addr)
+        self.assertDictEqual(self.ordinal_expected, result)
+
+        result = normalize_address_record(self.hash_tag)
+        self.assertDictEqual(self.hash_expected, result)
+
+    def test_normalize_class(self):
+        """Test normalize_address_record function."""
+        result = NormalizeAddress(self.parseable_addr_str).normalize()
+        self.assertDictEqual(self.expected, result)
+
+        result = NormalizeAddress(self.address_dict).normalize()
+        self.assertDictEqual(self.expected, result)
+
+        result = NormalizeAddress(self.ordinal_addr).normalize()
+        self.assertDictEqual(self.ordinal_expected, result)
+
+        result = NormalizeAddress(self.hash_tag).normalize()
+        self.assertDictEqual(self.hash_expected, result)
+
+    def test_normalize_addr_str(self):
+        """Test normalize_addr_str function."""
+        result = normalize_addr_str(self.parseable_addr_str)
+        self.assertDictEqual(self.expected, result)
+
+        broken_line1 = '6000 SW 1000TH AVE '
+        broken_line2 = '(BLDG  A1 RIGHT)'
+        result = normalize_addr_str(
+            broken_line1, line2=broken_line2,
+            city='Portland', state='OR', zipcode='97203'
+        )
+        expected = {
+            'address_line_1': '6000 SW 1000TH AVE',
+            'address_line_2': 'BLDG A1 RIGHT',
+            'state': 'OR', 'city': 'PORTLAND',
+            'postal_code': '97203'
+        }
+        self.assertDictEqual(expected, result)
+
+        def addtl_test_func(addr_str):
+            if 'BLDG A1' in addr_str:
+                return '123 NOWHERE STREET', 'BLDG A1 RIGHT'
+            else:
+                raise ValueError
+
+        addtl_processing = '123 Nowhere Street (BLDG A1 RIGHT)'
+        expected = {
+            'address_line_1': '123 NOWHERE ST',
+            'address_line_2': 'BLDG A1 RIGHT',
+            'state': 'OR', 'city': 'PORTLAND',
+            'postal_code': '97203'
+        }
+        result = normalize_addr_str(
+            addtl_processing, city='Portland', state='OR', zipcode='97203',
+            addtl_funcs=[addtl_test_func]
+        )
+        self.assertDictEqual(expected, result)
+
+        self.assertRaises(
+            UnParseableAddressError,
+            normalize_addr_str,
+            self.unparesable_addr_str,
+            city='Portland', state='OR', zipcode='97203',
+            addtl_funcs=[addtl_test_func]
+
+        )
+
+    def test_normalize_addr_dict(self):
+        """Test normalize_addr_dict function."""
+        result = normalize_addr_dict(self.address_dict)
+        self.assertDictEqual(self.expected, result)
+
+        alternate_dict = dict(
+            address1='123 Nowhere St',
+            address2='Suite 0',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        dict_map = {
+            'address_line_1': 'address1',
+            'address_line_2': 'address2',
+            'city': 'city',
+            'state': 'state',
+            'postal_code': 'zip'
+        }
+        result = normalize_addr_dict(alternate_dict, addr_map=dict_map)
+        self.assertDictEqual(self.expected, result)
+
+    def test_parse_address_string(self):
+        """Test parse_address_string function."""
+        result = parse_address_string(self.parseable_addr_str)
+        self.assertIsInstance(result, OrderedDict)
+
+        ambig_addr_str = 'AWBREY VILLAGE'
+        with self.assertRaises(AmbiguousAddressError):
+            parse_address_string(ambig_addr_str)
+
+    def test_normalize_occupancies(self):
+        """Test normalize_addr_dict function with handling for occupancy
+        type oddities.  This is based on a real life incident; the original
+        behavior to allow non-standard unit types to pass through resulted
+        in an address validation service also allowing the address to pass
+        through even though no unit should have existed on the home.
+        """
+        dict_map = {
+            'address_line_1': 'address1',
+            'address_line_2': 'address2',
+            'city': 'city',
+            'state': 'state',
+            'postal_code': 'zip'
+        }
+
+        weird_unit = dict(
+            address1='123 Nowhere St',
+            address2='Ave 345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        expected = dict(
+            address_line_1='123 NOWHERE ST',
+            address_line_2='UNIT 345',
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+        result = normalize_addr_dict(weird_unit, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+        late_unit_add = dict(
+            address1='123 Nowhere St',
+            address2='345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        result = normalize_addr_dict(late_unit_add, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+        expected = dict(
+            address_line_1='123 NOWHERE ST',
+            address_line_2='# 345',
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+
+        hashtag_unit = dict(
+            address1='123 Nowhere St',
+            address2='# 345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        result = normalize_addr_dict(hashtag_unit, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+        hashtag_unit = dict(
+            address1='123 Nowhere St',
+            address2='#345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        result = normalize_addr_dict(hashtag_unit, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+        expected = dict(
+            address_line_1='123 NOWHERE ST',
+            address_line_2='APT 345',
+            city='BORING',
+            state='OR',
+            postal_code='97009'
+        )
+
+        abbreviation = dict(
+            address1='123 Nowhere St',
+            address2='Apt 345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        result = normalize_addr_dict(abbreviation, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+        full_name = dict(
+            address1='123 Nowhere St',
+            address2='Apartment 345',
+            city='Boring',
+            state='OR',
+            zip='97009'
+        )
+        result = normalize_addr_dict(full_name, addr_map=dict_map)
+        self.assertDictEqual(expected, result)
+
+
+class TestAddressNormalizationUtils(TestCase):
+    """Unit tests for scourgify utils"""
+
+    def setUp(self):
+
+        self.address_dict = dict(
+            address_line_1='123 Nowhere St',
+            address_line_2='Suite 0',
+            city='Boring',
+            state='OR',
+            postal_code='97009'
+        )
+        self.parseable_addr = '123 Nowhere Street Suite 0 Boring OR 97009'
+        self.parsed_addr = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetName', 'NOWHERE'),
+            ('StreetNamePostType', 'STREET'),
+            ('OccupancyType', 'SUITE'),
+            ('OccupancyIdentifier', '0'),
+            ('PlaceName', 'BORING'),
+            ('StateName', 'OR'),
+            ('ZipCode', '97009')
+        ])
+
+        self.unparesable_addr = '6000 SW 1000TH AVE  (BLDG  A1 RIGHT)'
+
+        self.unparesable_addr_dict = OrderedDict([
+            ('AddressNumber', '6000'),
+            ('StreetNamePreDirectional', 'SW'),
+            ('StreetName', '1000TH'),
+            ('StreetNamePostType', 'AVE'),
+            ('SubaddressType', 'BLDG'),
+            ('SubaddressIdentifier', 'A1'),
+            ('SubaddressType', 'RIGHT')
+        ])
+
+    def test_get_parsed_values(self):
+        """Test get_parsed_values function."""
+        expected = 'BORING'
+        result = get_parsed_values(self.parsed_addr, 'Boring',
+                                   'PlaceName', self.parseable_addr)
+        self.assertEqual(expected, result)
+
+        expected = 'ONE VALUE PRESENT'
+        result = get_parsed_values(self.parsed_addr, 'One Value Present',
+                                   'LandmarkName', self.parseable_addr)
+        self.assertEqual(expected, result)
+
+        result = get_parsed_values(self.parsed_addr, None,
+                                   'LandmarkName', self.parseable_addr)
+        self.assertIsNone(result)
+
+        with self.assertRaises(AmbiguousAddressError):
+            get_parsed_values(self.parsed_addr, 'UnMatched City',
+                              'PlaceName', self.parseable_addr)
+
+    def test_get_norm_line_segment(self):
+        """Test get normalized_line_segment function."""
+        result = get_normalized_line_segment(self.parsed_addr,
+                                             ['StreetName', 'AddressNumber'])
+        expected = '{} {}'.format(self.parsed_addr['AddressNumber'],
+                                  self.parsed_addr['StreetName'])
+        self.assertEqual(expected, result)
+
+        result = get_normalized_line_segment(
+            self.parsed_addr,
+            ['StreetName', 'StreetNamePostType', 'IntersectionSeparator']
+        )
+        expected = '{} {}'.format(self.parsed_addr['StreetName'],
+                                  self.parsed_addr['StreetNamePostType'])
+        self.assertEqual(expected, result)
+
+    def test_normalize_numbered_streets(self):
+        """Test normalize_numbered_streets function."""
+        numbered_addr = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetName', '100'),
+            ('StreetNamePostType', 'STREET')
+        ])
+        county_road = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreType', 'COUNTY ROAD'),
+            ('StreetName', '100')
+        ])
+        string_addr = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetName', '91st'),
+            ('StreetNamePostType', 'STREET')
+        ])
+
+        expected = '{}{}'.format(
+            numbered_addr['StreetName'], 'th'
+        )
+        result = normalize_numbered_streets(numbered_addr)
+        self.assertEqual(expected, result['StreetName'])
+
+        result = normalize_numbered_streets(county_road)
+        self.assertDictEqual(county_road, result)
+
+        result = normalize_numbered_streets(string_addr)
+        self.assertDictEqual(string_addr, result)
+
+    def test_normalize_directionals(self):
+        """Test normalize_directionals function."""
+        unabbr_directional = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'South West', ),
+            ('StreetName', '100'),
+            ('StreetNamePostType', 'STREET')
+        ])
+        abbrev_directional = OrderedDict([
+            ('AddressNumber', '123'),
+            ('SW', 'StreetNamePreDirectional'),
+            ('StreetNamePreType', 'COUNTY ROAD'),
+            ('StreetName', '100')
+        ])
+        no_directional = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetName', '91st'),
+            ('StreetNamePostType', 'STREET')
+        ])
+
+        expected = 'SW'
+        result = normalize_directionals(unabbr_directional)
+        self.assertEqual(expected, result['StreetNamePreDirectional'])
+
+        result = normalize_directionals(abbrev_directional)
+        self.assertDictEqual(abbrev_directional, result)
+
+        result = normalize_directionals(no_directional)
+        self.assertDictEqual(no_directional, result)
+
+    def test_normalize_street_types(self):
+        """Test normalize_street_types function."""
+        unabbr_type = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW', ),
+            ('StreetName', 'MAIN'),
+            ('StreetNamePostType', 'STREET')
+        ])
+        abbrev_type = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW', ),
+            ('StreetName', 'MAIN'),
+            ('StreetNamePostType', 'AVE')
+        ])
+        typo_type = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW', ),
+            ('StreetName', 'MAIN'),
+            ('StreetNamePostType', 'STROET')
+        ])
+        no_type = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW', ),
+            ('StreetName', 'MAIN'),
+        ])
+
+        expected = 'ST'
+        result = normalize_street_types(unabbr_type)
+        self.assertEqual(expected, result['StreetNamePostType'])
+
+        result = normalize_street_types(abbrev_type)
+        self.assertDictEqual(abbrev_type, result)
+
+        result = normalize_street_types(typo_type)
+        self.assertDictEqual(typo_type, result)
+
+        result = normalize_street_types(no_type)
+        self.assertDictEqual(no_type, result)
+
+    def test_normalize_occupancy_type(self):
+        """Test normalize_occupancy_type function."""
+        expected = 'STE'
+        result = normalize_occupancy_type(self.parsed_addr)
+        self.assertEqual(expected, result['OccupancyType'])
+
+    def test_normalize_state(self):
+        """Test normalize_state function"""
+        state = 'ore'
+        expected = 'OR'
+        result = normalize_state(state)
+        self.assertEqual(expected, result)
+
+        state = 'oregano'
+        expected = state
+        result = normalize_state(state)
+        self.assertEqual(expected, result)
+
+        self.assertIsNone(normalize_state(None))
+
+    def test_pre_clean_addr_str(self):
+        """Test pre_clean_addr_str function"""
+        odd_addr = '123 Nowhere    Street, Suite 0; @Boring OR 97009'
+        # we're leaving commas in the pre-clean until norm can be revisited
+        expected = '123 Nowhere Street, Suite 0 Boring OR 97009'.upper()
+        # expected = '123 Nowhere Street Suite 0 Boring OR 97009'.upper()
+        result = pre_clean_addr_str(odd_addr)
+        self.assertEqual(expected, result)
+
+    def test_post_clean_addr_str(self):
+        """Test post_clean_addr_str function."""
+        addr_str = '(100-104) SW NO   WHERE st'
+        expected = '100-104 SW NO WHERE ST'
+        result = post_clean_addr_str(addr_str)
+        self.assertEqual(expected, result)
+
+        self.assertIsNone(post_clean_addr_str(None))
+        self.assertEqual('', post_clean_addr_str(''))
+
+    def test_validate_address(self):
+        """Test validate_address_components function."""
+        expected = self.address_dict
+        result = validate_address_components(self.address_dict)
+        self.assertEqual(expected, result)
+
+        minus_line1 = dict(
+            address_line_1=None,
+            address_line_2='Suite 0',
+            city='Boring',
+            state='OR',
+            postal_code='97009'
+        )
+        with self.assertRaises(IncompleteAddressError):
+            validate_address_components(minus_line1)
+
+        minus_zip = dict(
+            address_line_1='123 NoWhere St',
+            address_line_2='Suite 0',
+            city='Boring',
+            state='OR',
+            postal_code=None
+        )
+        with self.assertRaises(IncompleteAddressError):
+            validate_address_components(minus_zip)
+
+        minus_city_state = dict(
+            address_line_1='123 NoWhere St',
+            address_line_2='Suite 0',
+            city=None,
+            state=None,
+            postal_code='97009'
+        )
+
+        with self.assertRaises(IncompleteAddressError):
+            validate_address_components(minus_city_state)
+
+        minus_city_state_zip = dict(
+            address_line_1='123 NoWhere St',
+            address_line_2='Suite 0',
+            city=None,
+            state=None,
+            postal_code=None
+        )
+        with self.assertRaises(IncompleteAddressError):
+            validate_address_components(minus_city_state_zip)
+
+    def test_validate_postal_code(self):
+        """Test validate_us_postal_code_format"""
+
+        with self.assertRaises(AddressValidationError):
+            zip_plus = '97219-0001-00'
+            validate_us_postal_code_format(zip_plus, self.address_dict)
+
+        with self.assertRaises(AddressValidationError):
+            zip_plus = '97219-00'
+            validate_us_postal_code_format(zip_plus, self.address_dict)
+
+        with self.assertRaises(AddressValidationError):
+            zip_plus = '972-0001'
+            validate_us_postal_code_format(zip_plus, self.address_dict)
+
+        with self.assertRaises(AddressValidationError):
+            zip_five = '9721900'
+            validate_us_postal_code_format(zip_five, self.address_dict)
+
+        with self.assertRaises(AddressValidationError):
+            zip_five = '972'
+            validate_us_postal_code_format(zip_five, self.address_dict)
+
+        expected = '97219'
+        result = validate_us_postal_code_format(expected, self.address_dict)
+        self.assertEqual(expected, result)
+
+    def test_get_addr_line_str(self):
+        """Test get_addr_line_str function."""
+        expected = '{} {}'.format(
+            self.address_dict['address_line_1'],
+            self.address_dict['address_line_2']
+        )
+        result = get_addr_line_str(self.address_dict)
+        self.assertEqual(expected, result)
+
+        no_line_2 = {
+            'address_line_1': 'address line 1'
+        }
+        expected = no_line_2['address_line_1']
+        result = get_addr_line_str(no_line_2)
+        self.assertEqual(expected, result)
+
+        empty_line_2 = {
+            'address_line_1': 'address line 1',
+            'address_line_2': None
+        }
+        expected = no_line_2['address_line_1']
+        result = get_addr_line_str(empty_line_2)
+        self.assertEqual(expected, result)
+
+        with self.assertRaises(TypeError):
+            get_addr_line_str(self.address_dict, addr_parts='line1')
+
+    @mock.patch(
+        'scourgify.normalize.geocoder'
+    )
+    def test_get_geocoder_normalized_addr(self, mock_geocoder):
+        """Test get_geocoder_normalized_addr"""
+        geo_addr = mock.MagicMock()
+        geo_addr.ok = True
+        geo_addr.housenumber = '1234'
+        geo_addr.street = "Main"
+        geo_addr.subpremise = ''
+        geo_addr.city = 'Boring'
+        geo_addr.state = 'OR'
+        geo_addr.postal = '97000'
+
+        mock_geocoder.google.return_value = geo_addr
+
+        address = {
+            'address_line_1': '1234 Main',
+            'address_line_2': None,
+            'city': 'Boring',
+            'state': 'OR',
+            'postal_code': '97000'
+        }
+        addr_str_return_value = "1234 Main Boring OR 97000"
+        get_geocoder_normalized_addr(address)
+        mock_geocoder.google.assert_called_with(addr_str_return_value)
+
+    def test_get_ordinal_indicator(self):
+        """Test get_ordinal_indicator"""
+        result = get_ordinal_indicator(11)
+        expected = 'th'
+        self.assertEqual(expected, result)
+
+        result = get_ordinal_indicator(112)
+        self.assertEqual(expected, result)
+
+        result = get_ordinal_indicator(3113)
+        self.assertEqual(expected, result)
+
+        result = get_ordinal_indicator(1)
+        expected = 'st'
+        self.assertEqual(expected, result)
+
+        result = get_ordinal_indicator(22)
+        expected = 'nd'
+        self.assertEqual(expected, result)
+
+        result = get_ordinal_indicator(31243)
+        expected = 'rd'
+        self.assertEqual(expected, result)
+
+    def test_clean_period_char(self):
+        """Test clean_period_char"""
+        text = "49.5 blah.blah."
+        expected = "49.5 blahblah"
+        result = clean_period_char(text)
+        self.assertEqual(expected, result)
+
+    def test_validate_parens_group_parsed(self):
+        """Test validate_parens_groups_parsed"""
+        broken_line1 = '6000 SW 1000TH AVE'
+        result = validate_parens_groups_parsed(broken_line1)
+        self.assertEqual(broken_line1, result)
+
+        bad_addr = '10000 NE 8TH (ROW HOUSE)'
+        with self.assertRaises(AmbiguousAddressError):
+            validate_parens_groups_parsed(bad_addr)
+
+    def test_clean_ambiguous_street_types(self):
+        """ Test clean_ambiguous_street_types"""
+        problem_addr = "1234 BROKEN CT"
+        expected = "1234 BROKEN COURT"
+        result = clean_ambiguous_street_types(problem_addr)
+        self.assertEqual(expected, result)
+
+        normal_addr = "1234 NORMAL ST"
+        result = clean_ambiguous_street_types(normal_addr)
+        self.assertEqual(normal_addr, result)
+
+    def test_address_normalization_error(self):
+        error_msg = 'Error Message'
+        error_title = 'ERROR TITLE'
+        addtl_args = 'Addition info'
+        expected = "{}: {}, {}".format(error_title, error_msg, addtl_args)
+        error = AddressNormalizationError(error_msg, error_title, addtl_args)
+        self.assertEqual(expected, str(error))
+
+    @mock.patch.object(address_constants.NormalizationConfig, 'get')
+    def test_set_constants(self, mock_config_get):
+        new_addr_keys = ['new keys']
+        new_problem_st = {
+            "PS": 'STREET'
+        }
+        mock_config_get.side_effect = (
+            'update', new_addr_keys,
+            None, None, None, None, None,
+            new_problem_st
+        )
+        address_constants.set_address_constants()
+        self.assertEqual(address_constants.ADDRESS_KEYS, new_addr_keys)
+        self.assertIn("PS", address_constants.PROBLEM_ST_TYPE_ABBRVS.keys())
+
+        mock_config_get.side_effect = (
+            'replace', new_addr_keys,
+            None, None, None, None, None,
+            new_problem_st
+        )
+        address_constants.set_address_constants()
+        self.assertEqual(address_constants.ADDRESS_KEYS, new_addr_keys)
+        self.assertDictEqual(
+            new_problem_st, address_constants.PROBLEM_ST_TYPE_ABBRVS
+        )
+
+        mock_config_get.side_effect = (
+            'invalid', new_addr_keys,
+            None, None, None, None, None,
+            new_problem_st
+        )
+        self.assertRaises(
+            ConfigError, address_constants.set_address_constants
+        )
+
+    def test_handle_abnormal_occupancy(self):
+        addr_str = '123 SW MAIN UN'
+        expected = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW'),
+            ('StreetName', 'MAIN'),
+            ('StreetNamePostType', 'UN'),
+        ])
+        result = parse_address_string(addr_str)
+        self.assertEqual(expected, result)
+
+        addr_str = '123 SW MAIN UN A'
+        expected = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW'),
+            ('StreetName', 'MAIN'),
+            ('OccupancyType', 'UN'),
+            ('OccupancyIdentifier', 'A')
+        ])
+        result = parse_address_string(addr_str)
+        self.assertEqual(expected, result)
+
+        addr_str = '123 SW MAIN UN, UN A'
+        expected = OrderedDict([
+            ('AddressNumber', '123'),
+            ('StreetNamePreDirectional', 'SW'),
+            ('StreetName', 'MAIN'),
+            ('StreetNamePostType', 'UN'),
+            ('OccupancyType', 'UN'),
+            ('OccupancyIdentifier', 'A')
+        ])
+        result = parse_address_string(addr_str)
+        self.assertEqual(expected, result)
```

### Comparing `usaddress-scourgify-0.2.4/scourgify/tests/test_cleaning.py` & `usaddress-scourgify-0.3.0/scourgify/tests/test_cleaning.py`

 * *Files identical despite different names*

### Comparing `usaddress-scourgify-0.2.4/scourgify/validations.py` & `usaddress-scourgify-0.3.0/scourgify/validations.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-#!/usr/bin/env python
-# encoding: utf-8
-"""
-copyright (c) 2016-2017 Earth Advantage.
-All rights reserved
-..codeauthor::Fable Turas <fable@rainsoftware.tech>
-
-[ INSERT DOC STRING ]  # TODO
-"""
-# Imports from Standard Library
-import re
-from typing import Mapping, Union
-
-# Local Imports
-# Public Classes and Functions
-from scourgify.cleaning import post_clean_addr_str
-from scourgify.exceptions import (
-    AddressValidationError,
-    AmbiguousAddressError,
-    IncompleteAddressError,
-)
-
-# Setup
-
-# Constants
-
-# Data Structure Definitions
-
-# Private Functions
-
-
-def _get_substrings_with_regex(string, pattern=None):
-    # type: (str) -> list
-    """Get substring matching regex rule.
-
-    :param string: string to search for substring
-    :type string: str
-    :param pattern: regex pattern
-    :type pattern: regex
-    :return: str matching pattern search or None
-    :rtype: list
-    """
-    pattern = re.compile(pattern)
-    match = re.findall(pattern, string)
-    return match
-
-
-# Public Functions
-def validate_address_components(address_dict, strict=True):
-    # type: (Mapping[str, str]) -> Mapping[str, str]
-    """Validate non-null values for minimally viable address elements.
-
-    All addresses should have at least an address_line_1 and a postal_code
-    or a city and state.
-
-    :param address_dict: dict containing address components having keys
-        'address_line_1', 'postal_code', 'city', 'state'
-    :type address_dict: Mapping
-    :param strict: bool indicating strict handling of components address parts
-        city, state and postal_code, vs city and state OR postal_code
-    :return: address_dict if no errors are raised.
-    :rtype: Mapping
-    """
-    locality = (
-        address_dict.get('postal_code') and
-        address_dict.get('city') and address_dict.get('state')
-        if strict else
-        address_dict.get('postal_code') or
-        (address_dict.get('city') and address_dict.get('state'))
-    )
-    if not address_dict.get('address_line_1'):
-        msg = 'Address records must include Line 1 data.'
-        raise IncompleteAddressError(msg)
-    elif not locality:
-        msg = (
-            'Address records must contain a city, state, and postal_code.'
-            if strict else
-            'Address records must contain a city and state, or a postal_code'
-        )
-        raise IncompleteAddressError(msg)
-    return address_dict
-
-
-def validate_us_postal_code_format(postal_code, address):
-    # type: (str, Union[str, Mapping]) -> str
-    """Validate postal code conforms to US five-digit Zip or Zip+4 standards.
-
-    :param postal_code: string containing US postal code data.
-    :type postal_code: str
-    :param address: dict or string containing original address.
-    :type address: dict | str
-    :return: original postal code if no error is raised
-    :rtype: str
-    """
-    error = None
-    msg = (
-        'US Postal Codes must conform to five-digit Zip or Zip+4 standards.'
-    )
-    postal_code = post_clean_addr_str(postal_code)
-    if '-' in postal_code:
-        plus_four_code = postal_code.split('-')
-        if len(plus_four_code) != 2:
-            error = True
-        elif len(plus_four_code[0]) != 5 or len(plus_four_code[1]) != 4:
-            error = True
-    elif len(postal_code) != 5:
-        error = True
-
-    if error:
-        raise AddressValidationError(msg, None, address)
-    else:
-        return postal_code
-
-
-def validate_parens_groups_parsed(line1):
-    # type: (str) -> str
-    """Validate any parenthesis segments have been successfully parsed.
-
-    Assumes any parenthesis segments in original address string are either
-    line 2 or ambiguous address elements.  If any parenthesis segment remains
-    in line1 after all other address processing has been applied,
-    AmbiguousAddressError is raised.
-
-    :param line1: processed line1 address string portion
-    :type line1: str
-    :return: line1 address string
-    :rtype: str
-    """
-    parenthesis_groups = _get_substrings_with_regex(line1, r'\((.+?)\)')
-    if parenthesis_groups:
-        raise AmbiguousAddressError(None, None, line1)
-    else:
-        return line1
+#!/usr/bin/env python
+# encoding: utf-8
+"""
+copyright (c) 2016-2017 Earth Advantage.
+All rights reserved
+..codeauthor::Fable Turas <fable@rainsoftware.tech>
+
+[ INSERT DOC STRING ]  # TODO
+"""
+# Imports from Standard Library
+import re
+from typing import Mapping, Union
+
+# Local Imports
+# Public Classes and Functions
+from scourgify.cleaning import post_clean_addr_str
+from scourgify.exceptions import (
+    AddressValidationError,
+    AmbiguousAddressError,
+    IncompleteAddressError,
+)
+
+# Setup
+
+# Constants
+
+# Data Structure Definitions
+
+# Private Functions
+
+
+def _get_substrings_with_regex(string, pattern=None):
+    # type: (str) -> list
+    """Get substring matching regex rule.
+
+    :param string: string to search for substring
+    :type string: str
+    :param pattern: regex pattern
+    :type pattern: regex
+    :return: str matching pattern search or None
+    :rtype: list
+    """
+    pattern = re.compile(pattern)
+    match = re.findall(pattern, string)
+    return match
+
+
+# Public Functions
+def validate_address_components(address_dict, strict=True):
+    # type: (Mapping[str, str]) -> Mapping[str, str]
+    """Validate non-null values for minimally viable address elements.
+
+    All addresses should have at least an address_line_1 and a postal_code
+    or a city and state.
+
+    :param address_dict: dict containing address components having keys
+        'address_line_1', 'postal_code', 'city', 'state'
+    :type address_dict: Mapping
+    :param strict: bool indicating strict handling of components address parts
+        city, state and postal_code, vs city and state OR postal_code
+    :return: address_dict if no errors are raised.
+    :rtype: Mapping
+    """
+    locality = (
+        address_dict.get('postal_code') and
+        address_dict.get('city') and address_dict.get('state')
+        if strict else
+        address_dict.get('postal_code') or
+        (address_dict.get('city') and address_dict.get('state'))
+    )
+    if not address_dict.get('address_line_1'):
+        msg = 'Address records must include Line 1 data.'
+        raise IncompleteAddressError(msg)
+    elif not locality:
+        msg = (
+            'Address records must contain a city, state, and postal_code.'
+            if strict else
+            'Address records must contain a city and state, or a postal_code'
+        )
+        raise IncompleteAddressError(msg)
+    return address_dict
+
+
+def validate_us_postal_code_format(postal_code, address):
+    # type: (str, Union[str, Mapping]) -> str
+    """Validate postal code conforms to US five-digit Zip or Zip+4 standards.
+
+    :param postal_code: string containing US postal code data.
+    :type postal_code: str
+    :param address: dict or string containing original address.
+    :type address: dict | str
+    :return: original postal code if no error is raised
+    :rtype: str
+    """
+    error = None
+    msg = (
+        'US Postal Codes must conform to five-digit Zip or Zip+4 standards.'
+    )
+    postal_code = post_clean_addr_str(postal_code)
+    if '-' in postal_code:
+        plus_four_code = postal_code.split('-')
+        if len(plus_four_code) != 2:
+            error = True
+        elif len(plus_four_code[0]) != 5 or len(plus_four_code[1]) != 4:
+            error = True
+    elif len(postal_code) != 5:
+        error = True
+
+    if error:
+        raise AddressValidationError(msg, None, address)
+    else:
+        return postal_code
+
+
+def validate_parens_groups_parsed(line1):
+    # type: (str) -> str
+    """Validate any parenthesis segments have been successfully parsed.
+
+    Assumes any parenthesis segments in original address string are either
+    line 2 or ambiguous address elements.  If any parenthesis segment remains
+    in line1 after all other address processing has been applied,
+    AmbiguousAddressError is raised.
+
+    :param line1: processed line1 address string portion
+    :type line1: str
+    :return: line1 address string
+    :rtype: str
+    """
+    parenthesis_groups = _get_substrings_with_regex(line1, r'\((.+?)\)')
+    if parenthesis_groups:
+        raise AmbiguousAddressError(None, None, line1)
+    else:
+        return line1
```

### Comparing `usaddress-scourgify-0.2.4/setup.cfg` & `usaddress-scourgify-0.3.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = usaddress-scourgify
-version = 0.2.4
+version = 0.3.0
 description = Clean US addresses following USPS pub 28 and RESO guidelines
 author = Fable Turas
 author_email = fable@rainsoftware.tech
 maintainer = GreenBuildingRegistry
 maintainer_email = admin@greenbuildingregistry.com
 keywords = usaddress, normalization, address
 url = https://github.com/GreenBuildingRegistry/usaddress-scourgify
@@ -21,15 +21,14 @@
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
 	geocoder>=1.22.6
 	usaddress>=0.5.9
-	frozendict>=1.2
 	yaml-config>=0.1.2
 
 [bdist_wheel]
 python-tag = py3
 
 [egg_info]
 tag_build =
```

### Comparing `usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/PKG-INFO` & `usaddress-scourgify-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: usaddress-scourgify
-Version: 0.2.4
+Version: 0.3.0
 Summary: Clean US addresses following USPS pub 28 and RESO guidelines
 Home-page: https://github.com/GreenBuildingRegistry/usaddress-scourgify
 Author: Fable Turas
 Author-email: fable@rainsoftware.tech
 Maintainer: GreenBuildingRegistry
 Maintainer-email: admin@greenbuildingregistry.com
 License: UNKNOWN
-Description: UNKNOWN
 Keywords: usaddress,normalization,address
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `usaddress-scourgify-0.2.4/usaddress_scourgify.egg-info/SOURCES.txt` & `usaddress-scourgify-0.3.0/usaddress_scourgify.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.rst
 setup.cfg
 setup.py
 scourgify/__init__.py
 scourgify/address_constants.py
 scourgify/cleaning.py
 scourgify/exceptions.py
```

