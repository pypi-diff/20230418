# Comparing `tmp/tago-3.1.0.tar.gz` & `tmp/tago-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tago-3.1.0.tar", last modified: Thu Feb 23 20:32:15 2023, max compression
+gzip compressed data, was "tago-3.1.1.tar", last modified: Tue Apr 18 15:39:08 2023, max compression
```

## Comparing `tago-3.1.0.tar` & `tago-3.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.388386 tago-3.1.0/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)    10753 2021-04-28 16:53:14.000000 tago-3.1.0/LICENSE.md
--rw-rw-rw-   0 felipefdl   (501) staff       (20)       14 2021-04-28 16:53:14.000000 tago-3.1.0/MANIFEST.in
--rw-r--r--   0 felipefdl   (501) staff       (20)     1748 2023-02-23 20:32:15.388545 tago-3.1.0/PKG-INFO
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1148 2021-04-28 16:53:14.000000 tago-3.1.0/README.md
--rw-r--r--   0 felipefdl   (501) staff       (20)       84 2023-02-23 20:25:39.000000 tago-3.1.0/requirements.txt
--rw-rw-rw-   0 felipefdl   (501) staff       (20)       79 2023-02-23 20:32:15.388920 tago-3.1.0/setup.cfg
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      931 2023-02-23 20:26:03.000000 tago-3.1.0/setup.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.377873 tago-3.1.0/tago/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      247 2021-04-28 16:53:14.000000 tago-3.1.0/tago/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.384558 tago-3.1.0/tago/account/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     6448 2021-10-22 14:06:06.000000 tago-3.1.0/tago/account/__init__.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1407 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/_share.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1726 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/accessManagement.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1665 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/actions.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     2643 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/analysis.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     4373 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/buckets.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     2723 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/connector.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     4728 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/dashboards.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     3850 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/dashboards_widgets.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     3932 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/devices.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      784 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/explore.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1995 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/files.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     2916 2021-10-22 14:06:06.000000 tago-3.1.0/tago/account/integration_network.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     2230 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/notifications.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      622 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/paymentHistory.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1255 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/paymentMethods.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1285 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/plan.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     4827 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/profiles.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     3365 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/run.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1560 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/service_authorization.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      715 2021-04-28 16:53:14.000000 tago-3.1.0/tago/account/socket.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      622 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/tags.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1193 2021-08-12 17:43:30.000000 tago-3.1.0/tago/account/template.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.384752 tago-3.1.0/tago/analysis/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     2763 2021-09-16 01:10:53.000000 tago-3.1.0/tago/analysis/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.385057 tago-3.1.0/tago/authorization/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      642 2021-08-12 17:43:30.000000 tago-3.1.0/tago/authorization/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.385263 tago-3.1.0/tago/connector/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      778 2021-08-12 17:43:30.000000 tago-3.1.0/tago/connector/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.385450 tago-3.1.0/tago/device/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1589 2021-08-12 17:43:30.000000 tago-3.1.0/tago/device/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.385669 tago-3.1.0/tago/internal/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      433 2021-04-28 16:53:14.000000 tago-3.1.0/tago/internal/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.385831 tago-3.1.0/tago/run_user/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     3339 2021-08-12 17:43:30.000000 tago-3.1.0/tago/run_user/__init__.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.387368 tago-3.1.0/tago/services/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      637 2021-04-28 16:53:14.000000 tago-3.1.0/tago/services/__init__.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      686 2021-08-12 17:43:30.000000 tago-3.1.0/tago/services/attachment.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      736 2021-08-12 17:43:30.000000 tago-3.1.0/tago/services/console.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)     1097 2021-08-12 17:43:30.000000 tago-3.1.0/tago/services/emailService.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      918 2021-10-22 14:06:06.000000 tago-3.1.0/tago/services/mqtt.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      664 2021-08-12 17:43:30.000000 tago-3.1.0/tago/services/notification.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      749 2021-08-12 17:43:30.000000 tago-3.1.0/tago/services/sms.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.388171 tago-3.1.0/tago/utils/
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      448 2021-04-28 16:53:14.000000 tago-3.1.0/tago/utils/__init__.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      162 2021-04-28 16:53:14.000000 tago-3.1.0/tago/utils/env_to_obj.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      643 2021-08-12 17:43:30.000000 tago-3.1.0/tago/utils/getTokenByName.py
--rw-rw-rw-   0 felipefdl   (501) staff       (20)      202 2021-08-12 17:43:30.000000 tago-3.1.0/tago/utils/version.py
-drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-02-23 20:32:15.378877 tago-3.1.0/tago.egg-info/
--rw-r--r--   0 felipefdl   (501) staff       (20)     1748 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/PKG-INFO
--rw-r--r--   0 felipefdl   (501) staff       (20)     1305 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/SOURCES.txt
--rw-r--r--   0 felipefdl   (501) staff       (20)        1 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/dependency_links.txt
--rw-r--r--   0 felipefdl   (501) staff       (20)        1 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/not-zip-safe
--rw-r--r--   0 felipefdl   (501) staff       (20)       84 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/requires.txt
--rw-r--r--   0 felipefdl   (501) staff       (20)        5 2023-02-23 20:32:15.000000 tago-3.1.0/tago.egg-info/top_level.txt
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.157749 tago-3.1.1/
+-rw-r--r--   0 felipefdl   (501) staff       (20)    10753 2023-04-18 15:33:30.000000 tago-3.1.1/LICENSE.md
+-rw-r--r--   0 felipefdl   (501) staff       (20)       14 2023-04-18 15:33:30.000000 tago-3.1.1/MANIFEST.in
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1748 2023-04-18 15:39:08.157821 tago-3.1.1/PKG-INFO
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1148 2023-04-18 15:33:30.000000 tago-3.1.1/README.md
+-rw-r--r--   0 felipefdl   (501) staff       (20)       84 2023-04-18 15:33:30.000000 tago-3.1.1/requirements.txt
+-rw-r--r--   0 felipefdl   (501) staff       (20)       79 2023-04-18 15:39:08.158038 tago-3.1.1/setup.cfg
+-rw-r--r--   0 felipefdl   (501) staff       (20)      931 2023-04-18 15:35:37.000000 tago-3.1.1/setup.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.151377 tago-3.1.1/tago/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      247 2023-04-18 15:33:30.000000 tago-3.1.1/tago/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.155310 tago-3.1.1/tago/account/
+-rw-r--r--   0 felipefdl   (501) staff       (20)     6448 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/__init__.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1407 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/_share.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1726 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/accessManagement.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1665 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/actions.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     2643 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/analysis.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     4373 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/buckets.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     2723 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/connector.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     4769 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/dashboards.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     3850 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/dashboards_widgets.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     3932 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/devices.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      784 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/explore.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1995 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/files.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     2916 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/integration_network.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     2230 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/notifications.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      622 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/paymentHistory.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1255 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/paymentMethods.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1285 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/plan.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     4827 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/profiles.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     3365 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/run.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1560 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/service_authorization.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      715 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/socket.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      622 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/tags.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1193 2023-04-18 15:33:30.000000 tago-3.1.1/tago/account/template.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.155469 tago-3.1.1/tago/analysis/
+-rw-r--r--   0 felipefdl   (501) staff       (20)     2763 2023-04-18 15:33:30.000000 tago-3.1.1/tago/analysis/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.155615 tago-3.1.1/tago/authorization/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      642 2023-04-18 15:33:30.000000 tago-3.1.1/tago/authorization/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.155758 tago-3.1.1/tago/connector/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      778 2023-04-18 15:33:30.000000 tago-3.1.1/tago/connector/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.155882 tago-3.1.1/tago/device/
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1589 2023-04-18 15:33:30.000000 tago-3.1.1/tago/device/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.156093 tago-3.1.1/tago/internal/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      433 2023-04-18 15:33:30.000000 tago-3.1.1/tago/internal/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.156266 tago-3.1.1/tago/run_user/
+-rw-r--r--   0 felipefdl   (501) staff       (20)     3339 2023-04-18 15:33:30.000000 tago-3.1.1/tago/run_user/__init__.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.157150 tago-3.1.1/tago/services/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      637 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/__init__.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      686 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/attachment.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      736 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/console.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1097 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/emailService.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      918 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/mqtt.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      664 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/notification.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      749 2023-04-18 15:33:30.000000 tago-3.1.1/tago/services/sms.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.157617 tago-3.1.1/tago/utils/
+-rw-r--r--   0 felipefdl   (501) staff       (20)      448 2023-04-18 15:33:30.000000 tago-3.1.1/tago/utils/__init__.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      162 2023-04-18 15:33:30.000000 tago-3.1.1/tago/utils/env_to_obj.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      643 2023-04-18 15:33:30.000000 tago-3.1.1/tago/utils/getTokenByName.py
+-rw-r--r--   0 felipefdl   (501) staff       (20)      202 2023-04-18 15:33:30.000000 tago-3.1.1/tago/utils/version.py
+drwxr-xr-x   0 felipefdl   (501) staff       (20)        0 2023-04-18 15:39:08.152337 tago-3.1.1/tago.egg-info/
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1748 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/PKG-INFO
+-rw-r--r--   0 felipefdl   (501) staff       (20)     1305 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/SOURCES.txt
+-rw-r--r--   0 felipefdl   (501) staff       (20)        1 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/dependency_links.txt
+-rw-r--r--   0 felipefdl   (501) staff       (20)        1 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/not-zip-safe
+-rw-r--r--   0 felipefdl   (501) staff       (20)       84 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/requires.txt
+-rw-r--r--   0 felipefdl   (501) staff       (20)        5 2023-04-18 15:39:08.000000 tago-3.1.1/tago.egg-info/top_level.txt
```

### Comparing `tago-3.1.0/LICENSE.md` & `tago-3.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/PKG-INFO` & `tago-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tago
-Version: 3.1.0
+Version: 3.1.1
 Summary: Official Python lib for TagoIO
 Home-page: https://github.com/tago-io/tago-sdk-python
 Author: Tago LLC
 Author-email: dev@tago.io
 License: Apache License
 Keywords: tago tagoio develop iot sdk analysis device
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tago-3.1.0/README.md` & `tago-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/setup.py` & `tago-3.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   long_description = f.read()
 
 with open('requirements.txt', 'r') as f:
   required = f.read().splitlines()
 
 setuptools.setup(
   name='tago',
-  version='3.1.0',
+  version='3.1.1',
   python_requires='>=3.6',
   description='Official Python lib for TagoIO',
   long_description=long_description,
   long_description_content_type="text/markdown",
   classifiers=[
       'Development Status :: 5 - Production/Stable',
       'License :: OSI Approved :: Apache Software License',
```

### Comparing `tago-3.1.0/tago/account/__init__.py` & `tago-3.1.1/tago/account/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/_share.py` & `tago-3.1.1/tago/account/_share.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/accessManagement.py` & `tago-3.1.1/tago/account/accessManagement.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/actions.py` & `tago-3.1.1/tago/account/actions.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/analysis.py` & `tago-3.1.1/tago/account/analysis.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/buckets.py` & `tago-3.1.1/tago/account/buckets.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/connector.py` & `tago-3.1.1/tago/account/connector.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/dashboards.py` & `tago-3.1.1/tago/account/dashboards.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     params = {
       'page': page,
       'filter': filter,
       'fields': fields,
       'amount': amount,
       'orderBy': orderBy,
     }
-    return requests.get('{api_endpoint}/dashboard'.format(api_endpoint=API_TAGO), headers=self.default_headers, data=params).json()
+    params = fixFilter(params, filter)
+    return requests.get('{api_endpoint}/dashboard'.format(api_endpoint=API_TAGO), headers=self.default_headers, params=params).json()
 
     # Create a Dashboard
   def create(self, data):
     data = data if data else {}
     return requests.post('{api_endpoint}/dashboard'.format(api_endpoint=API_TAGO), headers=self.default_headers, json=data).json()
 
     # Edit a Dashboard
```

### Comparing `tago-3.1.0/tago/account/dashboards_widgets.py` & `tago-3.1.1/tago/account/dashboards_widgets.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/devices.py` & `tago-3.1.1/tago/account/devices.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/explore.py` & `tago-3.1.1/tago/account/explore.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/files.py` & `tago-3.1.1/tago/account/files.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/integration_network.py` & `tago-3.1.1/tago/account/integration_network.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/notifications.py` & `tago-3.1.1/tago/account/notifications.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/paymentHistory.py` & `tago-3.1.1/tago/account/paymentHistory.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/paymentMethods.py` & `tago-3.1.1/tago/account/paymentMethods.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/plan.py` & `tago-3.1.1/tago/account/plan.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/profiles.py` & `tago-3.1.1/tago/account/profiles.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/run.py` & `tago-3.1.1/tago/account/run.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/service_authorization.py` & `tago-3.1.1/tago/account/service_authorization.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/socket.py` & `tago-3.1.1/tago/account/socket.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/tags.py` & `tago-3.1.1/tago/account/tags.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/account/template.py` & `tago-3.1.1/tago/account/template.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/analysis/__init__.py` & `tago-3.1.1/tago/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/authorization/__init__.py` & `tago-3.1.1/tago/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/connector/__init__.py` & `tago-3.1.1/tago/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/device/__init__.py` & `tago-3.1.1/tago/device/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/run_user/__init__.py` & `tago-3.1.1/tago/run_user/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/__init__.py` & `tago-3.1.1/tago/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/attachment.py` & `tago-3.1.1/tago/services/attachment.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/console.py` & `tago-3.1.1/tago/services/console.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/emailService.py` & `tago-3.1.1/tago/services/emailService.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/mqtt.py` & `tago-3.1.1/tago/services/mqtt.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/notification.py` & `tago-3.1.1/tago/services/notification.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/services/sms.py` & `tago-3.1.1/tago/services/sms.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago/utils/getTokenByName.py` & `tago-3.1.1/tago/utils/getTokenByName.py`

 * *Files identical despite different names*

### Comparing `tago-3.1.0/tago.egg-info/PKG-INFO` & `tago-3.1.1/tago.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tago
-Version: 3.1.0
+Version: 3.1.1
 Summary: Official Python lib for TagoIO
 Home-page: https://github.com/tago-io/tago-sdk-python
 Author: Tago LLC
 Author-email: dev@tago.io
 License: Apache License
 Keywords: tago tagoio develop iot sdk analysis device
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tago-3.1.0/tago.egg-info/SOURCES.txt` & `tago-3.1.1/tago.egg-info/SOURCES.txt`

 * *Files identical despite different names*

