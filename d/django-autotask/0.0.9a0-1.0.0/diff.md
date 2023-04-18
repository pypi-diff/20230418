# Comparing `tmp/django-autotask-0.0.9a0.tar.gz` & `tmp/django-autotask-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-autotask-0.0.9a0.tar", last modified: Tue Oct  8 23:20:54 2019, max compression
+gzip compressed data, was "django-autotask-1.0.0.tar", last modified: Tue Apr 18 21:17:57 2023, max compression
```

## Comparing `django-autotask-0.0.9a0.tar` & `django-autotask-1.0.0.tar`

### file list

```diff
@@ -1,96 +1,341 @@
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/
--rw-rw-r--   0 sam       (1000) sam       (1000)       99 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/apps.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/migrations/
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0010_merge_20190923_1155.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1430 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0004_auto_20190913_1425.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1843 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0008_auto_20190917_1454.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     2211 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0001_initial.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1583 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/migrations/0015_auto_20191001_0847.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     6182 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/migrations/0014_auto_20190930_1548.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      601 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3229 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      552 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      547 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      545 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1718 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1537 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      545 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1774 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1663 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      589 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      591 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      917 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      153 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1582 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1612 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1470 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      627 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      668 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     3136 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1649 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      337 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0005_remove_ticketstatus_value.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      360 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0011_auto_20190923_1157.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/djautotask/migrations/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1640 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0007_auto_20190917_1009.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      441 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190920_1648.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     4964 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190918_1525.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      287 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0006_merge_20190920_1450.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1036 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0010_auto_20190923_0930.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1723 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0006_auto_20190916_1645.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      446 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0013_auto_20190923_1439.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      280 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0012_merge_20190923_1439.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      281 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0008_merge_20190920_1644.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1715 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0003_auto_20190913_0941.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1517 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0005_auto_20190916_1549.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      407 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/migrations/0002_ticket_ticket_number.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)     8811 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/models.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     2949 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/api.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      683 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/utils.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      332 2019-10-08 23:20:52.000000 django-autotask-0.0.9a0/djautotask/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    16255 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/__pycache__/sync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     6563 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/models.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      226 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/__init__.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/tests/
--rw-rw-r--   0 sam       (1000) sam       (1000)    11643 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/fixtures.py
--rw-rw-r--   0 sam       (1000) sam       (1000)   174033 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/tests/atws.wsdl
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)    10185 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_commands.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     7853 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/fixture_utils.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     7163 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/fixtures.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)    18302 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_sync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     1836 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/mocks.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      363 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/test_model.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)      148 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/tests/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)       72 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/tests/test_model.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     8875 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/test_commands.py
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/djautotask/tests/__init__.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1516 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/mocks.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    15091 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/test_sync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     7839 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/tests/fixture_utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3236 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/admin.py
--rw-rw-r--   0 sam       (1000) sam       (1000)    16965 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/sync.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)      153 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/management/__pycache__/__init__.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)        0 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/djautotask/management/__init__.py
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/commands/
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/djautotask/management/commands/__pycache__/
--rw-rw-r--   0 sam       (1000) sam       (1000)     4469 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/djautotask/management/commands/__pycache__/atsync.cpython-35.pyc
--rw-rw-r--   0 sam       (1000) sam       (1000)     5350 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/management/commands/atsync.py
--rw-rw-r--   0 sam       (1000) sam       (1000)      384 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/utils.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     3005 2019-10-08 23:20:37.000000 django-autotask-0.0.9a0/djautotask/api.py
--rw-rw-r--   0 sam       (1000) sam       (1000)     1797 2019-10-01 23:08:49.000000 django-autotask-0.0.9a0/setup.py
--rw-rw-r--   0 sam       (1000) sam       (1000)       38 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/setup.cfg
--rw-rw-r--   0 sam       (1000) sam       (1000)     2385 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/PKG-INFO
-drwxrwxr-x   0 sam       (1000) sam       (1000)        0 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/
--rw-rw-r--   0 sam       (1000) sam       (1000)     3978 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/SOURCES.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/dependency_links.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)     2385 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/PKG-INFO
--rw-rw-r--   0 sam       (1000) sam       (1000)       97 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/requires.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)       11 2019-10-08 23:20:54.000000 django-autotask-0.0.9a0/django_autotask.egg-info/top_level.txt
--rw-rw-r--   0 sam       (1000) sam       (1000)        1 2019-10-08 23:20:53.000000 django-autotask-0.0.9a0/django_autotask.egg-info/not-zip-safe
--rw-rw-r--   0 sam       (1000) sam       (1000)      945 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/README.md
--rw-rw-r--   0 sam       (1000) sam       (1000)       82 2019-09-05 17:26:40.000000 django-autotask-0.0.9a0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.723753 django-autotask-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1083 2023-04-18 21:17:14.000000 django-autotask-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-04-18 21:17:14.000000 django-autotask-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-18 21:17:57.723753 django-autotask-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-04-18 21:17:14.000000 django-autotask-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/django_autotask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-04-18 21:17:57.000000 django-autotask-1.0.0/django_autotask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    18996 2023-04-18 21:17:57.000000 django-autotask-1.0.0/django_autotask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 21:17:57.000000 django-autotask-1.0.0/django_autotask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 21:17:26.000000 django-autotask-1.0.0/django_autotask.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-18 21:17:57.000000 django-autotask-1.0.0/django_autotask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-18 21:17:57.000000 django-autotask-1.0.0/django_autotask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/
+-rw-r--r--   0 runner    (1001) docker     (122)      226 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-18 21:17:26.000000 django-autotask-1.0.0/djautotask/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/__pycache__/api.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/__pycache__/apps.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    47701 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    57459 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/__pycache__/sync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      370 2023-04-18 21:17:56.000000 django-autotask-1.0.0/djautotask/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2578 2023-04-18 21:17:56.000000 django-autotask-1.0.0/djautotask/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    10903 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31950 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/management/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/management/commands/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.695753 django-autotask-1.0.0/djautotask/management/commands/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)     6367 2023-04-18 21:17:47.000000 django-autotask-1.0.0/djautotask/management/commands/__pycache__/atsync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/management/commands/atsync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1637 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/management/commands/clearoldsyncjobs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/management/commands/list_users.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.707753 django-autotask-1.0.0/djautotask/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     2211 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0002_ticket_ticket_number.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1715 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0003_auto_20190913_0941.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0004_auto_20190913_1425.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0005_auto_20190916_1549.py
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0005_remove_ticketstatus_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0006_auto_20190916_1645.py
+-rw-r--r--   0 runner    (1001) docker     (122)      287 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0006_merge_20190920_1450.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0007_auto_20190917_1009.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1843 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0008_auto_20190917_1454.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0008_merge_20190920_1644.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4964 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0009_auto_20190918_1525.py
+-rw-r--r--   0 runner    (1001) docker     (122)      441 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0009_auto_20190920_1648.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1036 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0010_auto_20190923_0930.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0010_merge_20190923_1155.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0011_auto_20190923_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0012_merge_20190923_1439.py
+-rw-r--r--   0 runner    (1001) docker     (122)      446 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0013_auto_20190923_1439.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6182 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0014_auto_20190930_1548.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1583 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0015_auto_20191001_0847.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0016_auto_20191021_0958.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0017_auto_20191021_1028.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1697 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0018_auto_20191029_1621.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1552 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0018_auto_20191029_1634.py
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0019_auto_20191030_0905.py
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0020_auto_20191030_0916.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0021_merge_20191031_0858.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0021_merge_20191031_1259.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0022_merge_20191031_1620.py
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0023_auto_20191119_0923.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3582 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0024_auto_20191122_1516.py
+-rw-r--r--   0 runner    (1001) docker     (122)      362 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0025_auto_20191125_0939.py
+-rw-r--r--   0 runner    (1001) docker     (122)      366 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0026_auto_20191125_0952.py
+-rw-r--r--   0 runner    (1001) docker     (122)      375 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0027_auto_20191125_1103.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1763 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0028_phase.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0028_task_secondary_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0029_phase_last_activity_date.py
+-rw-r--r--   0 runner    (1001) docker     (122)      490 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0030_task_phase.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0031_auto_20191129_1454.py
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0031_merge_20191202_1119.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0032_auto_20191129_1501.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0033_merge_20191204_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0034_auto_20191210_1518.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2114 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0035_timeentry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0036_auto_20200127_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0037_subissuetype_parent_value.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0038_auto_20200130_1218.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4027 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0038_notetype_tasknote_ticketnote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0039_auto_20200131_1134.py
+-rw-r--r--   0 runner    (1001) docker     (122)      290 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0039_merge_20200131_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0040_auto_20200204_1538.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0040_merge_20200131_1627.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0041_merge_20200204_1546.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0042_auto_20200205_1057.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1304 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0042_auto_20200205_1455.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0043_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0043_timeentry_allocation_code.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0044_merge_20200205_1651.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1647 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0045_resourceroledepartment_resourceservicedeskrole.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0046_auto_20200207_1002.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0046_ticket_assigned_resource_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0047_auto_20200207_1126.py
+-rw-r--r--   0 runner    (1001) docker     (122)      523 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0047_task_assigned_resource_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      853 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0048_auto_20200211_1037.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0049_merge_20200227_1701.py
+-rw-r--r--   0 runner    (1001) docker     (122)      331 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0050_remove_ticket_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)      754 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0051_auto_20200315_1819.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0051_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      445 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0052_contract_status.py
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0053_timeentry_contract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0054_merge_20200323_1511.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0055_auto_20200325_0928.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0055_auto_20200325_1335.py
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0056_merge_20200327_1045.py
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0057_auto_20200406_1620.py
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0058_auto_20200408_1022.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8223 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0059_auto_20200414_1242.py
+-rw-r--r--   0 runner    (1001) docker     (122)      850 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0060_auto_20200414_1522.py
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0061_auto_20200416_1241.py
+-rw-r--r--   0 runner    (1001) docker     (122)      506 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0062_task_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0063_accountphysicallocation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0064_auto_20200511_1124.py
+-rw-r--r--   0 runner    (1001) docker     (122)      529 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0064_servicecall_location.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0065_auto_20200512_1224.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0066_auto_20200512_1420.py
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0067_auto_20200519_1100.py
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0067_merge_20200514_1713.py
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0068_merge_20200521_1615.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0069_auto_20200602_1419.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0070_auto_20200714_0807.py
+-rw-r--r--   0 runner    (1001) docker     (122)      421 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0071_project_status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0072_account_parent_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)      401 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0073_syncjob_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)      437 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0074_auto_20200827_1818.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1385 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0075_taskpredecessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0076_auto_20200923_0953.py
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0076_auto_20200925_1326.py
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0077_auto_20200924_1512.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0078_merge_20201001_1657.py
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0079_auto_20201003_1125.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14818 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      590 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0081_project_department.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0082_auto_20201020_1617.py
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0083_ticketudftracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      917 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0084_projectudftracker_taskudftracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0085_auto_20201022_1822.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2105 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0086_auto_20201222_1402.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0087_auto_20210108_1214.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0087_auto_20210108_1307.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0088_merge_20210113_1743.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1705 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0089_auto_20210125_1649.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0090_auto_20210309_1157.py
+-rw-r--r--   0 runner    (1001) docker     (122)      417 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0091_auto_20210525_1723.py
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0092_auto_20210629_1124.py
+-rw-r--r--   0 runner    (1001) docker     (122)      477 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0093_auto_20210629_1204.py
+-rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0094_auto_20210723_1018.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0094_auto_20210727_0940.py
+-rw-r--r--   0 runner    (1001) docker     (122)      368 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0095_auto_20210726_1251.py
+-rw-r--r--   0 runner    (1001) docker     (122)      279 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0096_merge_20210728_1429.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0097_auto_20210819_1402.py
+-rw-r--r--   0 runner    (1001) docker     (122)      430 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0098_auto_20211029_1641.py
+-rw-r--r--   0 runner    (1001) docker     (122)      528 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0099_auto_20211124_1808.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1863 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0100_auto_20211228_1443.py
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0101_auto_20220104_1349.py
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0102_auto_20220104_1655.py
+-rw-r--r--   0 runner    (1001) docker     (122)      391 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0103_auto_20220106_1622.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0104_rename_allocationcode_billingcode_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0105_tasknote_created_by_contact.py
+-rw-r--r--   0 runner    (1001) docker     (122)      525 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0106_ticketnote_created_by_contact.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0107_contact_extension.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1600 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0108_billingcodetype_billingcodetypetracker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0109_billingcode_billing_code_type.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0110_account_phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0111_alter_phase_estimated_hours.py
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/0112_account_owner_resource.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.723753 django-autotask-1.0.0/djautotask/migrations/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)     1622 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1517 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0003_auto_20190913_0941.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0004_auto_20190913_1425.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1414 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0005_auto_20190916_1549.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1525 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0006_auto_20190916_1645.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      516 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1467 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0007_auto_20190917_1009.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0008_auto_20190917_1454.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2645 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0009_auto_20190918_1525.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      837 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0010_auto_20190923_0930.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0012_merge_20190923_1439.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      586 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0013_auto_20190923_1439.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0014_auto_20190930_1548.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0015_auto_20191001_0847.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0016_auto_20191021_0958.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0017_auto_20191021_1028.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1136 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0018_auto_20191029_1621.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1435 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0018_auto_20191029_1634.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      659 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0019_auto_20191030_0905.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0020_auto_20191030_0916.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0021_merge_20191031_0858.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0021_merge_20191031_1259.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0022_merge_20191031_1620.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0023_auto_20191119_0923.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0024_auto_20191122_1516.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0025_auto_20191125_0939.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0026_auto_20191125_0952.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0028_phase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      732 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0028_task_secondary_resources.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      621 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0029_phase_last_activity_date.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      719 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0030_task_phase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1003 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0031_auto_20191129_1454.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0031_merge_20191202_1119.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0032_auto_20191129_1501.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0033_merge_20191204_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0034_auto_20191210_1518.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1673 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0035_timeentry.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      860 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0036_auto_20200127_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0037_subissuetype_parent_value.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0038_auto_20200130_1218.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0038_notetype_tasknote_ticketnote.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1429 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0039_auto_20200131_1134.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      519 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0039_merge_20200131_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0040_auto_20200204_1538.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0040_merge_20200131_1627.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0041_merge_20200204_1546.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1681 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0042_auto_20200205_1057.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1262 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0042_auto_20200205_1455.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      802 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0043_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0043_timeentry_allocation_code.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0044_merge_20200205_1651.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0045_resourceroledepartment_resourceservicedeskrole.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0046_auto_20200207_1002.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      787 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0046_ticket_assigned_resource_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      803 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0047_auto_20200207_1126.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      766 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0047_task_assigned_resource_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0048_auto_20200211_1037.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0049_merge_20200227_1701.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      545 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0050_remove_ticket_role.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0051_auto_20200315_1819.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0051_contract.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0053_timeentry_contract.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0054_merge_20200323_1511.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0055_auto_20200325_0928.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0055_auto_20200325_1335.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0056_merge_20200327_1045.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      762 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0057_auto_20200406_1620.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0058_auto_20200408_1022.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0059_auto_20200414_1242.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0060_auto_20200414_1522.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      623 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0061_auto_20200416_1241.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      737 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0062_task_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0063_accountphysicallocation.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      942 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0064_auto_20200511_1124.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0064_servicecall_location.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0065_auto_20200512_1224.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0066_auto_20200512_1420.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0067_auto_20200519_1100.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      511 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0067_merge_20200514_1713.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0068_merge_20200521_1615.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      822 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0069_auto_20200602_1419.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0070_auto_20200714_0807.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0071_project_status_detail.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0072_account_parent_account.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0073_syncjob_skipped.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0074_auto_20200827_1818.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0075_taskpredecessor.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1033 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0076_auto_20200923_0953.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0076_auto_20200925_1326.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      814 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0077_auto_20200924_1512.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0078_merge_20201001_1657.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0079_auto_20201003_1125.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     5525 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0080_accountphysicallocationtracker_accounttracker_accounttypetracker_allocationcodetracker_contracttrack.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      825 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0081_project_department.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0082_auto_20201020_1617.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      672 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0084_projectudftracker_taskudftracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      684 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0085_auto_20201022_1822.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1569 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0086_auto_20201222_1402.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0087_auto_20210108_1214.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0087_auto_20210108_1307.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0088_merge_20210113_1743.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      988 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0089_auto_20210125_1649.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0090_auto_20210309_1157.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      637 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0091_auto_20210525_1723.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0092_auto_20210629_1124.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0093_auto_20210629_1204.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0094_auto_20210723_1018.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0094_auto_20210727_0940.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0096_merge_20210728_1429.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      862 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0097_auto_20210819_1402.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      670 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0098_auto_20211029_1641.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      704 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0099_auto_20211124_1808.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0100_auto_20211228_1443.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      589 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0101_auto_20220104_1349.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      579 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0102_auto_20220104_1655.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0103_auto_20220106_1622.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1012 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0104_rename_allocationcode_billingcode_and_more.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      782 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0105_tasknote_created_by_contact.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0106_ticketnote_created_by_contact.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0107_contact_extension.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0108_billingcodetype_billingcodetypetracker.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0109_billingcode_billing_code_type.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      638 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0110_account_phone.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      674 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0111_alter_phase_estimated_hours.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/0112_account_owner_resource.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-18 21:17:34.000000 django-autotask-1.0.0/djautotask/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    44374 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    70262 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.723753 django-autotask-1.0.0/djautotask/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/templates/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.723753 django-autotask-1.0.0/djautotask/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 21:17:57.723753 django-autotask-1.0.0/djautotask/tests/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    14124 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/fixture_utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    14344 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/fixtures.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     9091 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/mocks.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    29946 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/test_commands.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     3903 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/test_model.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    51638 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/test_sync.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)     2447 2023-04-18 21:17:40.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-04-18 21:17:56.000000 django-autotask-1.0.0/djautotask/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (122)    11695 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/fixture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39489 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8430 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6592 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31888 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3815 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53083 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2268 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2213 2023-04-18 21:17:14.000000 django-autotask-1.0.0/djautotask/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 21:17:57.723753 django-autotask-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1781 2023-04-18 21:17:14.000000 django-autotask-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0004_auto_20190913_1425.py` & `django-autotask-1.0.0/djautotask/migrations/0004_auto_20190913_1425.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0008_auto_20190917_1454.py` & `django-autotask-1.0.0/djautotask/migrations/0008_auto_20190917_1454.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0001_initial.py` & `django-autotask-1.0.0/djautotask/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0015_auto_20191001_0847.py` & `django-autotask-1.0.0/djautotask/migrations/0015_auto_20191001_0847.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0014_auto_20190930_1548.py` & `django-autotask-1.0.0/djautotask/migrations/0014_auto_20190930_1548.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0006_merge_20190920_1450.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0083_ticketudftracker.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-00000000: 160d 0d0a 81dc 935d 1f01 0000 e300 0000  .......]........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0a64 6a61 7574 6f74 6173 6bda 1730  n..djautotask..0
-000000c0: 3030 355f 6175 746f 5f32 3031 3930 3931  005_auto_2019091
-000000d0: 365f 3135 3439 da1e 3030 3035 5f72 656d  6_1549..0005_rem
-000000e0: 6f76 655f 7469 636b 6574 7374 6174 7573  ove_ticketstatus
-000000f0: 5f76 616c 7565 4e29 02fa 0a64 6a61 7574  _valueN)...djaut
-00000100: 6f74 6173 6b7a 1730 3030 355f 6175 746f  otaskz.0005_auto
-00000110: 5f32 3031 3930 3931 365f 3135 3439 2902  _20190916_1549).
-00000120: 7207 0000 0072 0600 0000 2905 da08 5f5f  r....r....)...__
-00000130: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00000140: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000150: da0c 6465 7065 6e64 656e 6369 6573 da0a  ..dependencies..
-00000160: 6f70 6572 6174 696f 6e73 a900 720d 0000  operations..r...
-00000170: 0072 0d00 0000 fa56 2f68 6f6d 652f 7361  .r.....V/home/sa
-00000180: 6d2f 6769 742f 4b61 6e62 616e 2f64 6a61  m/git/Kanban/dja
-00000190: 6e67 6f2d 6175 746f 7461 736b 2f64 6a61  ngo-autotask/dja
-000001a0: 7574 6f74 6173 6b2f 6d69 6772 6174 696f  utotask/migratio
-000001b0: 6e73 2f30 3030 365f 6d65 7267 655f 3230  ns/0006_merge_20
-000001c0: 3139 3039 3230 5f31 3435 302e 7079 7203  190920_1450.pyr.
-000001d0: 0000 0006 0000 0073 0600 0000 0c03 0301  .......s........
-000001e0: 0903 7203 0000 004e 2903 da09 646a 616e  ..r....N)...djan
-000001f0: 676f 2e64 6272 0200 0000 7203 0000 0072  go.dbr....r....r
-00000200: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000210: 0000 00da 083c 6d6f 6475 6c65 3e03 0000  .....<module>...
-00000220: 0073 0200 0000 1003                      .s......
+00000000: 550d 0d0a 0000 0000 da08 3f64 3f02 0000  U.........?d?...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0800 0000 4000 0000 7330  ..........@...s0
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0267 0064 0364 0467 0067  .e.j.d.g.d.d.g.g
+000000a0: 0064 059c 0464 0664 078d 0467 015a 0664  .d...d.d...g.Z.d
+000000b0: 0853 0029 09da 094d 6967 7261 7469 6f6e  .S.)...Migration
+000000c0: 2902 da0a 646a 6175 746f 7461 736b 5a17  )...djautotaskZ.
+000000d0: 3030 3832 5f61 7574 6f5f 3230 3230 3130  0082_auto_202010
+000000e0: 3230 5f31 3631 37da 1054 6963 6b65 7455  20_1617..TicketU
+000000f0: 4446 5472 6163 6b65 72da 1464 6a61 7574  DFTracker..djaut
+00000100: 6f74 6173 6b5f 7469 636b 6574 7564 6654  otask_ticketudfT
+00000110: 2904 da08 6462 5f74 6162 6c65 da05 7072  )...db_table..pr
+00000120: 6f78 79da 0769 6e64 6578 6573 da0b 636f  oxy..indexes..co
+00000130: 6e73 7472 6169 6e74 7329 017a 1464 6a61  nstraints).z.dja
+00000140: 7574 6f74 6173 6b2e 7469 636b 6574 7564  utotask.ticketud
+00000150: 6629 04da 046e 616d 65da 0666 6965 6c64  f)...name..field
+00000160: 73da 076f 7074 696f 6e73 da05 6261 7365  s..options..base
+00000170: 734e 2907 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
+00000180: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000190: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+000001a0: 656e 6369 6573 7202 0000 00da 0b43 7265  enciesr......Cre
+000001b0: 6174 654d 6f64 656c da0a 6f70 6572 6174  ateModel..operat
+000001c0: 696f 6e73 a900 7215 0000 0072 1500 0000  ions..r....r....
+000001d0: fa60 2f68 6f6d 652f 7275 6e6e 6572 2f77  .`/home/runner/w
+000001e0: 6f72 6b2f 646a 616e 676f 2d61 7574 6f74  ork/django-autot
+000001f0: 6173 6b2f 646a 616e 676f 2d61 7574 6f74  ask/django-autot
+00000200: 6173 6b2f 646a 6175 746f 7461 736b 2f6d  ask/djautotask/m
+00000210: 6967 7261 7469 6f6e 732f 3030 3833 5f74  igrations/0083_t
+00000220: 6963 6b65 7475 6466 7472 6163 6b65 722e  icketudftracker.
+00000230: 7079 7203 0000 0006 0000 0073 1a00 0000  pyr........s....
+00000240: 0803 02ff 0405 0401 0201 0203 0201 0201  ................
+00000250: 0201 02fc 0406 02f6 04ff 7203 0000 004e  ..........r....N
+00000260: 2903 da09 646a 616e 676f 2e64 6272 0200  )...django.dbr..
+00000270: 0000 7203 0000 0072 1500 0000 7215 0000  ..r....r....r...
+00000280: 0072 1500 0000 7216 0000 00da 083c 6d6f  .r....r......<mo
+00000290: 6475 6c65 3e03 0000 0073 0200 0000 0c03  dule>....s......
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0008_merge_20190920_1644.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0090_auto_20210309_1157.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-00000000: 160d 0d0a 81dc 935d 1901 0000 e300 0000  .......]........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0a64 6a61 7574 6f74 6173 6bda 1730  n..djautotask..0
-000000c0: 3030 375f 6175 746f 5f32 3031 3930 3931  007_auto_2019091
-000000d0: 375f 3130 3039 da18 3030 3036 5f6d 6572  7_1009..0006_mer
-000000e0: 6765 5f32 3031 3930 3932 305f 3134 3530  ge_20190920_1450
-000000f0: 4e29 02fa 0a64 6a61 7574 6f74 6173 6b72  N)...djautotaskr
-00000100: 0500 0000 2902 7207 0000 007a 1830 3030  ....).r....z.000
-00000110: 365f 6d65 7267 655f 3230 3139 3039 3230  6_merge_20190920
-00000120: 5f31 3435 3029 05da 085f 5f6e 616d 655f  _1450)...__name_
-00000130: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000140: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-00000150: 656e 6465 6e63 6965 73da 0a6f 7065 7261  endencies..opera
-00000160: 7469 6f6e 73a9 0072 0d00 0000 720d 0000  tions..r....r...
-00000170: 00fa 562f 686f 6d65 2f73 616d 2f67 6974  ..V/home/sam/git
-00000180: 2f4b 616e 6261 6e2f 646a 616e 676f 2d61  /Kanban/django-a
-00000190: 7574 6f74 6173 6b2f 646a 6175 746f 7461  utotask/djautota
-000001a0: 736b 2f6d 6967 7261 7469 6f6e 732f 3030  sk/migrations/00
-000001b0: 3038 5f6d 6572 6765 5f32 3031 3930 3932  08_merge_2019092
-000001c0: 305f 3136 3434 2e70 7972 0300 0000 0600  0_1644.pyr......
-000001d0: 0000 7306 0000 000c 0303 0109 0372 0300  ..s..........r..
-000001e0: 0000 4e29 03da 0964 6a61 6e67 6f2e 6462  ..N)...django.db
-000001f0: 7202 0000 0072 0300 0000 720d 0000 0072  r....r....r....r
-00000200: 0d00 0000 720d 0000 0072 0e00 0000 da08  ....r....r......
-00000210: 3c6d 6f64 756c 653e 0300 0000 7302 0000  <module>....s...
-00000220: 0010 03                                  ...
+00000000: 550d 0d0a 0000 0000 da08 3f64 a901 0000  U.........?d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0500 0000 4000 0000 7328  ..........@...s(
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0264 0364 0464 059c 0264  .e.j.d.d.d.d...d
+000000a0: 068d 0267 015a 0664 0753 0029 08da 094d  ...g.Z.d.S.)...M
+000000b0: 6967 7261 7469 6f6e 2902 da0a 646a 6175  igration)...djau
+000000c0: 746f 7461 736b 5a17 3030 3839 5f61 7574  totaskZ.0089_aut
+000000d0: 6f5f 3230 3231 3031 3235 5f31 3634 39da  o_20210125_1649.
+000000e0: 0974 696d 6565 6e74 7279 2903 7a10 2d73  .timeentry).z.-s
+000000f0: 7461 7274 5f64 6174 655f 7469 6d65 7a0c  tart_date_timez.
+00000100: 2d64 6174 655f 776f 726b 6564 7a03 2d69  -date_workedz.-i
+00000110: 647a 0c54 696d 6520 656e 7472 6965 7329  dz.Time entries)
+00000120: 02da 086f 7264 6572 696e 67da 1376 6572  ...ordering..ver
+00000130: 626f 7365 5f6e 616d 655f 706c 7572 616c  bose_name_plural
+00000140: 2902 da04 6e61 6d65 da07 6f70 7469 6f6e  )...name..option
+00000150: 734e 2907 da08 5f5f 6e61 6d65 5f5f da0a  sN)...__name__..
+00000160: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00000170: 616c 6e61 6d65 5f5f da0c 6465 7065 6e64  alname__..depend
+00000180: 656e 6369 6573 7202 0000 00da 1141 6c74  enciesr......Alt
+00000190: 6572 4d6f 6465 6c4f 7074 696f 6e73 da0a  erModelOptions..
+000001a0: 6f70 6572 6174 696f 6e73 a900 7210 0000  operations..r...
+000001b0: 0072 1000 0000 fa62 2f68 6f6d 652f 7275  .r.....b/home/ru
+000001c0: 6e6e 6572 2f77 6f72 6b2f 646a 616e 676f  nner/work/django
+000001d0: 2d61 7574 6f74 6173 6b2f 646a 616e 676f  -autotask/django
+000001e0: 2d61 7574 6f74 6173 6b2f 646a 6175 746f  -autotask/djauto
+000001f0: 7461 736b 2f6d 6967 7261 7469 6f6e 732f  task/migrations/
+00000200: 3030 3930 5f61 7574 6f5f 3230 3231 3033  0090_auto_202103
+00000210: 3039 5f31 3135 372e 7079 7203 0000 0006  09_1157.pyr.....
+00000220: 0000 0073 0e00 0000 0803 02ff 0405 0401  ...s............
+00000230: 0201 08fe 04ff 7203 0000 004e 2903 da09  ......r....N)...
+00000240: 646a 616e 676f 2e64 6272 0200 0000 7203  django.dbr....r.
+00000250: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+00000260: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000270: 3e03 0000 0073 0200 0000 0c03            >....s......
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0010_merge_20190923_1155.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0027_auto_20191125_1103.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-00000000: 160d 0d0a 81dc 935d 1801 0000 e300 0000  .......]........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0003 0000 0040 0000 0073 2200  .........@...s".
-00000080: 0000 6500 005a 0100 6400 005a 0200 6405  ..e..Z..d..Z..d.
-00000090: 0064 0600 6702 005a 0300 6700 005a 0400  .d..g..Z..g..Z..
-000000a0: 6404 0053 2907 da09 4d69 6772 6174 696f  d..S)...Migratio
-000000b0: 6eda 0a64 6a61 7574 6f74 6173 6bda 1730  n..djautotask..0
-000000c0: 3030 385f 6175 746f 5f32 3031 3930 3931  008_auto_2019091
-000000d0: 375f 3134 3534 da17 3030 3039 5f61 7574  7_1454..0009_aut
-000000e0: 6f5f 3230 3139 3039 3230 5f31 3634 384e  o_20190920_1648N
-000000f0: 2902 fa0a 646a 6175 746f 7461 736b 7205  )...djautotaskr.
-00000100: 0000 0029 0272 0700 0000 7a17 3030 3039  ...).r....z.0009
-00000110: 5f61 7574 6f5f 3230 3139 3039 3230 5f31  _auto_20190920_1
-00000120: 3634 3829 05da 085f 5f6e 616d 655f 5fda  648)...__name__.
-00000130: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000140: 7561 6c6e 616d 655f 5fda 0c64 6570 656e  ualname__..depen
-00000150: 6465 6e63 6965 73da 0a6f 7065 7261 7469  dencies..operati
-00000160: 6f6e 73a9 0072 0d00 0000 720d 0000 00fa  ons..r....r.....
-00000170: 562f 686f 6d65 2f73 616d 2f67 6974 2f4b  V/home/sam/git/K
-00000180: 616e 6261 6e2f 646a 616e 676f 2d61 7574  anban/django-aut
-00000190: 6f74 6173 6b2f 646a 6175 746f 7461 736b  otask/djautotask
-000001a0: 2f6d 6967 7261 7469 6f6e 732f 3030 3130  /migrations/0010
-000001b0: 5f6d 6572 6765 5f32 3031 3930 3932 335f  _merge_20190923_
-000001c0: 3131 3535 2e70 7972 0300 0000 0600 0000  1155.pyr........
-000001d0: 7306 0000 000c 0303 0109 0372 0300 0000  s..........r....
-000001e0: 4e29 03da 0964 6a61 6e67 6f2e 6462 7202  N)...django.dbr.
-000001f0: 0000 0072 0300 0000 720d 0000 0072 0d00  ...r....r....r..
-00000200: 0000 720d 0000 0072 0e00 0000 da08 3c6d  ..r....r......<m
-00000210: 6f64 756c 653e 0300 0000 7302 0000 0010  odule>....s.....
-00000220: 03                                       .
+00000000: 550d 0d0a 0000 0000 da08 3f64 7701 0000  U.........?dw...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0500 0000 4000 0000 7324  ..........@...s$
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0264 0364 0464 058d 0367  .e.j.d.d.d.d...g
+000000a0: 015a 0664 0653 0029 07da 094d 6967 7261  .Z.d.S.)...Migra
+000000b0: 7469 6f6e 2902 da0a 646a 6175 746f 7461  tion)...djautota
+000000c0: 736b da17 3030 3236 5f61 7574 6f5f 3230  sk..0026_auto_20
+000000d0: 3139 3131 3235 5f30 3935 32da 0474 6173  191125_0952..tas
+000000e0: 6bda 0e70 7269 6f72 6974 795f 6c61 6265  k..priority_labe
+000000f0: 6cda 0870 7269 6f72 6974 7929 03da 0a6d  l..priority)...m
+00000100: 6f64 656c 5f6e 616d 65da 086f 6c64 5f6e  odel_name..old_n
+00000110: 616d 65da 086e 6577 5f6e 616d 654e 2907  ame..new_nameN).
+00000120: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000130: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000140: 6d65 5f5f da0c 6465 7065 6e64 656e 6369  me__..dependenci
+00000150: 6573 7202 0000 00da 0b52 656e 616d 6546  esr......RenameF
+00000160: 6965 6c64 da0a 6f70 6572 6174 696f 6e73  ield..operations
+00000170: a900 7212 0000 0072 1200 0000 fa62 2f68  ..r....r.....b/h
+00000180: 6f6d 652f 7275 6e6e 6572 2f77 6f72 6b2f  ome/runner/work/
+00000190: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001a0: 646a 616e 676f 2d61 7574 6f74 6173 6b2f  django-autotask/
+000001b0: 646a 6175 746f 7461 736b 2f6d 6967 7261  djautotask/migra
+000001c0: 7469 6f6e 732f 3030 3237 5f61 7574 6f5f  tions/0027_auto_
+000001d0: 3230 3139 3131 3235 5f31 3130 332e 7079  20191125_1103.py
+000001e0: 7203 0000 0006 0000 0073 1000 0000 0803  r........s......
+000001f0: 02ff 0405 0401 0201 0201 02fd 04ff 7203  ..............r.
+00000200: 0000 004e 2903 da09 646a 616e 676f 2e64  ...N)...django.d
+00000210: 6272 0200 0000 7203 0000 0072 1200 0000  br....r....r....
+00000220: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00000230: 083c 6d6f 6475 6c65 3e03 0000 0073 0200  .<module>....s..
+00000240: 0000 0c03                                ....
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0011_auto_20190923_1157.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0095_auto_20210726_1251.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 160d 0d0a 81dc 935d 6801 0000 e300 0000  .......]h.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0006 0000 0040 0000 0073 3a00  .........@...s:.
-00000080: 0000 6500 005a 0100 6400 005a 0200 6409  ..e..Z..d..Z..d.
-00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
-000000a0: 6404 0064 0500 6406 0064 0700 6901 0083  d..d..d..d..i...
-000000b0: 0002 6701 005a 0600 6408 0053 290a da09  ..g..Z..d..S)...
-000000c0: 4d69 6772 6174 696f 6eda 0a64 6a61 7574  Migration..djaut
-000000d0: 6f74 6173 6bda 1830 3031 305f 6d65 7267  otask..0010_merg
-000000e0: 655f 3230 3139 3039 3233 5f31 3135 35da  e_20190923_1155.
-000000f0: 046e 616d 65da 0571 7565 7565 da07 6f70  .name..queue..op
-00000100: 7469 6f6e 73da 1376 6572 626f 7365 5f6e  tions..verbose_n
-00000110: 616d 655f 706c 7572 616c da06 5175 6575  ame_plural..Queu
-00000120: 6573 4e29 027a 0a64 6a61 7574 6f74 6173  esN).z.djautotas
-00000130: 6b72 0500 0000 2907 da08 5f5f 6e61 6d65  kr....)...__name
-00000140: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00000150: 5f5f 7175 616c 6e61 6d65 5f5f da0c 6465  __qualname__..de
-00000160: 7065 6e64 656e 6369 6573 7202 0000 00da  pendenciesr.....
-00000170: 1141 6c74 6572 4d6f 6465 6c4f 7074 696f  .AlterModelOptio
-00000180: 6e73 da0a 6f70 6572 6174 696f 6e73 a900  ns..operations..
-00000190: 7211 0000 0072 1100 0000 fa55 2f68 6f6d  r....r.....U/hom
-000001a0: 652f 7361 6d2f 6769 742f 4b61 6e62 616e  e/sam/git/Kanban
-000001b0: 2f64 6a61 6e67 6f2d 6175 746f 7461 736b  /django-autotask
-000001c0: 2f64 6a61 7574 6f74 6173 6b2f 6d69 6772  /djautotask/migr
-000001d0: 6174 696f 6e73 2f30 3031 315f 6175 746f  ations/0011_auto
-000001e0: 5f32 3031 3930 3932 335f 3131 3537 2e70  _20190923_1157.p
-000001f0: 7972 0300 0000 0600 0000 7308 0000 000c  yr........s.....
-00000200: 0309 0409 0106 0172 0300 0000 4e29 03da  .......r....N)..
-00000210: 0964 6a61 6e67 6f2e 6462 7202 0000 0072  .django.dbr....r
-00000220: 0300 0000 7211 0000 0072 1100 0000 7211  ....r....r....r.
-00000230: 0000 0072 1200 0000 da08 3c6d 6f64 756c  ...r......<modul
-00000240: 653e 0300 0000 7302 0000 0010 03         e>....s......
+00000000: 550d 0d0a 0000 0000 da08 3f64 7001 0000  U.........?dp...
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0400 0000 4000 0000 7326  ..........@...s&
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0264 0364 0469 0164 058d  .e.j.d.d.d.i.d..
+000000a0: 0267 015a 0664 0653 0029 07da 094d 6967  .g.Z.d.S.)...Mig
+000000b0: 7261 7469 6f6e 2902 da0a 646a 6175 746f  ration)...djauto
+000000c0: 7461 736b 5a17 3030 3934 5f61 7574 6f5f  taskZ.0094_auto_
+000000d0: 3230 3231 3037 3233 5f31 3031 38da 0763  20210723_1018..c
+000000e0: 6f6e 7461 6374 da08 6f72 6465 7269 6e67  ontact..ordering
+000000f0: 2902 da0a 6669 7273 745f 6e61 6d65 da09  )...first_name..
+00000100: 6c61 7374 5f6e 616d 6529 02da 046e 616d  last_name)...nam
+00000110: 65da 076f 7074 696f 6e73 4e29 07da 085f  e..optionsN)..._
+00000120: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00000130: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00000140: 5fda 0c64 6570 656e 6465 6e63 6965 7372  _..dependenciesr
+00000150: 0200 0000 da11 416c 7465 724d 6f64 656c  ......AlterModel
+00000160: 4f70 7469 6f6e 73da 0a6f 7065 7261 7469  Options..operati
+00000170: 6f6e 73a9 0072 1100 0000 7211 0000 00fa  ons..r....r.....
+00000180: 622f 686f 6d65 2f72 756e 6e65 722f 776f  b/home/runner/wo
+00000190: 726b 2f64 6a61 6e67 6f2d 6175 746f 7461  rk/django-autota
+000001a0: 736b 2f64 6a61 6e67 6f2d 6175 746f 7461  sk/django-autota
+000001b0: 736b 2f64 6a61 7574 6f74 6173 6b2f 6d69  sk/djautotask/mi
+000001c0: 6772 6174 696f 6e73 2f30 3039 355f 6175  grations/0095_au
+000001d0: 746f 5f32 3032 3130 3732 365f 3132 3531  to_20210726_1251
+000001e0: 2e70 7972 0300 0000 0600 0000 730e 0000  .pyr........s...
+000001f0: 0008 0302 ff04 0504 0102 0106 fe04 ff72  ...............r
+00000200: 0300 0000 4e29 03da 0964 6a61 6e67 6f2e  ....N)...django.
+00000210: 6462 7202 0000 0072 0300 0000 7211 0000  dbr....r....r...
+00000220: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000230: da08 3c6d 6f64 756c 653e 0300 0000 7302  ..<module>....s.
+00000240: 0000 000c 03                             .....
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0005_remove_ticketstatus_value.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0009_auto_20190920_1648.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-00000000: 160d 0d0a 81dc 935d 5101 0000 e300 0000  .......]Q.......
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 2d00 0000 6400 0064 0100 6c00 006d  .s-...d..d..l..m
-00000030: 0100 5a01 0001 4764 0200 6403 0084 0000  ..Z...Gd..d.....
-00000040: 6403 0065 0100 6a02 0083 0300 5a02 0064  d..e..j.....Z..d
-00000050: 0400 5329 05e9 0000 0000 2901 da0a 6d69  ..S)......)...mi
-00000060: 6772 6174 696f 6e73 6300 0000 0000 0000  grationsc.......
-00000070: 0000 0000 0005 0000 0040 0000 0073 3400  .........@...s4.
-00000080: 0000 6500 005a 0100 6400 005a 0200 6408  ..e..Z..d..Z..d.
-00000090: 0067 0100 5a03 0065 0400 6a05 0064 0300  .g..Z..e..j..d..
-000000a0: 6404 0064 0500 6406 0083 0002 6701 005a  d..d..d.....g..Z
-000000b0: 0600 6407 0053 2909 da09 4d69 6772 6174  ..d..S)...Migrat
-000000c0: 696f 6eda 0a64 6a61 7574 6f74 6173 6bda  ion..djautotask.
-000000d0: 1730 3030 345f 6175 746f 5f32 3031 3930  .0004_auto_20190
-000000e0: 3931 335f 3134 3235 da0a 6d6f 6465 6c5f  913_1425..model_
-000000f0: 6e61 6d65 da0c 7469 636b 6574 7374 6174  name..ticketstat
-00000100: 7573 da04 6e61 6d65 da05 7661 6c75 654e  us..name..valueN
-00000110: 2902 7a0a 646a 6175 746f 7461 736b 7a17  ).z.djautotaskz.
-00000120: 3030 3034 5f61 7574 6f5f 3230 3139 3039  0004_auto_201909
-00000130: 3133 5f31 3432 3529 07da 085f 5f6e 616d  13_1425)...__nam
-00000140: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000150: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
-00000160: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
-00000170: da0b 5265 6d6f 7665 4669 656c 64da 0a6f  ..RemoveField..o
-00000180: 7065 7261 7469 6f6e 73a9 0072 1000 0000  perations..r....
-00000190: 7210 0000 00fa 5c2f 686f 6d65 2f73 616d  r.....\/home/sam
-000001a0: 2f67 6974 2f4b 616e 6261 6e2f 646a 616e  /git/Kanban/djan
-000001b0: 676f 2d61 7574 6f74 6173 6b2f 646a 6175  go-autotask/djau
-000001c0: 746f 7461 736b 2f6d 6967 7261 7469 6f6e  totask/migration
-000001d0: 732f 3030 3035 5f72 656d 6f76 655f 7469  s/0005_remove_ti
-000001e0: 636b 6574 7374 6174 7573 5f76 616c 7565  cketstatus_value
-000001f0: 2e70 7972 0300 0000 0600 0000 7308 0000  .pyr........s...
-00000200: 000c 0309 0409 0106 0172 0300 0000 4e29  .........r....N)
-00000210: 03da 0964 6a61 6e67 6f2e 6462 7202 0000  ...django.dbr...
-00000220: 0072 0300 0000 7210 0000 0072 1000 0000  .r....r....r....
-00000230: 7210 0000 0072 1100 0000 da08 3c6d 6f64  r....r......<mod
-00000240: 756c 653e 0300 0000 7302 0000 0010 03    ule>....s......
+00000000: 550d 0d0a 0000 0000 da08 3f64 b901 0000  U.........?d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2200 0000 6400  .....@...s"...d.
+00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
+00000040: 8400 6403 6501 6a02 8303 5a02 6404 5300  ..d.e.j...Z.d.S.
+00000050: 2905 e900 0000 0029 01da 0a6d 6967 7261  )......)...migra
+00000060: 7469 6f6e 7363 0000 0000 0000 0000 0000  tionsc..........
+00000070: 0000 0000 0000 0500 0000 4000 0000 732e  ..........@...s.
+00000080: 0000 0065 005a 0164 005a 0264 0167 015a  ...e.Z.d.Z.d.g.Z
+00000090: 0365 046a 0564 0264 0364 048d 0265 046a  .e.j.d.d.d...e.j
+000000a0: 0564 0564 0364 048d 0267 025a 0664 0653  .d.d.d...g.Z.d.S
+000000b0: 0029 07da 094d 6967 7261 7469 6f6e 2902  .)...Migration).
+000000c0: da0a 646a 6175 746f 7461 736b 5a18 3030  ..djautotaskZ.00
+000000d0: 3038 5f6d 6572 6765 5f32 3031 3930 3932  08_merge_2019092
+000000e0: 305f 3136 3434 da05 7175 6575 65da 0576  0_1644..queue..v
+000000f0: 616c 7565 2902 da0a 6d6f 6465 6c5f 6e61  alue)...model_na
+00000100: 6d65 da04 6e61 6d65 da0e 7469 636b 6574  me..name..ticket
+00000110: 7072 696f 7269 7479 4e29 07da 085f 5f6e  priorityN)...__n
+00000120: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+00000130: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5fda  _..__qualname__.
+00000140: 0c64 6570 656e 6465 6e63 6965 7372 0200  .dependenciesr..
+00000150: 0000 da0b 5265 6d6f 7665 4669 656c 64da  ....RemoveField.
+00000160: 0a6f 7065 7261 7469 6f6e 73a9 0072 1000  .operations..r..
+00000170: 0000 7210 0000 00fa 622f 686f 6d65 2f72  ..r.....b/home/r
+00000180: 756e 6e65 722f 776f 726b 2f64 6a61 6e67  unner/work/djang
+00000190: 6f2d 6175 746f 7461 736b 2f64 6a61 6e67  o-autotask/djang
+000001a0: 6f2d 6175 746f 7461 736b 2f64 6a61 7574  o-autotask/djaut
+000001b0: 6f74 6173 6b2f 6d69 6772 6174 696f 6e73  otask/migrations
+000001c0: 2f30 3030 395f 6175 746f 5f32 3031 3930  /0009_auto_20190
+000001d0: 3932 305f 3136 3438 2e70 7972 0300 0000  920_1648.pyr....
+000001e0: 0600 0000 7316 0000 0008 0302 ff04 0504  ....s...........
+000001f0: 0102 0102 fe04 0404 0102 0102 fe04 fb72  ...............r
+00000200: 0300 0000 4e29 03da 0964 6a61 6e67 6f2e  ....N)...django.
+00000210: 6462 7202 0000 0072 0300 0000 7210 0000  dbr....r....r...
+00000220: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00000230: da08 3c6d 6f64 756c 653e 0300 0000 7302  ..<module>....s.
+00000240: 0000 000c 03                             .....
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/__pycache__/0002_ticket_ticket_number.cpython-35.pyc` & `django-autotask-1.0.0/djautotask/migrations/__pycache__/0052_contract_status.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.5.1- byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-00000000: 160d 0d0a 81dc 935d 9701 0000 e300 0000  .......]........
-00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-00000020: 0073 3300 0000 6400 0064 0100 6c00 006d  .s3...d..d..l..m
-00000030: 0100 5a01 006d 0200 5a02 0001 4764 0200  ..Z..m..Z...Gd..
-00000040: 6403 0084 0000 6403 0065 0100 6a03 0083  d.....d..e..j...
-00000050: 0300 5a03 0064 0400 5329 05e9 0000 0000  ..Z..d..S)......
-00000060: 2902 da0a 6d69 6772 6174 696f 6e73 da06  )...migrations..
-00000070: 6d6f 6465 6c73 6300 0000 0000 0000 0000  modelsc.........
-00000080: 0000 000d 0000 0040 0000 0073 5200 0000  .......@...sR...
-00000090: 6500 005a 0100 6400 005a 0200 640e 0067  e..Z..d..Z..d..g
-000000a0: 0100 5a03 0065 0400 6a05 0064 0300 6404  ..Z..e..j..d..d.
-000000b0: 0064 0500 6406 0064 0700 6506 006a 0700  .d..d..d..e..j..
-000000c0: 6408 0064 0900 640a 0064 0b00 640c 0064  d..d..d..d..d..d
-000000d0: 0900 8300 0383 0003 6701 005a 0800 640d  ........g..Z..d.
-000000e0: 0053 290f da09 4d69 6772 6174 696f 6eda  .S)...Migration.
-000000f0: 0a64 6a61 7574 6f74 6173 6bda 0c30 3030  .djautotask..000
-00000100: 315f 696e 6974 6961 6cda 0a6d 6f64 656c  1_initial..model
-00000110: 5f6e 616d 65da 0674 6963 6b65 74da 046e  _name..ticket..n
-00000120: 616d 65da 0d74 6963 6b65 745f 6e75 6d62  ame..ticket_numb
-00000130: 6572 da05 6669 656c 64da 0562 6c61 6e6b  er..field..blank
-00000140: 54da 0a6d 6178 5f6c 656e 6774 68e9 3200  T..max_length.2.
-00000150: 0000 da04 6e75 6c6c 4e29 027a 0a64 6a61  ....nullN).z.dja
-00000160: 7574 6f74 6173 6b7a 0c30 3030 315f 696e  utotaskz.0001_in
-00000170: 6974 6961 6c29 09da 085f 5f6e 616d 655f  itial)...__name_
-00000180: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000190: 5f71 7561 6c6e 616d 655f 5fda 0c64 6570  _qualname__..dep
-000001a0: 656e 6465 6e63 6965 7372 0200 0000 da08  endenciesr......
-000001b0: 4164 6446 6965 6c64 7203 0000 00da 0943  AddFieldr......C
-000001c0: 6861 7246 6965 6c64 da0a 6f70 6572 6174  harField..operat
-000001d0: 696f 6e73 a900 7217 0000 0072 1700 0000  ions..r....r....
-000001e0: fa57 2f68 6f6d 652f 7361 6d2f 6769 742f  .W/home/sam/git/
-000001f0: 4b61 6e62 616e 2f64 6a61 6e67 6f2d 6175  Kanban/django-au
-00000200: 746f 7461 736b 2f64 6a61 7574 6f74 6173  totask/djautotas
-00000210: 6b2f 6d69 6772 6174 696f 6e73 2f30 3030  k/migrations/000
-00000220: 325f 7469 636b 6574 5f74 6963 6b65 745f  2_ticket_ticket_
-00000230: 6e75 6d62 6572 2e70 7972 0400 0000 0600  number.pyr......
-00000240: 0000 730a 0000 000c 0309 0409 0106 0106  ..s.............
-00000250: 0172 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
+00000000: 550d 0d0a 0000 0000 da08 3f64 bd01 0000  U.........?d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 4700  d.l.m.Z.m.Z...G.
+00000040: 6402 6403 8400 6403 6501 6a03 8303 5a03  d.d...d.e.j...Z.
+00000050: 6404 5300 2905 e900 0000 0029 02da 0a6d  d.S.)......)...m
+00000060: 6967 7261 7469 6f6e 73da 066d 6f64 656c  igrations..model
+00000070: 7363 0000 0000 0000 0000 0000 0000 0000  sc..............
+00000080: 0000 0900 0000 4000 0000 7336 0000 0065  ......@...s6...e
+00000090: 005a 0164 005a 0264 0167 015a 0365 046a  .Z.d.Z.d.g.Z.e.j
+000000a0: 0564 0264 0365 066a 0764 0464 0564 0667  .d.d.e.j.d.d.d.g
+000000b0: 0264 0764 0464 088d 0464 098d 0367 015a  .d.d.d...d...g.Z
+000000c0: 0864 0a53 0029 0bda 094d 6967 7261 7469  .d.S.)...Migrati
+000000d0: 6f6e 2902 da0a 646a 6175 746f 7461 736b  on)...djautotask
+000000e0: 5a0d 3030 3531 5f63 6f6e 7472 6163 74da  Z.0051_contract.
+000000f0: 0863 6f6e 7472 6163 74da 0673 7461 7475  .contract..statu
+00000100: 7354 2902 7201 0000 00da 0849 6e61 6374  sT).r......Inact
+00000110: 6976 6529 02e9 0100 0000 da06 4163 7469  ive)........Acti
+00000120: 7665 e914 0000 0029 04da 0562 6c61 6e6b  ve.....)...blank
+00000130: da07 6368 6f69 6365 73da 0a6d 6178 5f6c  ..choices..max_l
+00000140: 656e 6774 68da 046e 756c 6c29 03da 0a6d  ength..null)...m
+00000150: 6f64 656c 5f6e 616d 65da 046e 616d 65da  odel_name..name.
+00000160: 0566 6965 6c64 4e29 09da 085f 5f6e 616d  .fieldN)...__nam
+00000170: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000180: 0c5f 5f71 7561 6c6e 616d 655f 5fda 0c64  .__qualname__..d
+00000190: 6570 656e 6465 6e63 6965 7372 0200 0000  ependenciesr....
+000001a0: da08 4164 6446 6965 6c64 7203 0000 00da  ..AddFieldr.....
+000001b0: 0943 6861 7246 6965 6c64 da0a 6f70 6572  .CharField..oper
+000001c0: 6174 696f 6e73 a900 721a 0000 0072 1a00  ations..r....r..
+000001d0: 0000 fa5f 2f68 6f6d 652f 7275 6e6e 6572  ..._/home/runner
+000001e0: 2f77 6f72 6b2f 646a 616e 676f 2d61 7574  /work/django-aut
+000001f0: 6f74 6173 6b2f 646a 616e 676f 2d61 7574  otask/django-aut
+00000200: 6f74 6173 6b2f 646a 6175 746f 7461 736b  otask/djautotask
+00000210: 2f6d 6967 7261 7469 6f6e 732f 3030 3532  /migrations/0052
+00000220: 5f63 6f6e 7472 6163 745f 7374 6174 7573  _contract_status
+00000230: 2e70 7972 0400 0000 0600 0000 7310 0000  .pyr........s...
+00000240: 0008 0302 ff04 0504 0102 0102 0114 fd04  ................
+00000250: ff72 0400 0000 4e29 04da 0964 6a61 6e67  .r....N)...djang
 00000260: 6f2e 6462 7202 0000 0072 0300 0000 7204  o.dbr....r....r.
-00000270: 0000 0072 1700 0000 7217 0000 0072 1700  ...r....r....r..
-00000280: 0000 7218 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000290: 3e03 0000 0073 0200 0000 1603            >....s......
+00000270: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00000280: 0000 721b 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000290: 3e03 0000 0073 0200 0000 1003            >....s......
```

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0007_auto_20190917_1009.py` & `django-autotask-1.0.0/djautotask/migrations/0007_auto_20190917_1009.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0009_auto_20190918_1525.py` & `django-autotask-1.0.0/djautotask/migrations/0009_auto_20190918_1525.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0010_auto_20190923_0930.py` & `django-autotask-1.0.0/djautotask/migrations/0010_auto_20190923_0930.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0006_auto_20190916_1645.py` & `django-autotask-1.0.0/djautotask/migrations/0006_auto_20190916_1645.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0003_auto_20190913_0941.py` & `django-autotask-1.0.0/djautotask/migrations/0003_auto_20190913_0941.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/djautotask/migrations/0005_auto_20190916_1549.py` & `django-autotask-1.0.0/djautotask/migrations/0005_auto_20190916_1549.py`

 * *Files identical despite different names*

### Comparing `django-autotask-0.0.9a0/setup.py` & `django-autotask-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,30 +10,29 @@
     name='django-autotask',
     version=djautotask.__version__,
     description='Django app for working with Autotask. '
                 'Defines models (tickets, members, companies, etc.) '
                 'and callbacks.',
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/markdown',
-    keywords='django autotask soap api python',
+    keywords='django autotask rest api python',
     packages=find_packages(),
     author='Kerkhoff Technologies Inc.',
     author_email='matt@kerkhofftech.ca',
     url="https://github.com/KerkhoffTechnologies/django-autotask",
     include_package_data=True,
     license='MIT',
     install_requires=[
         'requests',
         'django',
         'python-dateutil',
         'django-model-utils',
         'django-braces',
         'django-extensions',
         'retrying',
-        'atws',
     ],
     test_suite='runtests.suite',
     tests_require=[
         'responses',
         'model-mommy',
         'django-coverage',
         'names'
```

### Comparing `django-autotask-0.0.9a0/PKG-INFO` & `django-autotask-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 0.0.9a0
+Version: 1.0.0
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
         
         Django app for working with Autotask. Defines models (tickets,
-        members, companies, etc.).
+        resources, accounts, etc.).
         
         ## Requirements
         
         -  Python 3.5
         -  Django 2.0
         
         Other versions may work; we haven't tried.
@@ -30,15 +30,14 @@
         
         1. Add to INSTALLED_APPS
         
             ```
             INSTALLED_APPS = [
                 ...
                 'djautotask',
-                'easy_thumbnails'  # Used for managing user pictures
                 ...
             ]
             ```
         
         
         ## Testing
         
@@ -71,15 +70,15 @@
         
         MIT
         
         ## Copyright
         
         ©2018 Kerkhoff Technologies Inc.
         
-Keywords: django autotask soap api python
+Keywords: django autotask rest api python
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `django-autotask-0.0.9a0/django_autotask.egg-info/PKG-INFO` & `django-autotask-1.0.0/django_autotask.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: django-autotask
-Version: 0.0.9a0
+Version: 1.0.0
 Summary: Django app for working with Autotask. Defines models (tickets, members, companies, etc.) and callbacks.
 Home-page: https://github.com/KerkhoffTechnologies/django-autotask
 Author: Kerkhoff Technologies Inc.
 Author-email: matt@kerkhofftech.ca
 License: MIT
 Description: ## django-autotask
         
         Django app for working with Autotask. Defines models (tickets,
-        members, companies, etc.).
+        resources, accounts, etc.).
         
         ## Requirements
         
         -  Python 3.5
         -  Django 2.0
         
         Other versions may work; we haven't tried.
@@ -30,15 +30,14 @@
         
         1. Add to INSTALLED_APPS
         
             ```
             INSTALLED_APPS = [
                 ...
                 'djautotask',
-                'easy_thumbnails'  # Used for managing user pictures
                 ...
             ]
             ```
         
         
         ## Testing
         
@@ -71,15 +70,15 @@
         
         MIT
         
         ## Copyright
         
         ©2018 Kerkhoff Technologies Inc.
         
-Keywords: django autotask soap api python
+Keywords: django autotask rest api python
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `django-autotask-0.0.9a0/README.md` & `django-autotask-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ## django-autotask
 
 Django app for working with Autotask. Defines models (tickets,
-members, companies, etc.).
+resources, accounts, etc.).
 
 ## Requirements
 
 -  Python 3.5
 -  Django 2.0
 
 Other versions may work; we haven't tried.
@@ -22,15 +22,14 @@
 
 1. Add to INSTALLED_APPS
 
     ```
     INSTALLED_APPS = [
         ...
         'djautotask',
-        'easy_thumbnails'  # Used for managing user pictures
         ...
     ]
     ```
 
 
 ## Testing
```

