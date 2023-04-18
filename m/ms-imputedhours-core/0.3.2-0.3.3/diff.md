# Comparing `tmp/ms_imputedhours_core-0.3.2.tar.gz` & `tmp/ms_imputedhours_core-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_imputedhours_core-0.3.2.tar", last modified: Tue Apr 18 11:56:22 2023, max compression
+gzip compressed data, was "ms_imputedhours_core-0.3.3.tar", last modified: Tue Apr 18 12:10:55 2023, max compression
```

## Comparing `ms_imputedhours_core-0.3.2.tar` & `ms_imputedhours_core-0.3.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/__pycache__/test_agreements.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/test_agreements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/__pycache__/test_employee.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/test_employee.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/constants.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/__pycache__/test_data.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/alert.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/dates.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_alert.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_bigquery.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_dates.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/__pycache__/hours.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/hours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-18 11:56:20.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/__pycache__/test_office.cpython-310.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/test_office.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 11:56:22.249283 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 11:56:22.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 11:56:22.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 11:56:22.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-18 11:56:22.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 11:56:22.000000 ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 11:56:22.253283 ms_imputedhours_core-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 11:56:03.000000 ms_imputedhours_core-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/test_agreements.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/test_agreements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/test_employee.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/test_employee.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/bigquery.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/constants.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/test_data.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10302 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/alert.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/bigquery.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/dates.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_alert.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_bigquery.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_dates.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/hours.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/hours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__pycache__/__init__.cpython-310.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-18 12:10:53.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/test_office.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/test_office.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:10:55.610769 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 12:10:55.000000 ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 12:10:55.614769 ms_imputedhours_core-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 12:10:33.000000 ms_imputedhours_core-0.3.3/setup.py
```

### Comparing `ms_imputedhours_core-0.3.2/LICENSE` & `ms_imputedhours_core-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/PKG-INFO` & `ms_imputedhours_core-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_imputedhours_core
-Version: 0.3.2
+Version: 0.3.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Jonathan Rodriguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ms_imputedhours_core-0.3.2/README.md` & `ms_imputedhours_core-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__init__.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__pycache__/__init__.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 3144 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 480c 0000  o.......S.>dH...
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 480c 0000  o.........>dH...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6500  ..d.d.l.m.Z...e.
 00000050: a004 6404 6405 a102 5a05 6500 a004 6406  ..d.d...Z.e...d.
 00000060: 6407 a102 5a06 6408 6701 5a07 4700 6409  d...Z.d.g.Z.G.d.
 00000070: 640a 8400 640a 6508 8303 5a09 6401 5300  d...d.e...Z.d.S.
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/__pycache__/test_agreements.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/__pycache__/test_agreements.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 3209 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 890c 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 890c 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 4700 6404 6405 8400 6405 6500 6a05  ..G.d.d...d.e.j.
 00000060: 8303 5a06 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000070: 2902 da04 4d6f 636b da05 7061 7463 6829  )...Mock..patch)
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/agreements/__tests__/test_agreements.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/agreements/__tests__/test_agreements.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__init__.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__pycache__/__init__.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 4025 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 b90f 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 b90f 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 6401 6c00 6d00 5a00 0100 6402 5a01 6403  d.l.m.Z...d.Z.d.
 00000040: 5a02 6404 6405 8400 5a03 0906 640a 6407  Z.d.d...Z...d.d.
 00000050: 6408 8401 5a04 6409 5300 290b e900 0000  d...Z.d.S.).....
 00000060: 0029 01da 0864 6174 6574 696d 65e9 6400  .)...datetime.d.
 00000070: 0000 6700 0000 0000 00f0 3f63 0300 0000  ..g.......?c....
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/__pycache__/test_employee.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/__pycache__/test_employee.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 6085 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 c517 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 c517 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0073 e200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 6400 6405 6c06  d.l.m.Z...d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6406 6900 6407  m.Z.m.Z...d.i.d.
 00000070: 6408 9301 6409 640a 9301 640b 640a 9301  d...d.d...d.d...
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/__tests__/test_employee.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/__tests__/test_employee.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__init__.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/__init__.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 6771 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 731a 0000  o.......S.>ds...
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 731a 0000  o.........>ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 c400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c  m.Z.m.Z.m.Z.m.Z.
 00000070: 6d0d 5a0d 0100 6400 6405 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__pycache__/bigquery.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__pycache__/bigquery.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 10302 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 3e28 0000  o.......S.>d>(..
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 3e28 0000  o.........>d>(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0801 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 6d07 5a07 0100 6500  d.l.m.Z.m.Z...e.
 00000060: a008 6405 6406 a102 5a09 6500 a008 6407  ..d.d...Z.e...d.
 00000070: 6408 a102 5a0a 6500 a008 6409 640a a102  d...Z.e...d.d...
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/__pycache__/test_data.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/__pycache__/test_data.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 8852 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 9422 0000  o.......S.>d."..
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 9422 0000  o.........>d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0010 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
 00000070: 6900 6407 6408 9301 6409 6408 9301 640a  i.d.d...d.d...d.
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/__tests__/test_data.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/__tests__/test_data.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/bigquery.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/alert.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/alert.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 622 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 6e02 0000  o.......S.>dn...
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 6e02 0000  o.........>dn...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 1800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 8400  d.l.m.Z...d.d...
 00000040: 5a02 6404 5300 2905 e900 0000 0029 01da  Z.d.S.)......)..
 00000050: 1445 5843 4c55 4445 5f41 4c45 5254 5f45  .EXCLUDE_ALERT_E
 00000060: 4d41 494c 5363 0400 0000 0000 0000 0000  MAILSc..........
 00000070: 0000 0800 0000 0300 0000 4300 0000 7358  ..........C...sX
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/bigquery.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/bigquery.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 3597 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 0d0e 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 0d0e 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6500 a002 6403 6404 a102 5a03 4700  ..e...d.d...Z.G.
 00000050: 6405 6406 8400 6406 6504 8303 5a05 6401  d.d...d.e...Z.d.
 00000060: 5300 2907 e900 0000 004e 2901 da08 6461  S.)......N)...da
 00000070: 7465 7469 6d65 da20 4249 4751 5545 5259  tetime. BIGQUERY
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__pycache__/dates.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__pycache__/dates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 433 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 b101 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 b101 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6403 6404 8400  d.l.m.Z...d.d...
 00000050: 5a04 6405 6406 8400 5a05 6409 6407 6408  Z.d.d...Z.d.d.d.
 00000060: 8401 5a06 6401 5300 290a e900 0000 004e  ..Z.d.S.)......N
 00000070: 2901 da0d 7265 6c61 7469 7665 6465 6c74  )...relativedelt
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_alert.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_alert.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 4301 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 cd10 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 cd10 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4200 0000 6400  .....@...sB...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c04 6d05 5a05 0100 4700 6405 6406  d.l.m.Z...G.d.d.
 00000060: 8400 6406 6500 6a06 8303 5a07 6401 5300  ..d.e.j...Z.d.S.
 00000070: 2907 e900 0000 004e 2901 da05 7061 7463  )......N)...patc
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_bigquery.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_bigquery.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 5713 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 5116 0000  o.......S.>dQ...
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 5116 0000  o.........>dQ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6403 6404 6c02 6d03 5a03 0100 4700  ..d.d.l.m.Z...G.
 00000050: 6405 6406 8400 6406 6500 6a04 8303 5a05  d.d...d.e.j...Z.
 00000060: 6401 5300 2907 e900 0000 004e 2901 da08  d.S.)......N)...
 00000070: 6461 7465 7469 6d65 e902 0000 0029 01da  datetime.....)..
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_dates.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/__pycache__/test_dates.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 776 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 0803 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 0803 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 4700  d.l.m.Z.m.Z...G.
 00000050: 6404 6405 8400 6405 6500 6a05 8303 5a06  d.d...d.e.j...Z.
 00000060: 6401 5300 2906 e900 0000 004e e902 0000  d.S.)......N....
 00000070: 0029 02da 0d67 6574 5f66 6972 7374 5f64  .)...get_first_d
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/__tests__/test_dates.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/alert.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/alert.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/helpers/bigquery.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/helpers/bigquery.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/__pycache__/hours.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/__pycache__/hours.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 3586 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 020e 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 020e 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3200 0000 6400  .....@...s2...d.
 00000030: 5a00 6401 6402 8400 5a01 6403 6404 8400  Z.d.d...Z.d.d...
 00000040: 5a02 6405 6406 8400 5a03 640d 6408 6409  Z.d.d...Z.d.d.d.
 00000050: 8401 5a04 640a 640b 8400 5a05 640c 5300  ..Z.d.d...Z.d.S.
 00000060: 290e da01 3063 0100 0000 0000 0000 0000  )...0c..........
 00000070: 0000 0300 0000 0500 0000 4300 0000 7338  ..........C...s8
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/employee/data/transformers/hours.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/employee/data/transformers/hours.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/__pycache__/test_office.cpython-310.pyc` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/__pycache__/test_office.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Apr 18 11:56:03 2023 UTC, .py size: 663 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 5385 3e64 9702 0000  o.......S.>d....
+00000000: 6f0d 0d0a 0000 0000 b988 3e64 9702 0000  o.........>d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 6500 6a03  ..G.d.d...d.e.j.
 00000050: 8303 5a04 6401 5300 2905 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da14 6765 745f 7265 616c 5f6f 6666  )...get_real_off
 00000070: 6963 655f 6e61 6d65 6300 0000 0000 0000  ice_namec.......
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core/office/__tests__/test_office.py` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core/office/__tests__/test_office.py`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/PKG-INFO` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-imputedhours-core
-Version: 0.3.2
+Version: 0.3.3
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Jonathan Rodriguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/SOURCES.txt` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_imputedhours_core-0.3.2/ms_imputedhours_core.egg-info/requires.txt` & `ms_imputedhours_core-0.3.3/ms_imputedhours_core.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 APScheduler==3.9.1
-Flask==2.0.2
 Jinja2==3.0.3
 MarkupSafe==2.0.1
 Pygments==2.13.0
 SecretStorage==3.3.3
 Werkzeug==2.0.2
 attrs==22.1.0
 autopep8==1.7.0
@@ -30,15 +29,14 @@
 google-cloud-bigquery==3.9.0
 google-cloud-core==2.3.2
 google-crc32c==1.5.0
 google-resumable-media==2.4.0
 googleapis-common-protos==1.57.0
 grpcio-status==1.50.0
 grpcio==1.50.0
-gunicorn==20.1.0
 httplib2==0.21.0
 idna==3.4
 importlib-metadata==5.0.0
 iniconfig==1.1.1
 isort==5.12.0
 itsdangerous==2.0.1
 jaraco.classes==3.2.3
```

### Comparing `ms_imputedhours_core-0.3.2/requirements.txt` & `ms_imputedhours_core-0.3.3/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 charset-normalizer==2.1.1
 click==8.0.3
 commonmark==0.9.1
 cryptography==38.0.3
 docutils==0.19
 exceptiongroup==1.0.0
 flake8==6.0.0
-Flask==2.0.2
 freezegun==1.2.2
 gc-google-services-api==1.2.5
 google-api-core==2.10.2
 google-api-python-client==2.85.0
 google-auth==2.14.1
 google-auth-httplib2==0.1.0
 google-auth-oauthlib==0.7.1
@@ -26,15 +25,14 @@
 google-cloud-bigquery-storage==2.16.2
 google-cloud-core==2.3.2
 google-crc32c==1.5.0
 google-resumable-media==2.4.0
 googleapis-common-protos==1.57.0
 grpcio==1.50.0
 grpcio-status==1.50.0
-gunicorn==20.1.0
 httplib2==0.21.0
 idna==3.4
 importlib-metadata==5.0.0
 iniconfig==1.1.1
 isort==5.12.0
 itsdangerous==2.0.1
 jaraco.classes==3.2.3
```

### Comparing `ms_imputedhours_core-0.3.2/setup.py` & `ms_imputedhours_core-0.3.3/setup.py`

 * *Files identical despite different names*

