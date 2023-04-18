# Comparing `tmp/eduvpn_client-4.0.1.tar.gz` & `tmp/eduvpn_client-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eduvpn_client-4.0.1.tar", last modified: Tue Mar  7 09:42:46 2023, max compression
+gzip compressed data, was "eduvpn_client-4.1.0.tar", last modified: Tue Apr 18 14:45:24 2023, max compression
```

## Comparing `eduvpn_client-4.0.1.tar` & `eduvpn_client-4.1.0.tar`

### file list

```diff
@@ -1,997 +1,1000 @@
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.699069 eduvpn_client-4.0.1/
--rw-r--r--   0 jerry     (1000) users      (100)    35149 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/LICENSE
--rw-r--r--   0 jerry     (1000) users      (100)      936 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/LICENSE.spdx
--rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/MANIFEST.in
--rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-03-07 09:42:46.699069 eduvpn_client-4.0.1/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/README.md
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.553068 eduvpn_client-4.0.1/doc/
--rw-r--r--   0 jerry     (1000) users      (100)       17 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/.gitignore
--rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/Makefile
--rw-r--r--   0 jerry     (1000) users      (100)     6119 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/doc/conf.py
--rw-r--r--   0 jerry     (1000) users      (100)     2424 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/doc/developer.rst
--rw-r--r--   0 jerry     (1000) users      (100)     3506 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/flow.dia
--rw-r--r--   0 jerry     (1000) users      (100)    32141 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/flow.png
--rw-r--r--   0 jerry     (1000) users      (100)      760 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/index.rst
--rw-r--r--   0 jerry     (1000) users      (100)     5905 2023-03-06 15:48:34.000000 eduvpn_client-4.0.1/doc/installation.rst
--rw-r--r--   0 jerry     (1000) users      (100)       80 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/requirements.txt
--rw-r--r--   0 jerry     (1000) users      (100)   201590 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/screenshot.png
--rw-r--r--   0 jerry     (1000) users      (100)      879 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/doc/usage.rst
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.556068 eduvpn_client-4.0.1/eduvpn/
--rw-r--r--   0 jerry     (1000) users      (100)       22 2023-03-07 09:22:54.000000 eduvpn_client-4.0.1/eduvpn/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)       71 2023-03-02 16:11:20.000000 eduvpn_client-4.0.1/eduvpn/__main__.py
--rw-r--r--   0 jerry     (1000) users      (100)    20914 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/eduvpn/app.py
--rw-r--r--   0 jerry     (1000) users      (100)    24578 2023-03-07 08:49:52.000000 eduvpn_client-4.0.1/eduvpn/cli.py
--rw-r--r--   0 jerry     (1000) users      (100)     1972 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/config.py
--rw-r--r--   0 jerry     (1000) users      (100)     2088 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/connection.py
--rw-r--r--   0 jerry     (1000) users      (100)     2321 2023-02-27 11:41:59.000000 eduvpn_client-4.0.1/eduvpn/i18n.py
--rw-r--r--   0 jerry     (1000) users      (100)     4284 2023-03-07 09:13:18.000000 eduvpn_client-4.0.1/eduvpn/keyring.py
--rw-r--r--   0 jerry     (1000) users      (100)    26794 2023-03-07 09:02:11.000000 eduvpn_client-4.0.1/eduvpn/nm.py
--rw-r--r--   0 jerry     (1000) users      (100)     1139 2023-02-20 15:51:24.000000 eduvpn_client-4.0.1/eduvpn/notify.py
--rw-r--r--   0 jerry     (1000) users      (100)     2689 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/ovpn.py
--rw-r--r--   0 jerry     (1000) users      (100)     2977 2023-03-02 16:08:27.000000 eduvpn_client-4.0.1/eduvpn/server.py
--rw-r--r--   0 jerry     (1000) users      (100)     1152 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/settings.py
--rw-r--r--   0 jerry     (1000) users      (100)     1993 2023-02-20 15:51:24.000000 eduvpn_client-4.0.1/eduvpn/storage.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.557068 eduvpn_client-4.0.1/eduvpn/ui/
--rw-r--r--   0 jerry     (1000) users      (100)        0 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/eduvpn/ui/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)     1370 2023-03-07 09:30:33.000000 eduvpn_client-4.0.1/eduvpn/ui/__main__.py
--rw-r--r--   0 jerry     (1000) users      (100)     5089 2023-03-02 16:15:13.000000 eduvpn_client-4.0.1/eduvpn/ui/app.py
--rw-r--r--   0 jerry     (1000) users      (100)     6541 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/ui/search.py
--rw-r--r--   0 jerry     (1000) users      (100)     3392 2023-02-27 11:42:06.000000 eduvpn_client-4.0.1/eduvpn/ui/stats.py
--rw-r--r--   0 jerry     (1000) users      (100)    49148 2023-03-02 16:14:31.000000 eduvpn_client-4.0.1/eduvpn/ui/ui.py
--rw-r--r--   0 jerry     (1000) users      (100)     3788 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/eduvpn/ui/utils.py
--rw-r--r--   0 jerry     (1000) users      (100)     7301 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/eduvpn/utils.py
--rw-r--r--   0 jerry     (1000) users      (100)     2219 2023-03-02 13:49:57.000000 eduvpn_client-4.0.1/eduvpn/variants.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.558068 eduvpn_client-4.0.1/eduvpn_client.egg-info/
--rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/PKG-INFO
--rw-r--r--   0 jerry     (1000) users      (100)    39045 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/SOURCES.txt
--rw-r--r--   0 jerry     (1000) users      (100)        1 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/dependency_links.txt
--rw-r--r--   0 jerry     (1000) users      (100)      193 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/entry_points.txt
--rw-r--r--   0 jerry     (1000) users      (100)      122 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/requires.txt
--rw-r--r--   0 jerry     (1000) users      (100)        7 2023-03-07 09:42:46.000000 eduvpn_client-4.0.1/eduvpn_client.egg-info/top_level.txt
--rw-r--r--   0 jerry     (1000) users      (100)      362 2023-03-07 09:42:46.699069 eduvpn_client-4.0.1/setup.cfg
--rw-r--r--   0 jerry     (1000) users      (100)     3009 2023-03-07 09:23:04.000000 eduvpn_client-4.0.1/setup.py
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.558068 eduvpn_client-4.0.1/share/applications/
--rw-r--r--   0 jerry     (1000) users      (100)      186 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/applications/org.eduvpn.client.desktop
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/applications/org.letsconnect-vpn.client.desktop
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.558068 eduvpn_client-4.0.1/share/eduvpn/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.558068 eduvpn_client-4.0.1/share/eduvpn/builder/
--rw-r--r--   0 jerry     (1000) users      (100)    78613 2023-03-02 13:49:47.000000 eduvpn_client-4.0.1/share/eduvpn/builder/mainwindow.ui
--rw-r--r--   0 jerry     (1000) users      (100)    16139 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/country_codes.json
--rw-r--r--   0 jerry     (1000) users      (100)    41091 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/eduvpn.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.569068 eduvpn_client-4.0.1/share/eduvpn/images/
--rw-r--r--   0 jerry     (1000) users      (100)     2491 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle.svg
--rw-r--r--   0 jerry     (1000) users      (100)    23956 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    43016 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/back.png
--rw-r--r--   0 jerry     (1000) users      (100)     1227 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/back@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2026 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/back@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-down.png
--rw-r--r--   0 jerry     (1000) users      (100)      459 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-down@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      554 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-down@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      226 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right-white.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right-white@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      365 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right-white@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right.png
--rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/chevron-right@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/cross.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/cross@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/cross@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3360 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected.png
--rw-r--r--   0 jerry     (1000) users      (100)     7683 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    12654 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2033 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting.png
--rw-r--r--   0 jerry     (1000) users      (100)     4997 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8431 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2239 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-default.png
--rw-r--r--   0 jerry     (1000) users      (100)     5315 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-default@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8881 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-default@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3023 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected.png
--rw-r--r--   0 jerry     (1000) users      (100)     6892 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    11157 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1068 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     2292 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3677 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1023 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)     2138 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3387 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/earth-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     4355 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     9182 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    14079 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3648 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo.png
--rw-r--r--   0 jerry     (1000) users      (100)     7525 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)    11375 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.549068 eduvpn_client-4.0.1/share/eduvpn/images/flags/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.696069 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/
--rw-r--r--   0 jerry     (1000) users      (100)      367 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      297 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      384 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      230 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      705 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      871 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1257 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      702 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      910 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      660 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1321 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1366 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1066 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      587 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      750 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      816 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1569 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      276 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      684 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      812 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1314 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      423 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      629 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Artsakh@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Artsakh@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Artsakh@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      529 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      556 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      723 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      342 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      434 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      457 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      633 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      222 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      584 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      829 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1796 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      701 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      786 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1300 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      885 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1129 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1723 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      350 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      476 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      508 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-BO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-BO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-BO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1144 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      520 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      591 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1205 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1734 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      813 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1160 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      241 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      275 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      264 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      738 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-AB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-AB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-AB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1095 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1546 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2436 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      710 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      843 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1354 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1067 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1465 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2414 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      864 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      941 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1446 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      826 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1163 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1512 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      489 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      647 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      860 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1172 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      721 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1547 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      925 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1318 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      846 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-SK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-SK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      716 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-SK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      671 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      739 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1135 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      403 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      606 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      676 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1303 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1890 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      443 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      576 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1662 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      593 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      613 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      808 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      727 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1059 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      438 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      767 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      810 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      511 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      242 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Chechnya@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      225 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Chechnya@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      303 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Chechnya@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      210 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      477 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      579 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      249 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      686 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      775 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1204 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      651 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      368 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      598 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      659 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      597 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      590 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      698 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      932 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      259 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      232 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1377 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      517 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/England-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/England-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/England-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      250 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      229 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      909 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1556 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1087 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1852 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      473 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      565 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      878 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      268 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      912 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      596 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      814 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-TF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-TF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-TF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      858 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/France-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/France-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/France-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-ENG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-ENG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-ENG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      574 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      859 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1267 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-WLS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-WLS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-WLS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      831 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1194 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      506 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE-AB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      614 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE-AB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      874 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE-AB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      560 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      396 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      233 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      513 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      373 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1887 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      338 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      626 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      355 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1137 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      770 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1136 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      381 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      653 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      428 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      528 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      266 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      244 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ID@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ID@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ID@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      388 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      548 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      690 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1031 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      311 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1076 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1514 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2658 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IQ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IQ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IQ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      298 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      401 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      265 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      898 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1238 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1065 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1573 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      494 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      636 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      623 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      959 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1030 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1402 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2205 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      622 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      803 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      301 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      340 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      818 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1347 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      561 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      954 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Kurdistan@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Kurdistan@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      952 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Kurdistan@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      380 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      468 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      257 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      239 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      236 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      707 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      825 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1345 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      630 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      347 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      605 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ME@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      307 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ME@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      377 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ME@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      913 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1131 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1684 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      774 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ML@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ML@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ML@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      512 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      881 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      601 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1311 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2243 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      851 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      254 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      361 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      391 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      427 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      482 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      572 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      796 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      856 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1086 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1695 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      478 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      592 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      248 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      857 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1162 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      352 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      625 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      827 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1400 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      764 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      828 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1443 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      337 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Netherlands Antilles@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Netherlands Antilles@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/OM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/OM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/OM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      177 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Overlay@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      186 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Overlay@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Overlay@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      324 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PF@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      424 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PF@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PF@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      804 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      523 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      206 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1085 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1755 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      495 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      610 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      480 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      414 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      616 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      310 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      353 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      540 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/QA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/QA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/QA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      602 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      895 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      850 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      692 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      269 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      245 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SB@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      452 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SB@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      526 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SB@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      820 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1014 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      234 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      797 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      295 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      461 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      559 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      530 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      322 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      545 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      970 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      485 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ST@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ST@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      696 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ST@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      317 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      472 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SX@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SX@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SX@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      417 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      765 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1180 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      383 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Sealand@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      440 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Sealand@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Sealand@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Serb Republic@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Serb Republic@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Serb Republic@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/South Ossetia@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/South Ossetia@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/South Ossetia@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      832 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1507 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TD@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TD@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TD@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      425 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      631 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TH@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TH@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TH@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TJ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TJ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TJ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      632 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      991 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      563 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      673 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      905 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      577 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1019 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TO@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      263 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TO@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TO@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      557 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      956 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      334 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TT@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TT@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      426 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TT@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      811 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1338 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      762 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      962 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1399 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Transnistria@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Transnistria@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Transnistria@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      510 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      645 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      204 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      208 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/US@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/US@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      328 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/US@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UY@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      354 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UY@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UY@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UZ@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      393 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UZ@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UZ@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      253 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      255 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      406 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VC@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VC@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      687 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VC@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      524 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      837 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1372 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1052 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1672 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VN@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VN@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VN@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      674 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1460 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/WS@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      293 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/WS@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/WS@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      507 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/XK@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/XK@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      502 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/XK@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/YE@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/YE@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/YE@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      965 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZM@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZM@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZM@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@1,5x.png
--rw-r--r--   0 jerry     (1000) users      (100)      699 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1150 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/group.png
--rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/group@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/group@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1000 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1522 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      578 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)      942 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1380 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2461 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute.png
--rw-r--r--   0 jerry     (1000) users      (100)     3790 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     5404 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/institute@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      644 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2228 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     2247 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/question-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1039 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      312 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon.png
--rw-r--r--   0 jerry     (1000) users      (100)      519 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)      985 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/server-icon@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings-dark.png
--rw-r--r--   0 jerry     (1000) users      (100)     1029 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings-dark@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1426 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings-dark@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)      619 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings.png
--rw-r--r--   0 jerry     (1000) users      (100)     1077 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     1424 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/eduvpn/images/settings@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.549068 eduvpn_client-4.0.1/share/icons/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/icons/hicolor/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.549068 eduvpn_client-4.0.1/share/icons/hicolor/128x128/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.696069 eduvpn_client-4.0.1/share/icons/hicolor/128x128/apps/
--rw-r--r--   0 jerry     (1000) users      (100)     9421 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/128x128/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)     5083 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.549068 eduvpn_client-4.0.1/share/icons/hicolor/256x256/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.696069 eduvpn_client-4.0.1/share/icons/hicolor/256x256/apps/
--rw-r--r--   0 jerry     (1000) users      (100)    24039 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/256x256/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)    11183 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/icons/hicolor/48x48/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.697069 eduvpn_client-4.0.1/share/icons/hicolor/48x48/apps/
--rw-r--r--   0 jerry     (1000) users      (100)     2714 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/48x48/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)     1739 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/icons/hicolor/512x512/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.697069 eduvpn_client-4.0.1/share/icons/hicolor/512x512/apps/
--rw-r--r--   0 jerry     (1000) users      (100)    67703 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/512x512/apps/org.eduvpn.client.png
--rw-r--r--   0 jerry     (1000) users      (100)    26109 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/letsconnect/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.698069 eduvpn_client-4.0.1/share/letsconnect/images/
--rw-r--r--   0 jerry     (1000) users      (100)     1638 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/app-icon-circle.svg
--rw-r--r--   0 jerry     (1000) users      (100)     2188 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/letsconnect.png
--rw-r--r--   0 jerry     (1000) users      (100)     4471 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/letsconnect@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     7163 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/letsconnect@3x.png
--rw-r--r--   0 jerry     (1000) users      (100)     3141 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/server-illustration.png
--rw-r--r--   0 jerry     (1000) users      (100)     5498 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/server-illustration@2x.png
--rw-r--r--   0 jerry     (1000) users      (100)     8037 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/letsconnect/images/server-illustration@3x.png
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/locale/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/locale/de_DE/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.698069 eduvpn_client-4.0.1/share/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 jerry     (1000) users      (100)     3669 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/locale/de_DE/LC_MESSAGES/eduVPN.mo
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.550068 eduvpn_client-4.0.1/share/locale/es_LA/
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.698069 eduvpn_client-4.0.1/share/locale/es_LA/LC_MESSAGES/
--rw-r--r--   0 jerry     (1000) users      (100)     3696 2022-02-07 19:05:03.000000 eduvpn_client-4.0.1/share/locale/es_LA/LC_MESSAGES/eduVPN.mo
-drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-03-07 09:42:46.699069 eduvpn_client-4.0.1/tests/
--rw-r--r--   0 jerry     (1000) users      (100)        0 2022-09-27 12:47:39.000000 eduvpn_client-4.0.1/tests/__init__.py
--rw-r--r--   0 jerry     (1000) users      (100)    16825 2023-02-20 15:51:24.000000 eduvpn_client-4.0.1/tests/mock_config.py
--rw-r--r--   0 jerry     (1000) users      (100)      847 2023-02-20 15:51:24.000000 eduvpn_client-4.0.1/tests/test_nm.py
--rw-r--r--   0 jerry     (1000) users      (100)     2869 2023-02-20 15:51:24.000000 eduvpn_client-4.0.1/tests/test_stats.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/
+-rw-r--r--   0 jerry     (1000) users      (100)    35149 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/LICENSE
+-rw-r--r--   0 jerry     (1000) users      (100)      936 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/LICENSE.spdx
+-rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/MANIFEST.in
+-rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2023-03-23 15:01:02.000000 eduvpn_client-4.1.0/README.md
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.228278 eduvpn_client-4.1.0/doc/
+-rw-r--r--   0 jerry     (1000) users      (100)       17 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/.gitignore
+-rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/Makefile
+-rw-r--r--   0 jerry     (1000) users      (100)     6119 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/conf.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2424 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/developer.rst
+-rw-r--r--   0 jerry     (1000) users      (100)     3506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/flow.dia
+-rw-r--r--   0 jerry     (1000) users      (100)    32141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/flow.png
+-rw-r--r--   0 jerry     (1000) users      (100)      787 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/index.rst
+-rw-r--r--   0 jerry     (1000) users      (100)     5941 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/installation.rst
+-rw-r--r--   0 jerry     (1000) users      (100)      629 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/doc/knownissues.rst
+-rw-r--r--   0 jerry     (1000) users      (100)       80 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/requirements.txt
+-rw-r--r--   0 jerry     (1000) users      (100)   201590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/doc/screenshot.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2814 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/doc/updating.rst
+-rw-r--r--   0 jerry     (1000) users      (100)      700 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/doc/usage.rst
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.231278 eduvpn_client-4.1.0/eduvpn/
+-rw-r--r--   0 jerry     (1000) users      (100)       22 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)       71 2023-04-18 09:59:58.000000 eduvpn_client-4.1.0/eduvpn/__main__.py
+-rw-r--r--   0 jerry     (1000) users      (100)    21618 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/app.py
+-rw-r--r--   0 jerry     (1000) users      (100)    25290 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/cli.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1972 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/config.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2088 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/connection.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2321 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/i18n.py
+-rw-r--r--   0 jerry     (1000) users      (100)     4284 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/keyring.py
+-rw-r--r--   0 jerry     (1000) users      (100)    27203 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/nm.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1139 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/notify.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2689 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/ovpn.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2977 2023-04-18 10:26:25.000000 eduvpn_client-4.1.0/eduvpn/server.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1152 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/settings.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1993 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/storage.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.232278 eduvpn_client-4.1.0/eduvpn/ui/
+-rw-r--r--   0 jerry     (1000) users      (100)        0 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/eduvpn/ui/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)     1370 2023-04-18 10:06:53.000000 eduvpn_client-4.1.0/eduvpn/ui/__main__.py
+-rw-r--r--   0 jerry     (1000) users      (100)     5089 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/app.py
+-rw-r--r--   0 jerry     (1000) users      (100)     6541 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/search.py
+-rw-r--r--   0 jerry     (1000) users      (100)     3392 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/eduvpn/ui/stats.py
+-rw-r--r--   0 jerry     (1000) users      (100)    50856 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/ui/ui.py
+-rw-r--r--   0 jerry     (1000) users      (100)     3788 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/ui/utils.py
+-rw-r--r--   0 jerry     (1000) users      (100)     7301 2023-04-17 09:57:40.000000 eduvpn_client-4.1.0/eduvpn/utils.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2229 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/eduvpn/variants.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.233278 eduvpn_client-4.1.0/eduvpn_client.egg-info/
+-rw-r--r--   0 jerry     (1000) users      (100)     1819 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/PKG-INFO
+-rw-r--r--   0 jerry     (1000) users      (100)    39118 2023-04-18 14:45:24.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        1 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      193 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/entry_points.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      129 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/requires.txt
+-rw-r--r--   0 jerry     (1000) users      (100)        7 2023-04-18 14:45:23.000000 eduvpn_client-4.1.0/eduvpn_client.egg-info/top_level.txt
+-rw-r--r--   0 jerry     (1000) users      (100)      362 2023-04-18 14:45:24.401279 eduvpn_client-4.1.0/setup.cfg
+-rw-r--r--   0 jerry     (1000) users      (100)     3016 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/setup.py
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.234278 eduvpn_client-4.1.0/share/applications/
+-rw-r--r--   0 jerry     (1000) users      (100)      178 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/applications/org.eduvpn.client.desktop
+-rw-r--r--   0 jerry     (1000) users      (100)      208 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/applications/org.letsconnect-vpn.client.desktop
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.234278 eduvpn_client-4.1.0/share/eduvpn/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.235278 eduvpn_client-4.1.0/share/eduvpn/builder/
+-rw-r--r--   0 jerry     (1000) users      (100)    79500 2023-04-18 13:38:11.000000 eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui
+-rw-r--r--   0 jerry     (1000) users      (100)    79493 2023-04-17 14:01:52.000000 eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui~
+-rw-r--r--   0 jerry     (1000) users      (100)    16139 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/country_codes.json
+-rw-r--r--   0 jerry     (1000) users      (100)    41091 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/eduvpn.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.247278 eduvpn_client-4.1.0/share/eduvpn/images/
+-rw-r--r--   0 jerry     (1000) users      (100)     2491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle.svg
+-rw-r--r--   0 jerry     (1000) users      (100)    23956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    43016 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1227 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2026 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/back@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down.png
+-rw-r--r--   0 jerry     (1000) users      (100)      459 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      554 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      226 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      365 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right-white@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right.png
+-rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/cross@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7683 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    12654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2033 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4997 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8431 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5315 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected.png
+-rw-r--r--   0 jerry     (1000) users      (100)     6892 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11157 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1068 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3677 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1023 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2138 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     9182 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    14079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3648 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/eduvpn/images/flags/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.395279 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/
+-rw-r--r--   0 jerry     (1000) users      (100)      367 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      297 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      384 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      230 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      705 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      871 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      702 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      910 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      660 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1066 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      587 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      750 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      816 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1036 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      276 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      812 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      423 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      294 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      629 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      620 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      529 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      342 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      434 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      457 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      633 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      222 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      584 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      829 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      701 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      786 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      885 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1129 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1723 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      350 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      476 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      508 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1144 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      520 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      591 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1734 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      813 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1160 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      241 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      275 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      264 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      738 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      453 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-AB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1095 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1546 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      710 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      843 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1067 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1465 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      864 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      941 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      826 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      489 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      647 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      860 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1172 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      721 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1547 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      925 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      846 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      716 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      671 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1135 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      403 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      504 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      606 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      676 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1890 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      576 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      318 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      336 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      593 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      435 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      613 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      808 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      555 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      727 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1059 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      438 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      767 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      810 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      441 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      511 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      242 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      225 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      303 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Chechnya@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      210 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      477 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      579 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      742 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      249 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      686 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      775 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      651 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1110 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      368 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      598 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      659 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      906 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      597 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      927 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      590 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      698 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      932 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      259 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      232 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      517 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/England-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      250 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      229 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      909 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1556 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1087 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1852 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      473 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      565 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      878 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      268 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      912 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      596 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      814 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      527 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      858 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/France-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-ENG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      574 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      859 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1267 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      370 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-WLS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1006 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2079 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      831 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1194 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      506 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      614 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      874 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      408 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      360 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      343 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      560 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      396 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      305 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      233 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      513 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      373 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      491 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1887 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      626 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      355 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      534 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1137 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      770 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1136 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      381 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      653 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      420 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      528 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      266 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      244 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ID@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      219 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      388 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      548 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      690 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1031 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      445 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1076 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1514 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IQ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      298 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      401 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      265 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      359 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      289 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      898 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1238 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      754 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1065 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1573 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      494 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      636 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      392 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      623 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      959 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      568 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1030 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1402 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2205 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      883 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      908 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      894 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1118 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      622 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      803 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      301 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      340 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      818 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      561 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      662 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      954 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      952 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      468 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      300 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      257 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      466 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      719 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      239 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      236 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      314 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      707 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      825 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1345 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      436 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      433 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      630 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      347 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      605 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      387 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      201 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      375 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      327 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      418 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      307 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      377 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ME@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      218 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      217 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      292 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      913 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1131 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1684 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      774 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ML@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      512 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      641 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      881 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      601 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      940 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1311 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2243 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      851 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      254 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      329 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      224 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      521 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      361 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      391 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      427 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      482 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      572 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      796 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      856 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1086 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      478 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      592 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      335 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      462 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      357 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      291 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      378 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      260 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      248 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      331 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      286 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      273 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      857 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1162 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      352 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      371 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      625 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      827 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1400 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      764 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      828 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1443 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      337 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      389 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      553 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      177 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      186 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Overlay@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      324 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      525 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      394 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      732 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1128 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      566 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      804 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      523 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      694 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1010 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      202 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      206 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      278 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      830 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1085 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1755 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      610 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      794 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      409 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      480 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      414 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      616 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      379 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      310 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      353 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      540 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      407 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      448 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      290 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      602 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      895 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      207 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      283 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      419 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      467 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      850 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      475 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      564 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      692 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      269 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      245 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      320 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      452 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      526 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      820 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1014 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      410 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      611 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      234 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      306 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      416 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      487 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      797 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      295 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      285 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      446 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      575 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      216 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      658 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      964 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      330 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      405 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      559 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      454 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      530 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      744 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      322 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      413 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      545 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      675 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      970 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      485 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      493 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      317 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      358 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      531 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      472 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      569 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      747 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      282 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      299 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      417 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      668 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      765 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1180 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      383 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      440 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      551 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      211 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      214 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Serb Republic@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      209 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      212 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      274 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/South Ossetia@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      730 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      832 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      220 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      288 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TD@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      425 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      444 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      631 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      223 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      287 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TH@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      302 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      363 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      632 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      713 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      991 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      563 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      673 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      958 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      456 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      581 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      905 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      577 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      740 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1019 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      308 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      263 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      321 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TO@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      557 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      652 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      956 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      334 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TT@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      695 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      811 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1338 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      366 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      562 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      762 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      962 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1399 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      258 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      221 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      296 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Transnistria@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      510 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      645 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      945 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      204 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      208 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      277 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      364 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      603 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      284 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      252 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      328 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/US@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      341 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      354 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      488 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UY@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      316 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      393 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UZ@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      253 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      255 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      344 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      406 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      496 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      687 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      524 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      654 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      994 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      691 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      837 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1372 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      897 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1052 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1672 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      486 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      585 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      821 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      674 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      917 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1460 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      333 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      293 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      346 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/WS@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      507 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      411 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      502 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/XK@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      213 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      215 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      280 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/YE@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      706 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      965 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      326 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      386 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      497 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZM@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      544 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@1,5x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      699 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1150 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      385 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group.png
+-rw-r--r--   0 jerry     (1000) users      (100)      642 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      815 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/group@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      583 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1000 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1522 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      578 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)      942 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1380 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2461 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3790 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5404 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/institute@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      644 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1495 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2228 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1428 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     2247 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/question-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      309 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)      538 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      312 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon.png
+-rw-r--r--   0 jerry     (1000) users      (100)      519 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      985 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/server-icon@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      621 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1029 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1426 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)      619 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1077 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1424 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/eduvpn/images/settings@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/icons/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.222278 eduvpn_client-4.1.0/share/icons/hicolor/128x128/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)     9421 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5083 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/256x256/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)    24039 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)    11183 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/48x48/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.396279 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)     2714 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)     1739 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/icons/hicolor/512x512/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.397279 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/
+-rw-r--r--   0 jerry     (1000) users      (100)    67703 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.eduvpn.client.png
+-rw-r--r--   0 jerry     (1000) users      (100)    26109 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.223278 eduvpn_client-4.1.0/share/letsconnect/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/letsconnect/images/
+-rw-r--r--   0 jerry     (1000) users      (100)     1638 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/app-icon-circle.svg
+-rw-r--r--   0 jerry     (1000) users      (100)     2188 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect.png
+-rw-r--r--   0 jerry     (1000) users      (100)     4471 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     7163 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@3x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     3141 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration.png
+-rw-r--r--   0 jerry     (1000) users      (100)     5498 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@2x.png
+-rw-r--r--   0 jerry     (1000) users      (100)     8037 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@3x.png
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/de_DE/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 jerry     (1000) users      (100)     3669 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/eduVPN.mo
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.224278 eduvpn_client-4.1.0/share/locale/es_LA/
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.398279 eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/
+-rw-r--r--   0 jerry     (1000) users      (100)     3696 2022-02-07 19:05:03.000000 eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/eduVPN.mo
+drwxr-xr-x   0 jerry     (1000) users      (100)        0 2023-04-18 14:45:24.400279 eduvpn_client-4.1.0/tests/
+-rw-r--r--   0 jerry     (1000) users      (100)        0 2022-09-27 12:47:39.000000 eduvpn_client-4.1.0/tests/__init__.py
+-rw-r--r--   0 jerry     (1000) users      (100)    16825 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/mock_config.py
+-rw-r--r--   0 jerry     (1000) users      (100)      847 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/test_nm.py
+-rw-r--r--   0 jerry     (1000) users      (100)     2869 2023-04-17 08:56:44.000000 eduvpn_client-4.1.0/tests/test_stats.py
```

### Comparing `eduvpn_client-4.0.1/LICENSE` & `eduvpn_client-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/LICENSE.spdx` & `eduvpn_client-4.1.0/LICENSE.spdx`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/PKG-INFO` & `eduvpn_client-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eduvpn_client
-Version: 4.0.1
+Version: 4.1.0
 Summary: eduVPN client
 Home-page: https://github.com/eduvpn/python-eduvpn-client
 Author: Jeroen Wijenbergh
 Author-email: jeroen.wijenbergh@geant.org
 License: GPL3
 Keywords: vpn openvpn networking security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eduvpn_client-4.0.1/README.md` & `eduvpn_client-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/Makefile` & `eduvpn_client-4.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/conf.py` & `eduvpn_client-4.1.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/developer.rst` & `eduvpn_client-4.1.0/doc/developer.rst`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/flow.dia` & `eduvpn_client-4.1.0/doc/flow.dia`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/flow.png` & `eduvpn_client-4.1.0/doc/flow.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/doc/index.rst` & `eduvpn_client-4.1.0/doc/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    installation
+   updating
    usage
    developer
+   knownissues
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `eduvpn_client-4.0.1/doc/installation.rst` & `eduvpn_client-4.1.0/doc/installation.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 Debian (11) and Ubuntu (22.04 & 22.10)
 =================
 
 .. code-block:: console
 
-    $ sudo apt install apt-transport-https lsb-release
+    $ sudo apt install apt-transport-https lsb-release wget
     $ wget -O- https://app.eduvpn.org/linux/v4/deb/app+linux@eduvpn.org.asc | gpg --dearmor | sudo tee /usr/share/keyrings/eduvpn-v4.gpg >/dev/null
-    $ echo "deb [signed-by=/usr/share/keyrings/eduvpn-v4.gpg] https://app.eduvpn.org/linux/v4/deb/ $(lsb_release -cs) main" | sudo tee -a /etc/apt/sources.list.d/eduvpn-v4.list
+    $ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/eduvpn-v4.gpg] https://app.eduvpn.org/linux/v4/deb/ $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/eduvpn-v4.list
     $ sudo apt update
     $ sudo apt install eduvpn-client
 
 Fedora (36 & 37)
 =================
 
 .. code-block:: console
```

### Comparing `eduvpn_client-4.0.1/doc/screenshot.png` & `eduvpn_client-4.1.0/doc/screenshot.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/app.py` & `eduvpn_client-4.1.0/eduvpn/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,16 @@
 import webbrowser
 from datetime import datetime
 from typing import Any, Callable, Iterator, List, Optional, TextIO
 
 from eduvpn_common.discovery import DiscoOrganization, DiscoServer
 from eduvpn_common.error import WrappedError
 from eduvpn_common.main import EduVPN
-from eduvpn_common.server import (
-    Config,
-    InstituteServer,
-    SecureInternetServer,
-    Server,
-    Token,
-)
+from eduvpn_common.server import (Config, InstituteServer,
+                                  SecureInternetServer, Server, Token)
 from eduvpn_common.state import State, StateType
 from eduvpn_common.types import ReadRxBytes
 
 from eduvpn import nm
 from eduvpn.config import Configuration
 from eduvpn.connection import Connection, Validity
 from eduvpn.keyring import DBusKeyring, InsecureFileKeyring, TokenKeyring
@@ -140,14 +135,15 @@
         self.keyring: TokenKeyring = DBusKeyring(variant)
         if not self.keyring.available:
             self.keyring = InsecureFileKeyring(variant)
         self.transitions = ApplicationModelTransitions(common, variant)
         self.variant = variant
         self.nm_manager = nm_manager
         self.common.register_class_callbacks(self)
+        self.was_tcp = False
 
     @property
     def server_db(self):
         return self.transitions.server_db
 
     @property
     def current_server(self):
@@ -161,60 +157,69 @@
         rx_bytes = self.nm_manager.get_stats_bytes(filehandler)
         if rx_bytes is None:
             return -1
         return rx_bytes
 
     def should_failover(self):
         current_vpn_protocol = self.nm_manager.protocol
-        if current_vpn_protocol != "WireGuard":
+        if current_vpn_protocol == "WireGuard":
+            logger.debug("Current protocol is WireGuard, failover should continue")
+            return True
+
+        if not self.was_tcp:
             logger.debug(
-                f"Current protocol ({current_vpn_protocol}) does not support failover"
+                "Protocol is not WireGuard and TCP was not previously triggered, failover should continue"
             )
-            return False
-        return True
+            return True
+
+        logger.debug("Failover should not continue")
+        return False
+
+    def reconnect_tcp(self, callback: Callable):
+        def on_reconnected():
+            self.common.set_support_wireguard(has_wireguard)
+            callback(True)
+
+        has_wireguard = nm.is_wireguard_supported()
+
+        # Disable wireguard
+        self.common.set_support_wireguard(False)
+        self.reconnect(on_reconnected, prefer_tcp=True)
 
     def start_failover(self, callback: Callable):
         try:
             rx_bytes_file = self.nm_manager.open_stats_file("rx_bytes")
             if rx_bytes_file is None:
                 logger.debug(
                     "Failed to initialize failover, failed to open rx bytes file"
                 )
                 callback(False)
                 return
-            endpoint = self.nm_manager.wg_endpoint_ip
+            endpoint = self.nm_manager.failover_endpoint_ip
             if endpoint is None:
-                logger.debug(
-                    "Failed to initialize failover, failed to get WireGuard endpoint"
-                )
+                logger.debug("Failed to initialize failover, failed to get endpoint")
                 callback(False)
                 return
-            wg_mtu = self.nm_manager.wireguard_mtu
-            if wg_mtu is None:
-                logger.debug("failed to get WireGuard MTU, setting MTU to 1000")
-                wg_mtu = 1000
+            mtu = self.nm_manager.mtu
+            if mtu is None:
+                logger.debug("failed to get MTU for failover, setting MTU to 1000")
+                mtu = 1000
+            logger.debug(
+                f"starting failover with gateway {endpoint} and MTU {mtu} for protocol {self.nm_manager.protocol}"
+            )
             dropped = self.common.start_failover(
                 endpoint,
-                wg_mtu,
+                mtu,
                 ReadRxBytes(lambda: self.get_failover_rx(rx_bytes_file)),
             )
-            has_wireguard = nm.is_wireguard_supported()
-
-            def on_reconnected():
-                self.common.set_support_wireguard(has_wireguard)
-                callback(True)
 
             if dropped:
                 logger.debug("Failover exited, connection is dropped")
                 if self.is_connected():
-                    has_wireguard = nm.is_wireguard_supported()
-
-                    # Disable wireguard
-                    self.common.set_support_wireguard(False)
-                    self.reconnect(on_reconnected, prefer_tcp=True)
+                    self.reconnect_tcp(callback)
                     return
                 # Dropped but not relevant anymore
                 callback(False)
                 return
             else:
                 logger.debug("Failover exited, connection is NOT dropped")
                 callback(False)
@@ -249,15 +254,15 @@
         self.common.go_back()
 
     def should_renew_button(self) -> int:
         return self.common.should_renew_button()
 
     def add(self, server, callback=None):
         if isinstance(server, InstituteServer):
-            self.common.add_institute_acces(server.url)
+            self.common.add_institute_access(server.url)
         elif isinstance(server, DiscoServer):
             self.common.add_institute_access(server.base_url)
         elif isinstance(server, SecureInternetServer) or isinstance(
             server, DiscoOrganization
         ):
             self.common.add_secure_internet_home(server.org_id)
         elif isinstance(server, Server):
@@ -278,15 +283,14 @@
 
         # Delete tokens from the keyring
         self.clear_tokens(server)
 
     def connect_get_config(
         self, server, tokens=None, prefer_tcp: bool = False
     ) -> Optional[Config]:
-        # We prefer TCP if the user has set it or UDP is determined to be blocked
         if isinstance(server, InstituteServer):
             return self.common.get_config_institute_access(
                 server.url, prefer_tcp, tokens
             )
         elif isinstance(server, DiscoServer):
             return self.common.get_config_institute_access(
                 server.base_url, prefer_tcp, tokens
@@ -329,57 +333,68 @@
             return Token(tokens["access"], tokens["refresh"], int(tokens["expires"]))
         except Exception as e:
             logger.debug("Failed loading tokens with exception:")
             logger.debug(e, exc_info=True)
             return None
 
     def save_tokens(self, server, tokens):
+        logger.debug("Save tokens called")
+        if tokens.access == "" and tokens.refresh == "":
+            logger.warning("Got empty tokens, not saving them to the keyring")
+            return
         tokens_dict = {}
         tokens_dict["access"] = tokens.access
         tokens_dict["refresh"] = tokens.refresh
         tokens_dict["expires"] = str(tokens.expires)
         attributes = {
             "server": server.url,
             "category": server.category,
         }
         label = f"{server.url} - OAuth Tokens"
         try:
             self.keyring.save(label, attributes, json.dumps(tokens_dict))
         except Exception as e:
-            logger.debug("Failed saving tokens with exception:")
-            logger.debug(e, exc_info=True)
+            logger.error("Failed saving tokens with exception:")
+            logger.error(e, exc_info=True)
 
     def connect(
         self,
         server,
         callback: Optional[Callable] = None,
         ensure_exists=False,
         prefer_tcp: bool = False,
     ) -> None:
+        # Variable to be used as a last resort or for debugging
+        # to override the prefer TCP setting
+        if os.environ.get("EDUVPN_PREFER_TCP", "0") == "1":
+            prefer_tcp = True
+
         config = None
         config_type = None
         if ensure_exists:
             self.add(server)
 
         tokens = None
         if not isinstance(server, DiscoServer) and not isinstance(
             server, DiscoOrganization
         ):
             tokens = self.load_tokens(server)
+        # keep track if we preferred TCP
+        # this is for failover
+        self.was_tcp = prefer_tcp
+
         config = self.connect_get_config(server, tokens, prefer_tcp=prefer_tcp)
         if not config:
             raise Exception("No configuration available")
 
         # Get the updated info from the go library
         # Because profiles can be switched
         # And we need the most updated profile settings for default gateway
         server = self.current_server
 
-        self.save_tokens(server, config.tokens)
-
         default_gateway = True
         if server.profiles is not None and server.profiles.current is not None:
             default_gateway = server.profiles.current.default_gateway
 
         def on_connected():
             self.common.set_connected()
             if callback:
```

### Comparing `eduvpn_client-4.0.1/eduvpn/cli.py` & `eduvpn_client-4.1.0/eduvpn/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 # readline is used! It is for going up and down in interactive mode
 import argparse
 import readline  # noqa: W0611
-import signal
 import sys
+from functools import partial
 from typing import Callable
 
 import eduvpn_common.main as common
 from eduvpn_common.server import InstituteServer, SecureInternetServer, Server
 from eduvpn_common.state import State, StateType
 
 import eduvpn.nm as nm
 from eduvpn import __version__
 from eduvpn.app import Application
 from eduvpn.i18n import country, retrieve_country_name
 from eduvpn.server import ServerDatabase
-from eduvpn.settings import (
-    CLIENT_ID,
-    CONFIG_DIR_MODE,
-    CONFIG_PREFIX,
-    LETSCONNECT_CLIENT_ID,
-    LETSCONNECT_CONFIG_PREFIX,
-)
+from eduvpn.settings import (CLIENT_ID, CONFIG_DIR_MODE, CONFIG_PREFIX,
+                             LETSCONNECT_CLIENT_ID, LETSCONNECT_CONFIG_PREFIX)
 from eduvpn.ui.search import ServerGroup, group_servers
 from eduvpn.ui.utils import get_validity_text, should_show_error
 from eduvpn.utils import cmd_transition, init_logger, run_in_background_thread
 from eduvpn.variants import EDUVPN, LETS_CONNECT, ApplicationVariant
 
 
 def get_grouped_index(servers, index):
@@ -42,45 +37,54 @@
     # There is only a single profile
     if len(profiles.profiles) == 1:
         print("There is only a single profile for this server:", profiles.profiles[0])
         app.model.set_profile(profiles.profiles[0])
         return False
 
     # Multiple profiles, print the index
-    for index, profile in enumerate(profiles.profiles):
+    sorted_profiles = sorted(profiles.profiles, key=lambda p: str(p))
+    for index, profile in enumerate(sorted_profiles):
         print(f"[{index+1}]: {str(profile)}")
 
     # And ask for the 1 based index
     while True:
         profile_nr = input("Please select a profile number to continue connecting: ")
         try:
             profile_index = int(profile_nr)
 
-            if profile_index < 1 or profile_index > len(profiles.profiles):
+            if profile_index < 1 or profile_index > len(sorted_profiles):
                 print(f"Invalid profile choice: {profile_index}")
                 continue
-            app.model.set_profile(profiles.profiles[profile_index - 1])
+            app.model.set_profile(sorted_profiles[profile_index - 1])
             return True
         except ValueError:
             print(f"Input is not a number: {profile_nr}")
 
 
 def ask_locations(app, locations):
-    for index, location in enumerate(locations):
-        print(f"[{index+1}]: {retrieve_country_name(location)}")
+    # Create tuples of country name, location id
+    location_tuples = []
+    for loc in locations:
+        country_name = retrieve_country_name(loc)
+        location_tuples.append((country_name, loc))
+
+    # Sort them and then print
+    location_tuples.sort(key=lambda k: k[0])
+    for index, location in enumerate(location_tuples):
+        print(f"[{index+1}]: {location[0]}")
 
     while True:
         location_nr = input("Please select a location to continue: ")
         try:
             location_index = int(location_nr)
 
-            if location_index < 1 or location_index > len(locations):
+            if location_index < 1 or location_index > len(location_tuples):
                 print(f"Invalid location choice: {location_index}")
                 continue
-            app.model.set_secure_location(locations[location_index - 1])
+            app.model.set_secure_location(location_tuples[location_index - 1][1])
             return
         except ValueError:
             print(f"Input is not a number: {location_nr}")
 
 
 class CommandLine:
     def __init__(self, name: str, variant: ApplicationVariant, common):
@@ -159,34 +163,37 @@
         if not self.app.model.should_failover():
             callback()
             return
 
         def on_reconnected(dropped):
             if dropped:
                 print(
-                    "We have switched to a new VPN protocol as the previous protocol was blocked"
+                    "We have switched to a new protocol as the previous protocol was blocked"
                 )
             else:
-                print("Done testing, you are connected")
+                print(
+                    "Done testing, you are connected. If you experience any connectivity issues, you can disconnect and try again with the --tcp flag"
+                )
             callback()
 
         print("Connected, but we are testing your VPN if it can reach the internet...")
         self.app.model.start_failover(on_reconnected)
 
-    def connect_server(self, server):
+    def connect_server(self, server, prefer_tcp: bool):
         def connect(callback=None):
             @run_in_background_thread("connect")
             def connect_background():
                 try:
                     # Connect to the server and ensure it exists
                     should_add = not self.server_db.has(server)
                     self.app.model.connect(
                         server,
                         lambda: self.start_failover(callback),
                         ensure_exists=should_add,
+                        prefer_tcp=prefer_tcp,
                     )
                 except Exception as e:
                     if should_show_error(e):
                         print("Error connecting:", e, file=sys.stderr)
                     if callback:
                         callback()
 
@@ -235,15 +242,15 @@
 
         if search_query:
             server = self.get_server_search(search_query)
         elif url:
             server = InstituteServer(url, "Institute Server", [], None, 0)
         elif org_id:
             server = SecureInternetServer(
-                org_id, "Organisation Server", [], None, 0, "NL"
+                org_id, "Organisation Server", [], [], None, 0, "NL"
             )
         elif custom_url:
             server = Server(custom_url, "Custom Server")
         elif number is not None:
             server = get_grouped_index(self.server_db.configured, number - 1)
             if not server:
                 print(f"Configured server with number: {number} does not exist")
@@ -284,15 +291,17 @@
             return False
 
         if not variables:
             server = self.ask_server()
         else:
             server = self.parse_server(variables)
 
-        return self.connect_server(server)
+        prefer_tcp = variables.get("tcp", False)
+
+        return self.connect_server(server, prefer_tcp)
 
     def disconnect(self, _arg={}):
         if not self.app.model.is_connected():
             print("You are not connected to a server", file=sys.stderr)
             return False
 
         def disconnect(callback=None):
@@ -457,64 +466,54 @@
                 print("Please enter a number")
                 return
             server = get_grouped_index(self.server_db.configured, number - 1)
             if not server:
                 print(f"Configured server with number: {number} does not exist")
         return self.remove_server(server)
 
-    def help_interactive(self):
-        print(
-            "Available commands: change-location, change-profile, connect, disconnect, renew, remove, status, list, help, quit"
-        )
+    def help_interactive(self, commands):
+        command_keys = sorted(list(commands.keys()) + ["help"])
+        print(f"Available commands: {', '.join(command_keys)}")
 
     def update_state(self, initial: bool = False):
         def update_state_callback(callback):
             state = self.nm_manager.connection_state
             self.app.on_network_update_callback(state, initial)
 
             # This exits the main loop and gives back control to the CLI
             callback()
 
         nm.action_with_mainloop(update_state_callback)
 
-    def handle_exit(self):
-        def signal_handler(_signal, _frame):
-            if self.app.model.is_oauth_started():
-                self.common.cancel_oauth()
-            self.common.deregister()
-            sys.exit(1)
-
-        signal.signal(signal.SIGINT, signal_handler)
-
     def interactive(self, _):
         # Show a title and the help
         print(f"Welcome to the {self.name} interactive commandline")
-        self.help_interactive()
+        # Execute the right command
+        commands = {
+            "change-profile": self.change_profile,
+            "connect": self.connect,
+            "disconnect": self.disconnect,
+            "renew": self.renew,
+            "remove": self.remove,
+            "status": self.status,
+            "list": self.list,
+            "quit": lambda: print("Exiting..."),
+        }
+        if self.variant.use_predefined_servers:
+            commands["change-location"] = self.change_location
+        self.help_interactive(commands)
         command = ""
         while command != "quit":
             # Ask for the command to execute
             command = input(f"[{self.name}]: ")
 
             # Update the state right before we execute
             self.update_state()
 
-            # Execute the right command
-            commands = {
-                "change-location": self.change_location,
-                "change-profile": self.change_profile,
-                "connect": self.connect,
-                "disconnect": self.disconnect,
-                "renew": self.renew,
-                "remove": self.remove,
-                "status": self.status,
-                "list": self.list,
-                "help": self.help_interactive,
-                "quit": lambda: print("Exiting..."),
-            }
-            func = commands.get(command, self.help_interactive)
+            func = commands.get(command, partial(self.help_interactive, commands))
             func()
 
     def start(self):
         parser = argparse.ArgumentParser(
             description=f"The {self.name} command line client"
         )
         parser.set_defaults(func=lambda _: parser.print_usage())
@@ -532,65 +531,72 @@
         interactive_parser.set_defaults(func=self.interactive)
 
         renew_parser = subparsers.add_parser(
             "renew", help="renew the validity for the currently connected server"
         )
         renew_parser.set_defaults(func=self.renew)
 
-        change_profile_parser = subparsers.add_parser(
-            "change-location",
-            help="change the location for the currently connected secure internet server",
-        )
-        change_profile_parser.set_defaults(func=self.change_location)
+        if self.variant.use_predefined_servers:
+            change_profile_parser = subparsers.add_parser(
+                "change-location",
+                help="change the location for the currently connected secure internet server",
+            )
+            change_profile_parser.set_defaults(func=self.change_location)
 
         change_profile_parser = subparsers.add_parser(
             "change-profile",
             help="change the profile for the currently connected server",
         )
         change_profile_parser.set_defaults(func=self.change_profile)
 
         connect_parser = subparsers.add_parser("connect", help="connect to a server")
+        connect_parser.add_argument(
+            "-t",
+            "--tcp",
+            action="store_true",
+            help="prefer to connect using TCP if available. Useful if your network blocks UDP connections and the client/NetworkManager does not properly detect issues",
+        )
         connect_group = connect_parser.add_mutually_exclusive_group(required=True)
         if self.variant.use_predefined_servers:
             connect_group.add_argument(
                 "-s",
                 "--search",
                 type=str,
-                help="connect to a server by searching for one",
+                help="connect to a new server by searching for one",
             )
             connect_group.add_argument(
                 "-o",
                 "--orgid",
                 type=str,
-                help="connect to a secure internet server using the organisation ID",
+                help="connect to a new secure internet server using the organisation ID",
             )
             connect_group.add_argument(
                 "-u",
                 "--url",
                 type=str,
-                help="connect to an institute access server using the URL",
+                help="connect to a new institute access server using the URL",
             )
         connect_group.add_argument(
             "-c",
             "--custom-url",
             type=str,
-            help="connect to a custom server using the URL",
+            help="connect to a new custom server using the URL",
         )
         connect_group.add_argument(
             "-n",
             "--number",
             type=int,
             help="connect to an already configured server using the number. Run the 'list' subcommand to see the currently configured servers with their number",
         )
         if self.variant.use_predefined_servers:
             connect_group.add_argument(
                 "-a",
                 "--number-all",
                 type=int,
-                help="connect to a server using the number for all servers. Run the 'list --all' command to see all the available servers with their number",
+                help="connect to a new server using the number for all servers. Run the 'list --all' command to see all the available servers with their number",
             )
         connect_group.set_defaults(func=lambda args: self.connect(vars(args)))
 
         disconnect_parser = subparsers.add_parser(
             "disconnect", help="disconnect the currently active server"
         )
         disconnect_parser.set_defaults(func=self.disconnect)
@@ -617,24 +623,22 @@
         status_parser = subparsers.add_parser(
             "status", help="see the current status of eduVPN"
         )
         status_parser.set_defaults(func=self.status)
 
         parsed = parser.parse_args()
 
-        # Handle ctrl+c
-        self.handle_exit()
-
         init_logger(parsed.debug, self.variant.logfile, CONFIG_DIR_MODE)
 
         # Skip yes/no prompts if given
         self.skip_yes = parsed.yes
 
         # Register the common library
         self.common.register(parsed.debug)
+        self.common.set_token_updater(self.app.model.save_tokens)
 
         # Update the state by asking NetworkManager
         self.update_state(True)
 
         # Run the command
         parsed.func(parsed)
```

### Comparing `eduvpn_client-4.0.1/eduvpn/config.py` & `eduvpn_client-4.1.0/eduvpn/config.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/connection.py` & `eduvpn_client-4.1.0/eduvpn/connection.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/i18n.py` & `eduvpn_client-4.1.0/eduvpn/i18n.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/keyring.py` & `eduvpn_client-4.1.0/eduvpn/keyring.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/nm.py` & `eduvpn_client-4.1.0/eduvpn/nm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import enum
+import ipaddress
 import logging
 import time
 import uuid
 from configparser import ConfigParser
 from functools import lru_cache
 from ipaddress import ip_address, ip_interface
 from pathlib import Path
 from shutil import rmtree
-from socket import AF_INET, AF_INET6, gaierror, gethostbyname
+from socket import AF_INET, AF_INET6
 from tempfile import mkdtemp
 from typing import Any, Callable, Optional, TextIO, Tuple
 
 import gi
 
 from eduvpn.ovpn import Ovpn
 from eduvpn.storage import get_uuid, set_uuid, write_ovpn
@@ -85,17 +86,17 @@
             raise ValueError(state)
 
 
 # A manager for a manager :-)
 class NMManager:
     def __init__(self, variant: ApplicationVariant):
         self.variant = variant
-        self.wg_endpoint_ip: Optional[str] = None
         try:
             self.client = NM.Client.new(None)
+            self.wg_gateway_ip: Optional[ipaddress.IPv4Address] = None
         except Exception:
             self.client = None
 
     @property
     def available(self) -> bool:
         if NM is None:
             return False
@@ -150,19 +151,26 @@
         master_devices = active_connection.get_devices()
         if master_devices is None:
             return False
 
         return any(d.get_managed() for d in master_devices)
 
     @property
-    def wireguard_mtu(self) -> Optional[int]:
-        device = self.wireguard_device
-        if device is None:
-            return None
-        return device.get_mtu()
+    def mtu(self) -> Optional[int]:
+        protocol = self.protocol
+        # For WireGuard, we can get the MTU from the device
+        if protocol == "WireGuard":
+            device = self.wireguard_device
+            if device is None:
+                return None
+            return device.get_mtu()
+        elif protocol == "OpenVPN":
+            # TODO: How to query networkmanager for this?
+            return 1500
+        return None
 
     @property
     def uuid(self):
         return get_uuid(self.variant)
 
     @uuid.setter
     def uuid(self, new_uuid):
@@ -226,23 +234,30 @@
             return None
 
         # Not always a master device is configured
         # So get the interface for the first device we have
         return devices[0].get_iface()
 
     @property
-    def ipv4(self) -> Optional[str]:
+    def ipv4_config(self) -> Optional[NM.IPConfig]:
         """
-        Get the ipv4 address for an openvpn or wireguard connection as a string if there is one
+        Get the ipv4 config for the active VPN connection
         """
         active_con = self.active_connection
         if not active_con:
             return None
 
-        ip4_config = active_con.get_ip4_config()
+        return active_con.get_ip4_config()
+
+    @property
+    def ipv4(self) -> Optional[str]:
+        """
+        Get the ipv4 address for an openvpn or wireguard connection as a string if there is one
+        """
+        ip4_config = self.ipv4_config
         if not ip4_config:
             return None
 
         addresses = ip4_config.get_addresses()
         if not addresses:
             return None
 
@@ -274,14 +289,31 @@
                 if not ipv6.is_link_local:
                     return ipv6_str
             except ValueError:
                 continue
         return None
 
     @property
+    def failover_endpoint_ip(self) -> Optional[str]:
+        protocol = self.protocol
+        if protocol == "OpenVPN":
+            # if OpenVPN return the gateway from the ip config
+            ipv4_config = self.ipv4_config
+            if not ipv4_config:
+                return None
+            return ipv4_config.get_gateway()
+        elif protocol == "WireGuard":
+            # if WireGuard return the cached IP
+            if not self.wg_gateway_ip:
+                return None
+            return str(self.wg_gateway_ip)
+        else:
+            return None
+
+    @property
     def existing_connection(self) -> Optional[str]:
         if not self.uuid:
             return None
         connection = self.client.get_connection_by_uuid(self.uuid)
         if connection is None:
             return None
         else:
@@ -419,35 +451,31 @@
     def start_openvpn_connection(
         self, ovpn: Ovpn, default_gateway, *, callback=None
     ) -> None:
         _logger.debug("writing ovpn configuration to Network Manager")
         new_con = self.import_ovpn(ovpn)
         self.set_connection(new_con, callback, default_gateway)  # type: ignore
 
-    def get_ip(self, url) -> Optional[str]:
-        try:
-            ip = gethostbyname(url)
-        except gaierror:
-            ip = None
-        return ip
-
     def start_wireguard_connection(  # noqa: C901
         self,
         config: ConfigParser,
         default_gateway,
         *,
         callback=None,
     ) -> None:
         _logger.debug("writing wireguard configuration to Network Manager")
 
         ipv4s = []
         ipv6s = []
+        self.wg_gateway_ip = None
         for ip in config["Interface"]["Address"].split(","):
             addr = ip_interface(ip.strip())
             if addr.version == 4:
+                if not self.wg_gateway_ip:
+                    self.wg_gateway_ip = addr.network[1]
                 ipv4s.append(
                     NM.IPAddress(AF_INET, str(addr.ip), addr.network.prefixlen)
                 )
             elif addr.version == 6:
                 ipv6s.append(
                     NM.IPAddress(AF_INET6, str(addr.ip), addr.network.prefixlen)
                 )
@@ -483,16 +511,14 @@
             NM.SETTING_CONNECTION_INTERFACE_NAME, self.variant.translation_domain
         )
 
         # https://lazka.github.io/pgi-docs/NM-1.0/classes/WireGuardPeer.html#NM.WireGuardPeer
         peer = NM.WireGuardPeer.new()
         wg_endpoint = config["Peer"]["Endpoint"]
         peer.set_endpoint(wg_endpoint, allow_invalid=False)
-        endpoint = wg_endpoint.split(":")[0]
-        self.wg_endpoint_ip = self.get_ip(endpoint)
 
         peer.set_public_key(config["Peer"]["PublicKey"], accept_invalid=False)
         for ip in config["Peer"]["AllowedIPs"].split(","):
             peer.append_allowed_ip(ip.strip(), accept_invalid=False)
 
         s_ip4 = NM.SettingIP4Config.new()
         s_ip6 = NM.SettingIP6Config.new()
@@ -571,36 +597,20 @@
     def deactivate_connection(self, callback: Optional[Callable] = None) -> None:
         connection = self.active_connection
         if connection is None:
             _logger.warning(f"no connection to deactivate of uuid {uuid}")
             return
         type = connection.get_connection_type()
         if type == "vpn":
-            self.deactivate_connection_vpn()
+            self.deactivate_connection_vpn(callback)
         elif type == "wireguard":
-            self.deactivate_connection_wg()
+            self.deactivate_connection_wg(callback)
         else:
             _logger.warning(f"unexpected connection type {type}")
 
-        if not callback:
-            return
-        signal = None
-
-        def changed_state(
-            active: "NM.ActiveConnection", state_code: int, _reason_code: int
-        ):
-            state = NM.ActiveConnectionState(state_code)
-            if ConnectionState.from_active_state(state) == ConnectionState.DISCONNECTED:
-                if signal:
-                    active.disconnect(signal)
-                if callback:
-                    callback()
-
-        signal = connection.connect("state-changed", changed_state)
-
     @run_in_glib_thread
     def deactivate_connection_vpn(self, callback: Optional[Callable] = None) -> None:
         con = self.active_connection
         _logger.debug(f"deactivate_connection uuid: {uuid} connection: {con}")
         if con:
 
             def on_deactivate_connection(a_client: "NM.Client", res, callback=None):
@@ -619,22 +629,22 @@
         else:
             _logger.debug("No active connection to deactivate")
 
     @run_in_glib_thread
     def delete_connection(self, callback: Callable) -> None:
         # We run the disconnected callback early if a delete fail happens
         if self.uuid is None:
-            callback()
             _logger.warning("No uuid found for deleting the connection")
+            callback()
             return
 
         con = self.client.get_connection_by_uuid(self.uuid)
         if con is None:
-            callback()
             _logger.warning(f"No uuid connection found to delete with uuid {uuid}")
+            callback()
             return
 
         # Delete the connection and after that do the callback
         def on_deleted(a_con: "NM.RemoteConnection", res, callback=None):
             try:
                 result = a_con.delete_finish(res)
             except Exception as e:
```

### Comparing `eduvpn_client-4.0.1/eduvpn/notify.py` & `eduvpn_client-4.1.0/eduvpn/notify.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ovpn.py` & `eduvpn_client-4.1.0/eduvpn/ovpn.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/server.py` & `eduvpn_client-4.1.0/eduvpn/server.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/settings.py` & `eduvpn_client-4.1.0/eduvpn/settings.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/storage.py` & `eduvpn_client-4.1.0/eduvpn/storage.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/__main__.py` & `eduvpn_client-4.1.0/eduvpn/ui/__main__.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/app.py` & `eduvpn_client-4.1.0/eduvpn/ui/app.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/search.py` & `eduvpn_client-4.1.0/eduvpn/ui/search.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/stats.py` & `eduvpn_client-4.1.0/eduvpn/ui/stats.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/ui.py` & `eduvpn_client-4.1.0/eduvpn/ui/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,33 +24,20 @@
 
 from eduvpn import __version__
 from eduvpn.i18n import retrieve_country_name
 from eduvpn.server import StatusImage
 from eduvpn.settings import FLAG_PREFIX, IMAGE_PREFIX
 from eduvpn.ui import search
 from eduvpn.ui.stats import NetworkStats
-from eduvpn.ui.utils import (
-    QUIT_ID,
-    get_validity_text,
-    link_markup,
-    should_show_error,
-    show_error_dialog,
-    show_ui_component,
-    style_widget,
-)
-from eduvpn.utils import (
-    ERROR_STATE,
-    get_prefix,
-    get_ui_state,
-    log_exception,
-    run_in_background_thread,
-    run_in_glib_thread,
-    run_periodically,
-    ui_transition,
-)
+from eduvpn.ui.utils import (QUIT_ID, get_validity_text, link_markup,
+                             should_show_error, show_error_dialog,
+                             show_ui_component, style_widget)
+from eduvpn.utils import (ERROR_STATE, get_prefix, get_ui_state, log_exception,
+                          run_in_background_thread, run_in_glib_thread,
+                          run_periodically, ui_transition)
 
 logger = logging.getLogger(__name__)
 
 
 UPDATE_EXPIRY_INTERVAL = 1.0  # seconds
 UPDATE_RENEW_INTERVAL = 60.0  # seconds
 
@@ -113,14 +100,15 @@
             "on_search_activate": self.on_search_activate,
             "on_switch_connection_state": self.on_switch_connection_state,
             "on_toggle_connection_info": self.on_toggle_connection_info,
             "on_profile_row_activated": self.on_profile_row_activated,
             "on_profile_combo_changed": self.on_profile_combo_changed,
             "on_location_row_activated": self.on_location_row_activated,
             "on_acknowledge_error": self.on_acknowledge_error,
+            "on_reconnect_tcp_clicked": self.on_reconnect_tcp_clicked,
             "on_renew_session_clicked": self.on_renew_session_clicked,
             "on_close_window": self.on_close_window,
         }
         builder.connect_signals(handlers)
 
         style_context = self.get_style_context()  # type: ignore
         bg_color = style_context.get_background_color(Gtk.StateFlags.NORMAL)  # type: ignore
@@ -144,14 +132,15 @@
         self.is_selected = False
 
         self.app_logo = builder.get_object("appLogo")
         self.app_logo_info = builder.get_object("appLogoInfo")
         self.info_support_box = builder.get_object("infoSupportBox")
 
         self.failover_text = builder.get_object("failoverText")
+        self.failover_text_timeout_shown = False
         self.failover_text_cancel = None
         self.failover_label = builder.get_object("failoverLabel")
 
         self.page_stack = builder.get_object("pageStack")
         self.back_button_container = builder.get_object("backButtonEventBox")
 
         self.server_list_container = builder.get_object("serverListContainer")
@@ -227,14 +216,15 @@
         self.keyring_do_not_show = builder.get_object("keyringDoNotShow")
 
         self.server_image = builder.get_object("serverImage")
         self.server_label = builder.get_object("serverLabel")
         self.server_support_label = builder.get_object("supportLabel")
 
         self.renew_session_button = builder.get_object("renewSessionButton")
+        self.reconnect_tcp_button = builder.get_object("reconnectTCPButton")
         self.select_profile_combo = builder.get_object("selectProfileCombo")
         self.select_profile_text = builder.get_object("selectProfileText")
 
         self.oauth_page = builder.get_object("openBrowserPage")
         self.oauth_cancel_button = builder.get_object("cancelBrowserButton")
 
         self.loading_page = builder.get_object("loadingPage")
@@ -284,14 +274,15 @@
 
         @run_in_background_thread("register")
         def register():
             try:
                 self.common.register_class_callbacks(self)
                 self.enter_deregistered()
                 self.common.register(debug=self.eduvpn_app.debug)
+                self.common.set_token_updater(self.app.model.save_tokens)
                 self.exit_deregistered()
                 self.app.initialize_network()
             except Exception as e:
                 log_exception(e)
                 if not should_show_error(e):
                     return
                 show_error_dialog(
@@ -488,25 +479,27 @@
         """
         self.current_shown_page = None
 
     def recreate_profile_combo(self, server_info) -> None:
         # Create a store of profiles
         profile_store = Gtk.ListStore(GObject.TYPE_STRING, GObject.TYPE_PYOBJECT)  # type: ignore
         active_profile = 0
-        for index, profile in enumerate(server_info.profiles.profiles):
-            if profile == server_info.profiles.current:
+        sorted_profiles = sorted(server_info.profiles.profiles, key=lambda p: str(p))
+        for index, profile in enumerate(sorted_profiles):
+            if index == server_info.profiles.current:
                 active_profile = index
             profile_store.append([str(profile), profile])  # type: ignore
 
         # Create a new combobox
         # We create a new one every time because Gtk has some weird behaviour regarding the width of the combo box
         # When we add items that are large, the combobox resizes to fit the content
         # However, when we add items again that are all smaller (e.g. for a new server), the combo box does not shrink back
         # The only proper way seems to be to recreate the combobox every time
         combo = Gtk.ComboBoxText.new()  # type: ignore
+        # Sort the model too
         combo.set_model(profile_store)  # type: ignore
         combo.set_active(active_profile)
         combo.set_halign(Gtk.Align.CENTER)
         combo.connect("changed", self.on_profile_combo_changed)
 
         # Get the position of the current combobox in the connection page
         position = self.connection_page.child_get_property(
@@ -609,20 +602,22 @@
     def enter_connecting(self, old_state: str, data):
         self.connection_status_label.set_text(_("Connecting..."))
         self.connection_status_image.set_from_file(StatusImage.CONNECTING.path)
         self.set_connection_switch_state(True)
         # Disable the profile combo box and switch
         self.connection_switch.set_sensitive(False)
         self.select_profile_combo.set_sensitive(False)
+        self.connection_session_label.hide()
 
     @ui_transition(State.CONNECTING, StateType.LEAVE)
     def exit_connecting(self, old_state: str, data):
         # Re-enable the profile combo box and switch
         self.connection_switch.set_sensitive(True)
         self.select_profile_combo.set_sensitive(True)
+        self.connection_session_label.show()
 
     @ui_transition(State.DISCONNECTING, StateType.ENTER)
     def enter_disconnecting(self, old_state: str, data):
         self.connection_status_label.set_text(_("Disconnecting..."))
         self.connection_status_image.set_from_file(StatusImage.CONNECTING.path)
         self.set_connection_switch_state(False)
         # Disable the profile combo box and switch
@@ -771,15 +766,17 @@
             text_cell = Gtk.CellRendererText()
             text_cell.set_property("size-points", 14)
             text_cell.set_property("ypad", 10)
 
             column = Gtk.TreeViewColumn(None, text_cell, text=0)
             profile_tree_view.append_column(column)
 
-        profile_tree_view.set_model(profiles_list_model)
+        sorted_model = Gtk.TreeModelSort(model=profiles_list_model)
+        sorted_model.set_sort_column_id(0, Gtk.SortType.ASCENDING)
+        profile_tree_view.set_model(sorted_model)
         profiles_list_model.clear()
         for profile in profiles.profiles:
             profiles_list_model.append([str(profile), profile])
 
     @ui_transition(State.ASK_PROFILE, StateType.LEAVE)
     def exit_ChooseProfile(self, old_state, data):
         self.show_back_button(False)
@@ -806,15 +803,17 @@
             renderer_pixbuf = Gtk.CellRendererPixbuf()
             column = Gtk.TreeViewColumn("Image", renderer_pixbuf, pixbuf=1)
             location_tree_view.append_column(column)
 
             column = Gtk.TreeViewColumn(None, text_cell, text=0)
             location_tree_view.append_column(column)
 
-            location_tree_view.set_model(location_list_model)
+            sorted_model = Gtk.TreeModelSort(model=location_list_model)
+            sorted_model.set_sort_column_id(0, Gtk.SortType.ASCENDING)
+            location_tree_view.set_model(sorted_model)
 
         location_list_model.clear()
         for location in locations:
             flag_path = get_flag_path(location)
             if flag_path is None:
                 logger.warning(f"No flag found for country code {location}")
                 flag = None
@@ -855,75 +854,87 @@
     def enter_ConnectionStatus(self, old_state: str, server_info):
         self.show_back_button(True)
         self.stop_validity_renew()
         self.stop_connection_info()
         self.show_page(self.connection_page)
         self.update_connection_status(False)
         self.update_connection_server(server_info)
+        self.reconnect_tcp_button.hide()
+        self.renew_session_button.hide()
 
     @ui_transition(State.DISCONNECTED, StateType.LEAVE)
     def exit_ConnectionStatus(self, old_state, new_state):
         self.show_back_button(False)
         self.hide_page(self.connection_page)
         self.pause_connection_info()
 
     @run_in_glib_thread
     def update_failover_text(self, dropped):
         if self.failover_text_cancel is not None:
             GLib.source_remove(self.failover_text_cancel)
         self.failover_text_cancel = None
+
         if not dropped:
-            self.failover_text.hide()
+            if self.failover_text_timeout_shown:
+                # not dropped but it took a while
+                self.reconnect_tcp_button.show()
+                self.failover_label.set_text(
+                    "There might be a problem with the VPN connection. If you observe any issues, press 'Reconnect with TCP'."
+                )
+                self.failover_text.show()
         else:
             # Show the failover text for 10 seconds
             self.failover_text_cancel = GLib.timeout_add(
                 10_000, self.hide_failover_text_timeout
             )
             self.failover_label.set_text(
-                "The VPN was unable to reach the internet. We have switched to a different VPN protocol"
+                "The VPN had issues with connectivity. We have switched to a different protocol"
             )
             self.failover_text.show()
 
     def hide_failover_text_timeout(self):
         self.failover_text_cancel = None
         self.failover_text.hide()
         return False
 
     def show_failover_text_timeout(self):
         self.failover_text_cancel = None
+        self.failover_text_timeout_shown = True
         self.failover_text.show()
         return False
 
     @ui_transition(State.CONNECTED, StateType.LEAVE)
     def leave_ConnectedState(self, old_state, server_info):
         if self.failover_text_cancel is not None:
             GLib.source_remove(self.failover_text_cancel)
+        self.failover_text_timeout_shown = False
+        self.reconnect_tcp_button.hide()
         self.failover_text_cancel = None
         self.failover_text.hide()
         self.connection_info_expander.hide()
+        self.renew_session_button.hide()
 
     @ui_transition(State.CONNECTED, StateType.ENTER)
     def enter_ConnectedState(self, old_state, server_info):
+        self.renew_session_button.hide()
         self.show_page(self.connection_page)
         self.show_back_button(False)
         is_expanded = self.connection_info_expander.get_expanded()
         if is_expanded:
             self.start_connection_info()
         self.update_connection_status(True)
         self.update_connection_server(server_info)
         self.start_validity_renew(server_info)
         self.connection_info_expander.show()
 
         if self.app.model.should_failover():
             self.failover_text_cancel = GLib.timeout_add(
-                1000, self.show_failover_text_timeout
-            )
-            self.failover_label.set_text(
-                "We have not yet determined that the VPN is able to reach the internet..."
+                2500, self.show_failover_text_timeout
             )
+            self.failover_label.set_text("Checking the VPN for connectivity issues...")
             self.call_model("start_failover", self.update_failover_text)
             return
 
     def start_validity_renew(self, server_info) -> None:
         self.connection_validity_thread_cancel = run_periodically(
             run_in_glib_thread(
                 partial(self.update_connection_validity, server_info.expire_time)
@@ -948,14 +959,15 @@
 
     def on_info_delete(self, widget, event):
         logger.debug("info dialog delete event")
         return widget.hide_on_delete()
 
     def on_info_button(self, widget: EventBox, event: EventButton) -> None:
         logger.debug("clicked info button")
+        self.info_dialog.set_title(f"{self.app.variant.name} Info")
         self.info_dialog.show()
         self.info_dialog.run()
         self.info_dialog.hide()
 
     def on_go_back(self, widget: EventBox, event: EventButton) -> None:
         logger.debug("clicked on go back")
         self.call_model("go_back")
@@ -1212,14 +1224,23 @@
         # TODO: Handle this case
 
     def on_renew_session_clicked(self, event):
         logger.debug("clicked on renew session")
 
         self.call_model("renew_session")
 
+    def on_reconnect_tcp_clicked(self, event):
+        logger.debug("clicked on reconnect TCP")
+
+        def on_reconnected(_: bool):
+            logger.debug("done reconnecting with tcp")
+            self.reconnect_tcp_button.hide()
+
+        self.call_model("reconnect_tcp", on_reconnected)
+
     def on_close_window(self, window: "EduVpnGtkWindow", event: Event) -> bool:
         logger.debug("clicked on close window")
         self.hide()  # type: ignore
         application = self.get_application()  # type: ignore
         if application:
             application.on_window_closed()  # type: ignore
         return True
```

### Comparing `eduvpn_client-4.0.1/eduvpn/ui/utils.py` & `eduvpn_client-4.1.0/eduvpn/ui/utils.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/utils.py` & `eduvpn_client-4.1.0/eduvpn/utils.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/eduvpn/variants.py` & `eduvpn_client-4.1.0/eduvpn/variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from pathlib import Path
 from typing import Optional, Tuple
 
 from eduvpn import __version__, settings
 from eduvpn.config import Configuration
-from eduvpn.settings import (
-    CLIENT_ID,
-    CONFIG_PREFIX,
-    LETSCONNECT_CLIENT_ID,
-    LETSCONNECT_CONFIG_PREFIX,
-)
+from eduvpn.settings import (CLIENT_ID, CONFIG_PREFIX, LETSCONNECT_CLIENT_ID,
+                             LETSCONNECT_CONFIG_PREFIX)
 
 
 class ApplicationVariant:
     def __init__(
         self,
         app_id: str,
         client_id: str,
```

### Comparing `eduvpn_client-4.0.1/eduvpn_client.egg-info/PKG-INFO` & `eduvpn_client-4.1.0/eduvpn_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eduvpn-client
-Version: 4.0.1
+Version: 4.1.0
 Summary: eduVPN client
 Home-page: https://github.com/eduvpn/python-eduvpn-client
 Author: Jeroen Wijenbergh
 Author-email: jeroen.wijenbergh@geant.org
 License: GPL3
 Keywords: vpn openvpn networking security
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `eduvpn_client-4.0.1/eduvpn_client.egg-info/SOURCES.txt` & `eduvpn_client-4.1.0/eduvpn_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 doc/Makefile
 doc/conf.py
 doc/developer.rst
 doc/flow.dia
 doc/flow.png
 doc/index.rst
 doc/installation.rst
+doc/knownissues.rst
 doc/requirements.txt
 doc/screenshot.png
+doc/updating.rst
 doc/usage.rst
 eduvpn/__init__.py
 eduvpn/__main__.py
 eduvpn/app.py
 eduvpn/cli.py
 eduvpn/config.py
 eduvpn/connection.py
@@ -45,14 +47,15 @@
 eduvpn_client.egg-info/requires.txt
 eduvpn_client.egg-info/top_level.txt
 share/applications/org.eduvpn.client.desktop
 share/applications/org.letsconnect-vpn.client.desktop
 share/eduvpn/country_codes.json
 share/eduvpn/eduvpn.png
 share/eduvpn/builder/mainwindow.ui
+share/eduvpn/builder/mainwindow.ui~
 share/eduvpn/images/app-icon-circle.svg
 share/eduvpn/images/app-icon-circle@2x.png
 share/eduvpn/images/app-icon-circle@3x.png
 share/eduvpn/images/back.png
 share/eduvpn/images/back@2x.png
 share/eduvpn/images/back@3x.png
 share/eduvpn/images/chevron-down.png
```

### Comparing `eduvpn_client-4.0.1/setup.py` & `eduvpn_client-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from glob import glob
 
 from setuptools import setup, find_packages
 
-__version__ = "4.0.1"
+__version__ = "4.1.0"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 install_requires = [
     'wheel',
-    'eduvpn_common',
+    'eduvpn_common==1.1.0',
 ]
 
 tests_require = [
     'pytest',
     'pycodestyle',
 ]
```

### Comparing `eduvpn_client-4.0.1/share/eduvpn/builder/mainwindow.ui` & `eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui`

 * *Files 1% similar despite different names*

#### Comparing `eduvpn_client-4.0.1/share/eduvpn/builder/mainwindow.ui` & `eduvpn_client-4.1.0/share/eduvpn/builder/mainwindow.ui`

```diff
@@ -802,15 +802,14 @@
                             <property name="position">0</property>
                           </packing>
                         </child>
                         <child>
                           <object class="GtkLabel" id="failoverLabel">
                             <property name="visible">True</property>
                             <property name="can-focus">False</property>
-                            <property name="label" translatable="yes"/>
                             <property name="wrap">True</property>
                           </object>
                           <packing>
                             <property name="expand">False</property>
                             <property name="fill">True</property>
                             <property name="position">1</property>
                           </packing>
@@ -819,14 +818,30 @@
                       <packing>
                         <property name="expand">False</property>
                         <property name="fill">True</property>
                         <property name="position">10</property>
                       </packing>
                     </child>
                     <child>
+                      <object class="GtkButton" id="reconnectTCPButton">
+                        <property name="label" translatable="yes">Reconnect with TCP</property>
+                        <property name="visible">False</property>
+                        <property name="can-focus">True</property>
+                        <property name="receives-default">True</property>
+                        <property name="halign">center</property>
+                        <property name="image-position">top</property>
+                        <signal name="clicked" handler="on_reconnect_tcp_clicked" swapped="no"/>
+                      </object>
+                      <packing>
+                        <property name="expand">False</property>
+                        <property name="fill">True</property>
+                        <property name="position">11</property>
+                      </packing>
+                    </child>
+                    <child>
                       <object class="GtkExpander" id="connectionInfoExpander">
                         <property name="visible">True</property>
                         <property name="can-focus">True</property>
                         <property name="halign">center</property>
                         <signal name="activate" handler="on_toggle_connection_info" swapped="no"/>
                         <child>
                           <object class="GtkFrame">
@@ -1011,15 +1026,15 @@
                             </attributes>
                           </object>
                         </child>
                       </object>
                       <packing>
                         <property name="expand">False</property>
                         <property name="fill">False</property>
-                        <property name="position">11</property>
+                        <property name="position">12</property>
                       </packing>
                     </child>
                   </object>
                   <packing>
                     <property name="position">4</property>
                   </packing>
                 </child>
@@ -1282,15 +1297,15 @@
                 <property name="orientation">vertical</property>
                 <child>
                   <object class="GtkLabel">
                     <property name="visible">True</property>
                     <property name="can-focus">True</property>
                     <property name="halign">start</property>
                     <property name="label" translatable="yes">If you have found a bug/issue with the client itself,
-you can report an issue on the &lt;a href=&quot;https://github.com/eduvpn/eduvpn-common&quot;&gt;GitHub repository&lt;/a&gt;.
+you can report an issue on the &lt;a href=&quot;https://github.com/eduvpn/python-eduvpn-client/issues&quot;&gt;GitHub repository&lt;/a&gt;.
 Make sure to include the log file if applicable, which is available
 at the following location:</property>
                     <property name="use-markup">True</property>
                   </object>
                   <packing>
                     <property name="expand">False</property>
                     <property name="fill">False</property>
```

### Comparing `eduvpn_client-4.0.1/share/eduvpn/country_codes.json` & `eduvpn_client-4.1.0/share/eduvpn/country_codes.json`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/eduvpn.png` & `eduvpn_client-4.1.0/share/eduvpn/eduvpn.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle.svg` & `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle.svg`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/app-icon-circle@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/app-icon-circle@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/back.png` & `eduvpn_client-4.1.0/share/eduvpn/images/back.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/back@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/back@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/back@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/back@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/chevron-down@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/chevron-down@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/chevron-right@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/chevron-right@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/cross@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/cross@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/cross@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/cross@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connected@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connected@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-connecting@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-connecting@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-default.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-default@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-default@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-default@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/desktop-not-connected@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/desktop-not-connected@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/earth-icon@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/earth-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/edu-vpn-logo@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/edu-vpn-logo@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AF@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AI@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AQ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/AZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/AZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Artsakh@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Artsakh@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Artsakh@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BD@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BF@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BH@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BI@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-BO@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-BO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-BO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SE@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BQ-SE@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BQ-SE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/BZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/BZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-BC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-BC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-MB@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-MB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NB@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-NU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-NU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-ON@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-ON@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-PE@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-PE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-QC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-QC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-SK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-SK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CA-YT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CA-YT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CD@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CF@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CV@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CW@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CX@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/CY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/CY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DJ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DJ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/DZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/DZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EH@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ER@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ER@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ES-CT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ES-CT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ET@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ET@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/EU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/EU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FJ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-MQ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-MQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-TF@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-TF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/FR-YT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/FR-YT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-SCT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-SCT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB-Symbol@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB-Symbol@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GB@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GD@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE-AB@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GE-AB@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GE-AB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GH@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GQ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GQ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GQ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/GY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/GY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/HR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/HR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/IO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/IO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JE@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/JP@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/JP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KE@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KG@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KI@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KP@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/KZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/KZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Kurdistan@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Kurdistan@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Kurdistan@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/LY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/LY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MH@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MP@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MR@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MV@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MX@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/MZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/MZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NP@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NP@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/NZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/NZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Netherlands Antilles@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/OM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/OM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PF@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PF@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PH@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PH@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PH@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PR@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PT@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PT@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/PY@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/PY@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/QA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/QA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/RW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/RW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Red Peak Flag (NZ)@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SB@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SB@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SD@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SD@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SH-HL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SH-HL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SO@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SO@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SO@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SS@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SS@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ST@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ST@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SV@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SX@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SX@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SX@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/SZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/SZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Sealand@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Sealand@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TJ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TJ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TK@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TK@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TL@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TL@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TM@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TM@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TM@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TR@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TR@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TV@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TV@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/TZ@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/TZ@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/Turkish Republic of Northern Cyprus@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/UG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/UG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VC@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VC@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VE@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VE@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VG@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VG@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VI@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VI@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VN@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VN@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VN@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/VU@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/VU@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZA@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZA@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@1,5x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@1,5x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/flags/png/ZW@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/flags/png/ZW@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/group@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/group@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/group@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/group@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute-icon@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/institute@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/institute@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/question-icon@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/question-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/server-icon-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/server-icon-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/server-icon-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/server-icon@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/server-icon@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/server-icon@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/server-icon@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings-dark.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings-dark@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings-dark@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings-dark@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings@2x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/eduvpn/images/settings@3x.png` & `eduvpn_client-4.1.0/share/eduvpn/images/settings@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/128x128/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/128x128/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/256x256/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/256x256/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/48x48/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/48x48/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/512x512/apps/org.eduvpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.eduvpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png` & `eduvpn_client-4.1.0/share/icons/hicolor/512x512/apps/org.letsconnect-vpn.client.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/app-icon-circle.svg` & `eduvpn_client-4.1.0/share/letsconnect/images/app-icon-circle.svg`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/letsconnect.png` & `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/letsconnect@2x.png` & `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/letsconnect@3x.png` & `eduvpn_client-4.1.0/share/letsconnect/images/letsconnect@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/server-illustration.png` & `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/server-illustration@2x.png` & `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@2x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/letsconnect/images/server-illustration@3x.png` & `eduvpn_client-4.1.0/share/letsconnect/images/server-illustration@3x.png`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/locale/de_DE/LC_MESSAGES/eduVPN.mo` & `eduvpn_client-4.1.0/share/locale/de_DE/LC_MESSAGES/eduVPN.mo`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/share/locale/es_LA/LC_MESSAGES/eduVPN.mo` & `eduvpn_client-4.1.0/share/locale/es_LA/LC_MESSAGES/eduVPN.mo`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/tests/mock_config.py` & `eduvpn_client-4.1.0/tests/mock_config.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/tests/test_nm.py` & `eduvpn_client-4.1.0/tests/test_nm.py`

 * *Files identical despite different names*

### Comparing `eduvpn_client-4.0.1/tests/test_stats.py` & `eduvpn_client-4.1.0/tests/test_stats.py`

 * *Files identical despite different names*

