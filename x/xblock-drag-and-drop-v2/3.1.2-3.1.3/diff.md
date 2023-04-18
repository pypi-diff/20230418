# Comparing `tmp/xblock-drag-and-drop-v2-3.1.2.tar.gz` & `tmp/xblock-drag-and-drop-v2-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-drag-and-drop-v2-3.1.2.tar", last modified: Mon Mar  6 12:01:32 2023, max compression
+gzip compressed data, was "xblock-drag-and-drop-v2-3.1.3.tar", last modified: Tue Apr 18 10:23:45 2023, max compression
```

## Comparing `xblock-drag-and-drop-v2-3.1.2.tar` & `xblock-drag-and-drop-v2-3.1.3.tar`

### file list

```diff
@@ -1,248 +1,165 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    12549 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    34307 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    21568 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/
--rw-r--r--   0 runner    (1001) docker     (122)      102 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/default_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    53365 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/drag_and_drop_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.055026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19892 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28625 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.055026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16505 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24470 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.055026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.055026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32171 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38531 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.055026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25388 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16671 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24859 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18883 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25607 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11388 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22806 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.067026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18941 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15579 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23406 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23285 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15801 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24322 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16196 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24372 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26457 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18165 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.059026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20913 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/css/
--rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/css/drag_and_drop.css
--rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/css/drag_and_drop_edit.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/img/
--rw-r--r--   0 runner    (1001) docker     (122)    34942 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/img/triangle.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/
--rw-r--r--   0 runner    (1001) docker     (122)    86843 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/drag_and_drop.js
--rw-r--r--   0 runner    (1001) docker     (122)    41638 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/drag_and_drop_edit.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ar/
--rw-r--r--   0 runner    (1001) docker     (122)    39006 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ar/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.071026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/de/
--rw-r--r--   0 runner    (1001) docker     (122)    18357 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/de/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/en/
--rw-r--r--   0 runner    (1001) docker     (122)     3578 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/en/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/eo/
--rw-r--r--   0 runner    (1001) docker     (122)    64209 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/eo/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/es_419/
--rw-r--r--   0 runner    (1001) docker     (122)    20270 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/es_419/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/fr/
--rw-r--r--   0 runner    (1001) docker     (122)    19590 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/fr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/he/
--rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/he/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/hi/
--rw-r--r--   0 runner    (1001) docker     (122)     6854 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/hi/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/it/
--rw-r--r--   0 runner    (1001) docker     (122)     7058 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/it/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ja/
--rw-r--r--   0 runner    (1001) docker     (122)    21316 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ja/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ko/
--rw-r--r--   0 runner    (1001) docker     (122)    22577 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ko/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/nl/
--rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/nl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pl/
--rw-r--r--   0 runner    (1001) docker     (122)    16851 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pl/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_BR/
--rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_BR/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_PT/
--rw-r--r--   0 runner    (1001) docker     (122)    18514 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_PT/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ru/
--rw-r--r--   0 runner    (1001) docker     (122)    37990 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ru/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/tr/
--rw-r--r--   0 runner    (1001) docker     (122)     5079 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/tr/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/zh_CN/
--rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/zh_CN/text.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)    84693 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
--rw-r--r--   0 runner    (1001) docker     (122)    16608 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/themes/
--rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/themes/apros.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/drag_and_drop.html
--rw-r--r--   0 runner    (1001) docker     (122)    16156 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/js_templates.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.075026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19892 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28625 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16505 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24470 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      380 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/en/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32171 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    38531 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25388 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16671 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24859 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18883 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25607 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11388 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22806 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    18941 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ko/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15579 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23406 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.079026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23285 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    15801 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24322 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    16196 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24372 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/rtl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/rtl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26457 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    18165 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.063026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo
--rw-r--r--   0 runner    (1001) docker     (122)    20913 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po
--rw-r--r--   0 runner    (1001) docker     (122)    11732 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      110 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4969 2023-03-06 12:01:26.000000 xblock-drag-and-drop-v2-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-06 12:01:32.083026 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34307 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6313 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-06 12:01:32.000000 xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    13122 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (122)    35136 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    35236 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    21924 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      102 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4294 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/default_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53365 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/drag_and_drop_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/
+-rw-r--r--   0 runner    (1001) docker     (122)    19803 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop.css
+-rw-r--r--   0 runner    (1001) docker     (122)     8911 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop_edit.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/
+-rw-r--r--   0 runner    (1001) docker     (122)    34942 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/triangle.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    86843 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop.js
+-rw-r--r--   0 runner    (1001) docker     (122)    41638 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop_edit.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/
+-rw-r--r--   0 runner    (1001) docker     (122)    39006 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/
+-rw-r--r--   0 runner    (1001) docker     (122)    18357 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/
+-rw-r--r--   0 runner    (1001) docker     (122)     3578 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/
+-rw-r--r--   0 runner    (1001) docker     (122)    64209 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/
+-rw-r--r--   0 runner    (1001) docker     (122)    20270 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/
+-rw-r--r--   0 runner    (1001) docker     (122)    19590 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/
+-rw-r--r--   0 runner    (1001) docker     (122)    22437 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/
+-rw-r--r--   0 runner    (1001) docker     (122)     6854 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.132537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/
+-rw-r--r--   0 runner    (1001) docker     (122)     7058 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/
+-rw-r--r--   0 runner    (1001) docker     (122)    21316 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/
+-rw-r--r--   0 runner    (1001) docker     (122)    22577 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/
+-rw-r--r--   0 runner    (1001) docker     (122)     5024 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/
+-rw-r--r--   0 runner    (1001) docker     (122)    16851 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/
+-rw-r--r--   0 runner    (1001) docker     (122)    18092 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/
+-rw-r--r--   0 runner    (1001) docker     (122)    18514 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/
+-rw-r--r--   0 runner    (1001) docker     (122)    37990 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/
+-rw-r--r--   0 runner    (1001) docker     (122)     5079 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/text.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)    84693 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js
+-rw-r--r--   0 runner    (1001) docker     (122)    16608 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1641 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/apros.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.136537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16156 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7944 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/js_templates.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.120537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19892 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28625 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2575 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16505 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24470 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    16953 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32171 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    38531 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.140538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18375 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25388 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16671 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24859 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18883 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25607 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11388 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22806 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18256 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4213 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    18941 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    13802 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23151 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.144538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    15579 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23406 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1280 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    13671 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23285 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.124537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    15801 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24322 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16196 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24372 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    20418 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26457 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    18165 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27878 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1907 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    17841 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.128538 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.148537 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    20913 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11732 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      110 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4959 2023-04-18 10:23:36.000000 xblock-drag-and-drop-v2-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-18 10:23:45.152537 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    35236 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4346 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-04-18 10:23:45.000000 xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/top_level.txt
```

### Comparing `xblock-drag-and-drop-v2-3.1.2/Changelog.md` & `xblock-drag-and-drop-v2-3.1.3/Changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.1.3 (2023-04-15)
+--------------------------
+
+* Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
+  * `conf/locale` directory is now the source of truth for translations.
+  * `translations` directory is now a symbolic link for backwards compatibility.
+  * `locale` symbolic link is deleted to avoid too many symbolic links.
+  * `en` translations are now extracted into `django.po` instead of `text.po`.
+  * `en` `text.po` is now a symbolic link to `django.po` for backwards compatibility.
+
 Version 3.1.0 (2023-01-31)
 --------------------------
 
 * Upgrade to be compatible with `bleach==6.0.0` and `bleach<6.0.0`
 * Make the dependency on the `css` extras explicit.
 
 Version 3.0.0 (2022-11-18)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_391rlhui_/tmp9yim854p_TarContainer/0/1.md", line 333, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_391rlhui_/tmp9yim854p_TarContainer/0/1.md", line 333, column 0: CDATA terminal not found*

```diff
@@ -1,6 +1,13 @@
-Drag and Drop XBlock changelog ============================== Version 3.1.0
-(2023-01-31) -------------------------- * Upgrade to be compatible with
-`bleach==6.0.0` and `bleach<6.0.0` * Make the dependency on the `css` extras
-explicit. Version 3.0.0 (2022-11-18) --------------------------- * Sanitize
-HTML tags to prevent XSS vulnerabilities. BREAKING CHANGE: Disallowed HTML tags
-(e.g. `
+Drag and Drop XBlock changelog ============================== Version 3.1.3
+(2023-04-15) -------------------------- * Prepare repository for upcoming
+changes related to [openedx-translations](https://github.com/openedx/openedx-
+translations). * `conf/locale` directory is now the source of truth for
+translations. * `translations` directory is now a symbolic link for backwards
+compatibility. * `locale` symbolic link is deleted to avoid too many symbolic
+links. * `en` translations are now extracted into `django.po` instead of
+`text.po`. * `en` `text.po` is now a symbolic link to `django.po` for backwards
+compatibility. Version 3.1.0 (2023-01-31) -------------------------- * Upgrade
+to be compatible with `bleach==6.0.0` and `bleach<6.0.0` * Make the dependency
+on the `css` extras explicit. Version 3.0.0 (2022-11-18) ----------------------
+----- * Sanitize HTML tags to prevent XSS vulnerabilities. BREAKING CHANGE:
+Disallowed HTML tags (e.g. `
```

### Comparing `xblock-drag-and-drop-v2-3.1.2/LICENSE` & `xblock-drag-and-drop-v2-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/PKG-INFO` & `xblock-drag-and-drop-v2-3.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 3.1.2
+Version: 3.1.3
 Summary: XBlock - Drag-and-Drop v2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Drag and Drop XBlock v2
 =======================
@@ -531,14 +531,16 @@
 * Default English translation
 * Fake "Esperanto" translation used to test i18n/l10n.
 
 Updates to translated strings are supposed to be propagated to `text.po` files. EdX [i18n_tools][edx-i18n-tools] is used here along GNU Gettext and a Makefile for automation.
 
 [edx-i18n-tools]: https://github.com/openedx/i18n-tools
 
+Note: currently `translations` directory is a symbolic link to `conf/locale` directory. Also, 'text.po' file for locale code `en` is a symbolic link to `conf/locale/en/LC_MESSAGES/django.po` file. Both links works as a transition step to fully moving translation files to [openedx-translations](https://github.com/openedx/openedx-translations) repository
+
 Translatable strings
 --------------------
 ```bash
 $ make extract_translations
 ```
 
 Note that this command generates `text.po` which is supposed to contain
@@ -587,14 +589,24 @@
 -------------------------------------
 To release a new version, update .travis.yml and setup.py to point to your new intended version number and create a new release with that version tag via Github.
 
 
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.1.3 (2023-04-15)
+--------------------------
+
+* Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
+  * `conf/locale` directory is now the source of truth for translations.
+  * `translations` directory is now a symbolic link for backwards compatibility.
+  * `locale` symbolic link is deleted to avoid too many symbolic links.
+  * `en` translations are now extracted into `django.po` instead of `text.po`.
+  * `en` `text.po` is now a symbolic link to `django.po` for backwards compatibility.
+
 Version 3.1.0 (2023-01-31)
 --------------------------
 
 * Upgrade to be compatible with `bleach==6.0.0` and `bleach<6.0.0`
 * Make the dependency on the `css` extras explicit.
 
 Version 3.0.0 (2022-11-18)
```

### Comparing `xblock-drag-and-drop-v2-3.1.2/README.md` & `xblock-drag-and-drop-v2-3.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -523,14 +523,16 @@
 * Default English translation
 * Fake "Esperanto" translation used to test i18n/l10n.
 
 Updates to translated strings are supposed to be propagated to `text.po` files. EdX [i18n_tools][edx-i18n-tools] is used here along GNU Gettext and a Makefile for automation.
 
 [edx-i18n-tools]: https://github.com/openedx/i18n-tools
 
+Note: currently `translations` directory is a symbolic link to `conf/locale` directory. Also, 'text.po' file for locale code `en` is a symbolic link to `conf/locale/en/LC_MESSAGES/django.po` file. Both links works as a transition step to fully moving translation files to [openedx-translations](https://github.com/openedx/openedx-translations) repository
+
 Translatable strings
 --------------------
 ```bash
 $ make extract_translations
 ```
 
 Note that this command generates `text.po` which is supposed to contain
```

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/compat.py` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/compat.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/default_data.py` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/default_data.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/drag_and_drop_v2.py` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/drag_and_drop_v2.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ar/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ar/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/config.yaml` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/config.yaml`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/de/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/de/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/en/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/eo/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/eo/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/es_419/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/es_419/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/fr_CA/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/fr_CA/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/he/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/he/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/hi/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/hi/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/it/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/it/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ja/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ja/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ko/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ko/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/nl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/nl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_BR/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_BR/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/pt_PT/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/pt_PT/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/rtl/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/rtl/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/ru/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/ru/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/settings.py` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/tr/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/tr/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/LC_MESSAGES/text.mo` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.mo`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/locale/zh_CN/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/zh_CN/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/css/drag_and_drop.css` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/css/drag_and_drop_edit.css` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/css/drag_and_drop_edit.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/img/triangle.png` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/img/triangle.png`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/drag_and_drop.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/drag_and_drop_edit.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/drag_and_drop_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ar/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ar/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/de/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/de/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/en/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/en/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/eo/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/eo/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/es_419/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/es_419/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/fr/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/fr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/he/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/he/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/hi/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/hi/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/it/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/it/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ja/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ja/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ko/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ko/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/nl/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/nl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pl/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pl/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_BR/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_BR/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/pt_PT/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/pt_PT/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/ru/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/ru/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/tr/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/tr/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/translations/zh_CN/text.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/translations/zh_CN/text.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/handlebars-v1.1.2.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/js/vendor/virtual-dom-1.3.0.min.js`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/public/themes/apros.css` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/public/themes/apros.css`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/drag_and_drop_edit.html` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/drag_and_drop_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/templates/html/js_templates.html` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/templates/html/js_templates.html`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/translations/en/LC_MESSAGES/text.po`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/drag_and_drop_v2/utils.py` & `xblock-drag-and-drop-v2-3.1.3/drag_and_drop_v2/utils.py`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/requirements/constraints.txt` & `xblock-drag-and-drop-v2-3.1.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `xblock-drag-and-drop-v2-3.1.2/setup.py` & `xblock-drag-and-drop-v2-3.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,10 +116,10 @@
     long_description=README + '\n\n' + CHANGELOG,
     long_description_content_type='text/markdown',
     install_requires=load_requirements('requirements/base.in'),
     entry_points={
         'xblock.v1': 'drag-and-drop-v2 = drag_and_drop_v2:DragAndDropBlock',
     },
     packages=['drag_and_drop_v2'],
-    package_data=package_data("drag_and_drop_v2", ["static", "templates", "public", "translations", "locale"]),
+    package_data=package_data("drag_and_drop_v2", ["static", "templates", "public", "translations"]),
     python_requires=">=3.8",
 )
```

### Comparing `xblock-drag-and-drop-v2-3.1.2/xblock_drag_and_drop_v2.egg-info/PKG-INFO` & `xblock-drag-and-drop-v2-3.1.3/xblock_drag_and_drop_v2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xblock-drag-and-drop-v2
-Version: 3.1.2
+Version: 3.1.3
 Summary: XBlock - Drag-and-Drop v2
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Drag and Drop XBlock v2
 =======================
@@ -531,14 +531,16 @@
 * Default English translation
 * Fake "Esperanto" translation used to test i18n/l10n.
 
 Updates to translated strings are supposed to be propagated to `text.po` files. EdX [i18n_tools][edx-i18n-tools] is used here along GNU Gettext and a Makefile for automation.
 
 [edx-i18n-tools]: https://github.com/openedx/i18n-tools
 
+Note: currently `translations` directory is a symbolic link to `conf/locale` directory. Also, 'text.po' file for locale code `en` is a symbolic link to `conf/locale/en/LC_MESSAGES/django.po` file. Both links works as a transition step to fully moving translation files to [openedx-translations](https://github.com/openedx/openedx-translations) repository
+
 Translatable strings
 --------------------
 ```bash
 $ make extract_translations
 ```
 
 Note that this command generates `text.po` which is supposed to contain
@@ -587,14 +589,24 @@
 -------------------------------------
 To release a new version, update .travis.yml and setup.py to point to your new intended version number and create a new release with that version tag via Github.
 
 
 Drag and Drop XBlock changelog
 ==============================
 
+Version 3.1.3 (2023-04-15)
+--------------------------
+
+* Prepare repository for upcoming changes related to [openedx-translations](https://github.com/openedx/openedx-translations).
+  * `conf/locale` directory is now the source of truth for translations.
+  * `translations` directory is now a symbolic link for backwards compatibility.
+  * `locale` symbolic link is deleted to avoid too many symbolic links.
+  * `en` translations are now extracted into `django.po` instead of `text.po`.
+  * `en` `text.po` is now a symbolic link to `django.po` for backwards compatibility.
+
 Version 3.1.0 (2023-01-31)
 --------------------------
 
 * Upgrade to be compatible with `bleach==6.0.0` and `bleach<6.0.0`
 * Make the dependency on the `css` extras explicit.
 
 Version 3.0.0 (2022-11-18)
```

